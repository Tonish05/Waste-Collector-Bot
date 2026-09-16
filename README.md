# Waste-Collector-Bot
Arduino-based autonomous waste collection robot featuring a 3-DOF robotic arm, Bluetooth wireless control, ultrasonic obstacle detection, and motor control using L298N. Integrates embedded systems, robotics, servo actuation, and power management into a mobile mechatronic platform for waste handling.
# Waste Collection Robot

A small-scale robotic system developed for waste collection and object handling. The robot combines a mobile chassis, Bluetooth-controlled movement, ultrasonic sensing, and a 3-DOF robotic arm controlled using an Arduino Uno.

## Overview

The main objective of the project was to build a functional waste-collection robot while gaining practical experience in robotics, embedded systems, motor control, and hardware integration.

The robot can be remotely controlled for movement and uses a servo-based robotic arm to pick and handle objects. Ultrasonic sensing was also integrated to support obstacle detection.

## Features

* 4-wheel mobile robot platform
* Bluetooth-based wireless control
* 3-DOF robotic arm
* Servo-controlled gripper
* DC motor control using L298N
* Ultrasonic obstacle detection
* Battery management and regulated power supply
* Arduino-based control system

## Hardware

| Component         | Purpose                       |
| ----------------- | ----------------------------- |
| Arduino Uno R3    | Main controller               |
| L298N             | DC motor driver               |
| BO DC Motors      | Robot movement                |
| HC-05             | Bluetooth communication       |
| Ultrasonic Sensor | Distance / obstacle detection |
| Servo Motors      | Robotic arm and gripper       |
| Battery Pack      | Power source                  |
| BMS               | Battery protection            |
| Buck Converter    | Voltage regulation            |

## System

The Arduino Uno acts as the main controller. Commands received through the HC-05 Bluetooth module are processed by the Arduino and used to control the motors through the L298N driver.

The robotic arm is operated using servo motors and consists of shoulder, elbow, and gripper mechanisms. Ultrasonic sensing provides distance information for detecting obstacles.

### Basic Architecture

```text
        Mobile / Bluetooth
                |
              HC-05
                |
                v
          Arduino Uno
           /       \
          /         \
         v           v
      L298N       Servos
         |           |
         v           v
     DC Motors    3-DOF Arm
                       |
                    Gripper

        Ultrasonic Sensor
                |
                v
          Arduino Uno
```

## Software

* Arduino IDE
* Embedded C/C++
* Arduino Servo Library
* Serial/Bluetooth communication
* PWM-based motor control

## Working

1. The robot receives movement commands through Bluetooth.
2. Arduino processes the commands and controls the DC motors through the L298N.
3. The robotic arm is controlled using servo motors.
4. The gripper is used to pick and handle objects.
5. Ultrasonic sensing is used to detect obstacles in the robot's path.

## Power System

The robot uses a rechargeable battery pack as its primary power source. A BMS is used for battery protection, while a buck converter is used to provide regulated voltage for the electronics and servo system.

## Project Development

This project involved working across both hardware and software:

* Mechanical assembly of the mobile chassis
* Motor driver and motor wiring
* Arduino programming
* Bluetooth communication
* Servo and robotic-arm control
* Ultrasonic sensor integration
* Power distribution and voltage regulation
* Testing and troubleshooting of the complete system

## Future Improvements

The current system is a manually controlled prototype. Possible extensions include:

* Autonomous navigation
* Improved obstacle avoidance
* Camera-based waste detection
* Object classification
* Automatic waste segregation
* Automated pick-and-place
* ROS2 integration
* Computer vision and AI

## Technologies

**Arduino Uno · Embedded C/C++ · L298N · HC-05 Bluetooth · Ultrasonic Sensors · Servo Motors · DC Motors · BMS · Buck Converter · Robotics · Mechatronics**

## Project Status

**Completed prototype**

The project was developed as a hands-on robotics project to understand the integration of mechanical, electrical, and embedded systems.
