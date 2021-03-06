# OOAD-WEEK11 HOMEWORK
## State DIAGRAM

  State 1
  Code
```
  @startuml

  [*] -right-> State1
  State1  -right-> State2
  State2 --> State3
  State3  -left-> State4
  State4 --> [*]

  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/State1.png?raw=true">

----------------------------------------------------------------
  State 2
  Code
```
  @startuml
  skinparam backgroundColor LightYellow
  skinparam state {
    StartColor Green
    EndColor Red
    BackgroundColor Blue
    BackgroundColor<<Warning>> pink
    BorderColor Gray
    FontName Impact
  }

  [*] --> Active

  state "Active" as Active {
    state "Wait mode" as Wait <<Warning>>
    state "Configuring mode" as Configuring
    [*] --> Wait
    Wait --> Configuring : EvConfig
    Configuring --> Wait : EvConfig
  }

  Active --> [*]
  @enduml
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/State2.png?raw=true">

----------------------------------------------------------------
  State 3
  Code
```
  @startuml

  [*] -right-> Input
  Input : insert smart card

  Input -> Read
  Read : Reading data

  Read -right-> Display
  Display -right-> [*]

  @enduml

```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/State3.png?raw=true">

----------------------------------------------------------------
  State 4
  Code
```
  @startuml
  [*] --> Active

  state Active {
    [*] ->Program
    Program --> AllProgram 
    --
    [*] -->Internet
    Internet --> Safari 
    --
    [*] -->MSOffice
    MSOffice --> Word 
  }

  @enduml
  
```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/State4.png?raw=true">

----------------------------------------------------------------
  State 5
  Code
```
  @startuml
  [*] -->Address
  Address --> Data

  note left of Address : Address data

  note right of Data
    Seaching Address Data
    Select Data
  end note

  @enduml

```
<img src="https://github.com/Mustted/OOAD-WEEK11/blob/master/Homework/State5.png?raw=true">

----------------------------------------------------------------
