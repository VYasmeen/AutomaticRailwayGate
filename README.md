🚆 Automatic Railway Gate System (Arduino Based)

An Arduino-based automation project that controls railway gates using ultrasonic sensors and servo motors. The system detects an approaching train and automatically opens or closes the railway gate, reducing manual intervention and improving safety.

📌 Overview

This project implements an automatic railway gate controller using:

Two ultrasonic sensors for train detection

Servo motors for gate movement

Arduino microcontroller for decision logic

When a train is detected within a certain distance threshold, the gate automatically toggles between open and closed states.

⚙️ Features

🚂 Train detection using dual ultrasonic sensors

🚧 Automated gate opening and closing

🔁 Toggle-based gate logic

💡 LED indicator for gate activity

⚡ Real-time embedded control system

How It Works?

Two ultrasonic sensors monitor distances on both sides of the track.

If an object (train) is detected within ~7 cm:

Arduino triggers gate movement.

Servo motors rotate:

One closes the entry gate

One closes the exit gate

LED indicator turns on during gate motion.

🛠️ Hardware Used

Arduino board (Uno or compatible)

2 × Ultrasonic Sensors (HC-SR04)

2 × Servo Motors

LED indicator

Jumper wires and breadboard

🔌 Pin Configuration
Component	Arduino Pin
Ultrasonic Sensor 1 Trigger	Pin 3
Ultrasonic Sensor 1 Echo	Pin 2
Ultrasonic Sensor 2 Trigger	Pin 6
Ultrasonic Sensor 2 Echo	Pin 7
Servo Motor 1	Pin 9
Servo Motor 2	Pin 8
LED Indicator	Pin 13
🧾 Code Highlights

Uses pulseIn() to calculate distance from ultrasonic sensors

Distance formula:

distance = (duration / 2) / 29.1

Servo angles:

Open gate → ~55°

Closed gate → ~135–144°

Boolean flag gateOpen prevents repeated triggers


This project demonstrates:

Embedded systems fundamentals

Sensor-based automation

Real-time hardware control

Arduino programming

Physical computing concepts

🚀 Future Enhancements

IoT monitoring using WiFi module (ESP8266)

GSM alerts for nearby vehicles

LCD display for gate status

Railway traffic analytics dashboard

📄 License

This project is built for educational and demonstration purposes.
