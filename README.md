# Finger Fource Measurement Device 

This project aims to develop a strength measurement device that will be capable of measuring applied force and transmitting data wirelessly to a mobile application via Bluetooth Low Energy (BLE). The device is planned to handle forces up to 100 kg, making it suitable for various strength-based applications. The following sections outline the planned features, components, and usage scenarios for this prototype.

## Planned Features

- **Force Measurement**: The device will be designed to measure applied force using a high-precision load cell (strain gauge) with a target capacity of at least 100 kg.
- **Wireless Communication**: It is intended that the device will transmit data wirelessly via BLE to a mobile app for real-time monitoring.
- **Rechargeable Battery**: The prototype is expected to include a rechargeable lithium-polymer battery for portable use and easy recharging.
- **Compact and Durable Design**: The device will be designed to be small, lightweight, and durable to ensure usability in a variety of environments.

## Planned Components

1. **Microcontroller**: The Nordic Semiconductor nRF52840 is planned to be used for handling BLE communication and device control.
2. **Force Sensor**: A strain gauge capable of measuring forces up to 100 kg is intended to be integrated for accurate force measurements.
3. **Battery**: The prototype will feature a rechargeable lithium-polymer battery.
4. **Charging Port**: The device will be equipped with a USB-C port for convenient charging.
5. **PCB**: A custom-designed PCB will be developed to integrate the necessary components.
6. **Enclosure**: A 3D-printed or custom-built case is planned to house the components and ensure durability.

## Planned Usage

The device is intended for applications that require accurate force measurement, such as grip strength testing, fitness tracking, or physical therapy. A mobile app is planned to allow users to track their progress and view force data in real-time.

### Potential Use Cases

- **Athlete Training**: The device is expected to help monitor grip strength or other exercises requiring strength measurement up to 100 kg.
- **Physical Therapy**: It will allow for tracking patient recovery progress through force measurements.
- **Research**: The device may be used for collecting and analyzing force data in various activities.

## First Version Goal

In the first version of the project, the primary goal is to receive data from the strain gauge sensor and send it via BLE to a computer using a development board.

## License

This project is open-source and will be distributed under the MIT License. See the `LICENSE` file for further details once the project is in its implementation phase.

## Contributing

Contributions will be welcomed during the development process! Feel free to suggest ideas, report issues, or submit pull requests as the prototype takes shape.
