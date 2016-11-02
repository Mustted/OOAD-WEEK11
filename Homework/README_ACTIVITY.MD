# OOAD-WEEK11 HOMEWORK
## ACTIVITY DIAGRAM

  Activity 1
  Code
```
  @startuml
  (*) --> "Activity"
  "Activity" --> (*)

  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/activity1.png?raw=true">

----------------------------------------------------------------

  Activity 2
  Code
```
   @startuml
  (*) --> "User/Pass"

  if "Process" then
    -->[true]"Desktop"
    -->"Another desktop"
    --> (*)
  else
    -->[false] "Return"
    -right->[Not match] "User/Pass"
  endif

  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/Activity2.png?raw=true">

----------------------------------------------------------------
Activity 3
  Code
```
    @startuml
  (*)  --> "Check Address"
  If "Input Address match " then
  --> [Yes] "Data Address"
  --> "Output"
  else
  --> "Output"
  Endif
  -->(*)
  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/Activity3.png?raw=true">

----------------------------------------------------------------
Activity 4
  Code
```
  @startuml

  (*) --> ===B1=== 
  --> "User 1"
  --> ===B2===

  ===B1=== --> "User 2"
  --> ===B2===

  --> (*)

  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/Activity4.png?raw=true">

----------------------------------------------------------------
Activity 5
  Code
  
```
  @startuml

  skinparam backgroundColor #AAFFFF
  skinparam activity {
    StartColor red
    BarColor SaddleBrown 
    EndColor Silver
    BackgroundColor Peru
    BackgroundColor<< Begin >> Olive
    BorderColor Peru
    FontName Impact
  }

  (*) --> "Select the ball" << Begin >>
  --> === S1 ===
  --> Throws the ball
  --> === S2 ===
  --> Serve
  --> === S3 ===
  --> WavesArmes
  --> (*)

  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/Activity5.png?raw=true">

----------------------------------------------------------------
