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
<img src="">

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
<img src="">

----------------------------------------------------------------
 State 3
  Code
```
  
```
<img src="">

----------------------------------------------------------------
State 4
  Code
```
  
```
<img src="">

----------------------------------------------------------------
State 5
  Code
```
  
```
<img src="">

----------------------------------------------------------------
