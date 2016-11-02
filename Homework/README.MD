
@startuml

[*] -right-> State1
State1  -right-> State2
State2 --> State3
State3  -left-> State4
State4 --> [*]

@enduml
