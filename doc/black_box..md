# Finger Fource Measurement Device Black Box
```
@startuml 

title Finger Strength Sensor Black Box
skinparam rectangle {
    BackgroundColor White
    BorderColor Black
}
skinparam note {
    BackgroundColor #FFFFE0
    BorderColor Black
}
skinparam legend {
    BorderColor Black
    BackgroundColor White
}

legend right
    |<b>LEGEND</b>|
    | <color:#FF6347>Mechanical interfaces</color> |
    | <color:#4682B4>Logical interfaces</color> |
    | <color:#F0E68C>Electrical interfaces</color> |
endlegend

<style>


sensor_style {
  FontSize 30
  BackGroundColor yellow
  Margin 30
  Padding 50
}

</style>


rectangle "Finger Strength Sensor" as sensor #f5f5f5 {
    skinparam {
        BackgroundColor #f5f5f5
        BorderColor Black
        RoundCorner 15
        FontSize 30
    }

}

note right of sensor
    <b><color:#3CB371>MECHANICAL INTERFACES:</color></b>
    - Force input for measuring finger strength
    - Potentiometer or encoder to adjust settings
    - Button for user interaction
end note

note left of sensor
    <b><color:#4682B4>LOGICAL INTERFACES:</color></b>
    - Sends data via BLE to PC
    - UART for additional communication
    - Status indicated via LED
    - Displays values on display
end note



rectangle "Power Supply" as ps #F0E68C
ps --> sensor : 5V DC input

note left of ps
    <b><color:#F0E68C>ELECTRICAL INTERFACES:</color></b>
    - Power Supply: 5V DC input
end note

rectangle "Force Input" as force #3CB371
force --> sensor : Measures force

rectangle "Potentiometer or Encoder" as pot #3CB371
pot --> sensor : Adjusts parameter

rectangle "Button" as btn #3CB371
btn --> sensor : User input

rectangle "BLE Data" as ble #4682B4
sensor --> ble : Sends data via BLE

rectangle "UART" as uart #4682B4
sensor --> uart : Sends data via UART

rectangle "Display" as display #4682B4
sensor --> display : Displays values

rectangle "LED" as led #4682B4
sensor --> led : Indicates status

@enduml
```