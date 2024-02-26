# IoT-Based Pet Care System

## Abstract

Pet care and welfare are significant issues that receive attention and funding. This paper presents an IoT-based solution for pet owners, addressing challenges such as maintaining a pet's schedule and providing care when the owner is away. The proposed system monitors and controls food, water, and temperature through sensors connected to an Arduino board, acting as an onboard computer. A Graphical User Interface (GUI) allows pet owners to access and manage these parameters remotely.

## Introduction

Pets have become integral parts of human life, requiring consistent care. However, busy schedules may lead to under-care situations. The paper introduces an IoT-based pet care system, utilizing sensors to monitor food, water, and temperature. An ESP8266 board serves as the central controller, and a GUI enables remote monitoring and control by pet owners.

## System Architecture

The system employs temperature, IR, and ultrasonic sensors to measure temperature, food level, and water level, respectively. The ESP8266 Wi-Fi module acts as the central controller, connected to a web server. A GUI allows pet owners to monitor and control the parameters. The architecture ensures real-time updates and notifications.

## Hardware Design

### Temperature Sensing

- Si7021 sensor is used for temperature and humidity.
- Interfaced with ESP8266 via I2C.
- ESP8266 sends notifications based on temperature readings.
- Heating or cooling devices activated to maintain the ideal temperature range.

### Food Level Detection

- IR sensor detects food level.
- ESP8266 receives sensor values.
- Notifications sent to the web server when food is below a threshold.
- Automated commands to refill food as needed.

### Water Level Detection

- Ultrasonic sensor measures distance to detect water level.
- ESP8266 processes sensor values.
- Notifications sent based on water level conditions.
- Refill commands triggered when water is below the required level.

## Software Design

- Arduino IDE used for software development.
- ESP8266 programmed to broadcast sensor values to the web server.
- GUI provides real-time monitoring and control.
- Notifications alert pet owners about temperature, food, and water conditions.

## Simulation and Results

- Circuit diagram and hardware interface designed.
- Web server displays real-time data and notifications.
- Notifications include temperature alerts and food/water level indications.
- Simulation ensures proper functioning of the IoT-based pet care system.

## Future Scope

- Addition of a second onboard computer (Arduino Uno) for extended functionalities.
- Integration of GPS and GSM modules to track pet location and send notifications.
- Connection to motors for automated food and water dispensing.
- Cloud integration for remote server access and enhanced security.

## Challenges Faced

- Calibration challenges with Si7021 sensor.
- Serial communication issues between Arduino and ESP8266 for GPS module.
- Overcoming noise and errors during sensor configuration.

## Conclusion

The IoT-based pet care system provides a comprehensive solution for pet owners to monitor and care for their pets remotely. The integration of sensors, controllers, and a user-friendly GUI ensures effective management of temperature, food, and water. The future scope suggests further enhancements for advanced functionalities.
