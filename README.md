# Balancing Robot MPU6050

## Overview
A self-balancing platform prototype using an MPU6050 gyroscope/accelerometer and a servo motor. It uses a PID controller to keep the platform level by counteracting tilt.

## Features
- Reads roll angle from MPU6050
- PID control (Proportional, Integral, Derivative)
- Real-time serial monitoring
- Smooth servo response

## Components
- Arduino Uno
- MPU6050 Gyroscope/Accelerometer
- Servo Motor
- Wires

## Circuit Connections
| Component | Pin |
|-----------|-----|
| MPU6050 SDA | A4 |
| MPU6050 SCL | A5 |
| MPU6050 VCC | 5V |
| MPU6050 GND | GND |
| Servo Signal | 9 |
| Servo VCC | 5V |
| Servo GND | GND |

## How It Works
- The MPU6050 measures the tilt angle (roll).
- The error is calculated as the difference between the target angle (0°) and the actual roll.
- PID computes the corrective output.
- The servo moves opposite to the tilt to stabilize the platform.

## Author
Created by [Anas | Αмizσ] — an aspiring mechatronics engineer.# Balance-system-
