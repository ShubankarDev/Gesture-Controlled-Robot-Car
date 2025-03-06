# Gesture-Controlled-Robot-Car
This repository contains Tinkercad simulation of hardware circuit and arduino ide and open cv code for Gesture controlled robot car 

## Project Overview
This project involves designing and implementing a **gesture-controlled robot car** using **OpenCV, Processing IDE, Proteus, and Arduino**. The robot is controlled based on hand gestures, which are recognized using a camera and processed using **MediaPipe Hand Tracking** in Processing. The recognized gestures are then transmitted to an Arduino board via a serial communication interface, which in turn drives the motors to control the movement of the car.

## Key Features
- **Real-time Gesture Recognition**: Uses OpenCV and MediaPipe for tracking hand movements.
- **Serial Communication**: Sends detected gestures as movement commands to Arduino.
- **Motor Control**: Uses an H-Bridge motor driver to drive the motors based on received commands.
- **Simulation Support**: The system is designed for both hardware implementation and simulation in Proteus.
- **Alternative TinkerCAD Simulation**: Since the specific motor driver was not available in TinkerCAD, **transistors and resistors** were used to drive the motors instead.

## Components Used
### Hardware Components
- **Arduino Nano ESP32** (for processing and motor control)
- **TB6612FNG Motor Driver** (to control the motors)
- **DC Motors** (to drive the robot)
- **Battery Pack** (to power the motors and Arduino)
- **Camera** (for gesture recognition)

### Software & Tools
- **Processing IDE** (for gesture recognition and serial communication)
- **OpenCV & MediaPipe** (for hand tracking)
- **Proteus Design Suite** (for circuit simulation)
- **Virtual Serial Port Emulator (VSPE)** (for serial communication testing)
- **Arduino IDE** (for motor control programming)

## Working Principle
1. The camera captures real-time hand gestures.
2. Processing IDE uses OpenCV & MediaPipe to detect and classify the gestures.
3. The detected gestures are converted into specific movement commands (e.g., Forward, Backward, Left, Right, Stop).
4. The command is transmitted to the Arduino via serial communication.
5. The Arduino processes the command and activates the appropriate motor driver pins.
6. The motor driver controls the motors, moving the robot in the desired direction.

## Gesture Control Mapping
- **Forward** → Two fingers up
- **Backward** → Two fingers down
- **Left** → Index finger pointing left
- **Right** → Index finger pointing right
- **Stop** → No valid gesture detected

## Simulation & Implementation
- **Proteus Simulation**: Used to verify the circuit before physical implementation.
- **TinkerCAD Simulation**: Used an alternative setup with transistors and resistors to drive the motors instead of a dedicated motor driver.
- **Real-World Implementation**: Uses Arduino, a motor driver, and real motors for practical application.

## Future Enhancements
- Implementing **Bluetooth/WiFi control** for wireless operation.
- Enhancing gesture recognition accuracy using **Machine Learning models**.
- Adding obstacle avoidance using **ultrasonic sensors**.

This project successfully demonstrates a **gesture-controlled robotic car** using computer vision and microcontroller-based motor control.
