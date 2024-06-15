# Smart Home Project

<p align="center">
  <img src="https://github.com/mariamAboujenane/SmartHome/assets/106840796/6b4432f8-2cbd-4871-be25-1b80338a5b00" >
</p>

## Introduction

Welcome to the Smart Home project, an innovative system designed to control and monitor various aspects of a home using Arduino microcontrollers. This project integrates multiple sensors, actuators, and communication modules to create a smart and secure home environment.

## Project Overview

The Smart Home project aims to provide a secure and convenient way to control and monitor a home environment. By leveraging the Arduino platform, we have developed a prototype that includes functionalities such as temperature and humidity monitoring, motion detection, gas leakage detection, remote control of lighting, and access control.

## Hardware Components

### Microcontrollers

#### Arduino Uno
- **Description**: Compact and versatile microcontroller with ATmega328P processor.
- **Features**: 14 digital I/O pins, 6 analog inputs, 32 KB flash memory.
- **Usage**: Suitable for connecting various sensors and actuators.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/6eb8f8a1-35d2-4a0e-bb80-084047d81a01)

#### Arduino Mega
- **Description**: Powerful microcontroller with ATmega2560 processor.
- **Features**: 54 digital I/O pins, 16 analog inputs, 256 KB flash memory.
- **Usage**: Ideal for handling more complex tasks and connecting multiple peripherals.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/b3e0c88c-fd49-406e-ac74-a32b22fd0fc1)

### Sensors

#### DHT11 (Temperature and Humidity)
- **Description**: Measures temperature and humidity.
- **Integration**: Displays data on an LCD screen and triggers actions based on predefined conditions.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/b677bd72-c8a4-4266-9442-9d96b99c9fa6)

#### PIR HC-SR501 (Motion Detection)
- **Description**: Detects motion using infrared radiation.
- **Integration**: Triggers lights or alarms when motion is detected.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/ac053f37-4de0-4af4-92d2-53a9a087e127)

#### MQ-135 (Gas Detection)
- **Description**: Detects harmful gases like CO, NH3, and benzene.
- **Integration**: Activates a buzzer to alert occupants of gas leaks.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/46766469-bfe4-4733-8388-d1182c3982a4)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/a12d2df9-63ff-4887-af93-77edd8051357)

#### 1838 IR Receiver
- **Description**: Receives infrared signals from a remote control.
- **Integration**: Allows remote control of an RGB LED.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/dac0a4be-454e-4135-a7a1-51b0b1920747)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/a2b140e5-d077-4b5b-ae6e-9299b7751166)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/550c4143-d663-4088-8664-362b6adbed63)

#### LDR (Light Dependent Resistor)
- **Description**: Detects ambient light levels.
- **Integration**: Automatically controls garden lighting based on light conditions.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/e3bbee1d-2e84-423f-8fe5-c009c39964ee)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/56aea067-6df7-44a0-a69e-5180b4fa15f4)

### Actuators

#### Stepper Motor (Curtain Control)
- **Description**: Precisely controls the position of curtains.
- **Integration**: Controlled by Arduino to open and close curtains.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/4383dade-24fc-4dfa-86b9-083376b48c60)

#### 8x8 LED Matrix
- **Description**: Displays visual information based on sensor input.
- **Integration**: Shows alerts and messages when motion is detected.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/e67a9169-3ea2-4460-9ba6-86304a929369)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/0b203760-b181-49f1-969a-d538c4e5223d)

#### 16x2 LCD Display
- **Description**: Displays temperature, humidity, date, and time.
- **Integration**: Provides a user interface for real-time monitoring.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/d0b1f58e-2b99-421c-8bf4-189e6e34be9a)

### Communication Modules

#### RFID RC522
- **Description**: Enables secure access control using RFID tags.
- **Integration**: Controls door locks and logs entry events.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/33d28252-7f18-469b-84bf-f8112a0edae3)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/a11d6dbb-5bb9-4493-af7e-1ff6a70b0902)

#### Bluetooth HC-05
- **Description**: Allows wireless communication with smartphones.
- **Integration**: Used for controlling lights and other devices via a mobile app.
  
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/0a216f96-4cdd-46be-aef1-6b2725925e56)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/3ff0e711-7b03-44ae-9ab3-7e4ac06a707b)

## Software

### Arduino IDE
- **Description**: Integrated development environment for programming Arduino boards.
- **Usage**: Write, compile, and upload code to the microcontrollers.

### Libraries
- **DHT Sensor Library**: For reading temperature and humidity data.
- **IRremote Library**: For decoding infrared signals.
- **Stepper Library**: For controlling the stepper motor.
- **LiquidCrystal Library**: For interfacing with the LCD display.
- **MFRC522 Library**: For handling RFID communication.
- **SoftwareSerial Library**: For serial communication with the Bluetooth module.

## System Architecture

The smart home system is built on a modular architecture where different sensors and actuators are connected to the Arduino microcontrollers. The microcontrollers process sensor data and trigger appropriate actions. Communication between components is handled through various interfaces, including I2C, SPI, and UART.

## Setup and Installation

### Hardware Setup
1. **Connect Sensors**: Wire each sensor to the appropriate pins on the Arduino boards.
2. **Connect Actuators**: Attach actuators such as the stepper motor and LED matrix to the Arduino boards.
3. **Power Supply**: Ensure a stable power supply to all components, either via USB or external power sources.

### Software Installation
1. **Install Arduino IDE**: Download and install the Arduino IDE from the official website.
2. **Install Libraries**: Add necessary libraries through the Library Manager in the Arduino IDE.
3. **Upload Code**: Write or upload the provided code to the Arduino boards.

## Usage

### Controlling the System
- **Temperature and Humidity Monitoring**: View real-time data on the LCD display and receive alerts for predefined conditions.
- **Motion Detection**: Automatically turn on lights or trigger alarms when motion is detected.
- **Gas Detection**: Receive audible alerts in case of gas leaks.
- **Remote Control**: Use a smartphone app to control lights and other devices via Bluetooth.
- **Access Control**: Use RFID tags or a keypad to unlock doors.

### Maintenance
- **Regular Checks**: Periodically check sensor readings and actuator functions to ensure proper operation.
- **Firmware Updates**: Update the microcontroller firmware as needed to add new features or fix bugs.

## Real Time realisation
### Conception 3D

![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/be3cfb1c-947e-4734-bedf-1fb6f156e47f)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/e33431c8-a647-49c4-b80c-1240cac4665d)

### Realisation

![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/91e683a2-4fab-4e2e-97ef-088d66eac5ad)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/7b0998c4-4468-476d-8618-b235e0dd0357)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/bc509b5a-0242-4840-b056-d4e244cfc177)

![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/2228f849-0dbd-4492-87e0-380658ed9a1d)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/6d4418b2-f0e3-4582-b643-9e5323d17ba3)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/8169d3bd-4dad-4b8f-b006-02004f37ade9)
![image](https://github.com/mariamAboujenane/SmartHome/assets/106840796/e368d0b2-eb07-4720-96a3-e62490558ada)

## Conclusion

The Smart Home project demonstrates the potential of integrating various sensors, actuators, and communication modules to create a secure and convenient home environment. By leveraging Arduino microcontrollers, we have developed a scalable and customizable system that can be easily expanded to include additional functionalities. This project serves as a foundation for future advancements in home automation and smart living.
