# Automated-Production-Line-ESP32
Automated production line model with a robotic arm controlled via ESP32, featuring a web interface, IR sensor, and conveyor belt system.
# Automated Production Line With Robotic Arm Control

## Overview
This project presents the development of a miniature automated production line model integrated with an industrial robotic arm. The system is designed to demonstrate an efficient method of transferring items on a conveyor belt to specified locations. The entire process is managed by an **ESP32 microcontroller**, with commands issued through a custom mobile web interface via WebSockets.

## 🎥 References & Acknowledgments
A special thanks to the following YouTube tutorial which provided great assistance and foundational knowledge for assembling the robotic arm and building the web interface:
* [Robot Arm using ESP32 and Smartphone | Complete Robot Arm assembly](https://youtu.be/cVSvg6VQhGU?si=p7T09PnH00FcyEWJ) (by Hash Include Electronics)

## Academic Context
* **University:** Sana'a University
* **Faculty:** Faculty of Engineering
* **Department:** Electricity Dep, Computer and Control
* **Year:** Fourth Year, First Semester (2024)
* **Author:** Mohammed Arif


## Key Features & Workflow
1. **Conveyor System:** A DC motor drives the conveyor belt, which is controlled by a 5V relay.
2. **Object Detection:** An IR sensor monitors the belt. When an object is detected, the sensor signals the relay to halt the DC motor automatically.
3. **Robotic Arm Control:** Once the belt stops, the operator uses a mobile web application to control the 4-DOF robotic arm (Base, Shoulder, Elbow, Gripper) built with SG90 servo motors to pick and place the object.
4. **Record & Playback:** The web interface features a unique "Record" and "Play" functionality, allowing the operator to record a sequence of manual arm movements and replay them automatically for repetitive tasks.

## Hardware Components
* ESP32 Microcontroller
* 4 x SG90 Servo Motors
* DC Motor (for the conveyor)
* IR Sensor
* 5V Relay Module
* Mechanical Robotic Arm Structure
* Power Supply & Breadboard

## Software & Technologies Used
* **C++ / Arduino IDE**
* **ESPAsyncWebServer & AsyncTCP:** For asynchronous HTTP requests and server hosting on the ESP32.
* **WebSockets:** For real-time, low-latency communication between the mobile app and the ESP32.
* **HTML/CSS/JS:** Custom web interface built directly into the microcontroller's code.
