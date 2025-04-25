 This project is a smart healthcare prototype that combines autonomous navigation, real-time health validation, and intelligent medicine dispensing using IoT and robotics. The system uses an Arduino Uno-powered robo car and an ESP32-based module, integrated with Firebase and ThingSpeak for cloud-based control, monitoring, and alerts.

🔧 Features (Implemented)
Autonomous Obstacle Avoidance
Uses an ultrasonic sensor mounted on a servo motor to detect obstacles and scan for a clear path before moving.

Scheduled Pill Dispensing
The ESP32 reads the dose count and time from the Firebase Realtime Database and activates one of four servo-controlled compartments (morning, afternoon, evening, night) to dispense a pill at the scheduled time.

Pulse Check Before Dispensing
A MAX30102 pulse sensor reads the user’s pulse to confirm presence and basic wellness before activating the dispenser.

Email Notification & Cloud Logging
After a successful dispense, the system sends an email to the registered person and logs the event to a custom dashboard via Firebase and ThingSpeak, enabling real-time remote monitoring.

Dashboard Integration (Completed)
A web-based dashboard shows live dispensing updates, patient data, and historical logs using Firebase and ThingSpeak cloud services.

Modular Integration

Arduino Uno: Controls motors, steering logic, and ultrasonic obstacle avoidance.

ESP32: Handles time sync (via NTPClient), cloud interaction, pulse monitoring, and servo-based pill dispensing.

🧪 Work in Progress / Planned
Facial Recognition (ESP32-CAM)
Identify and verify the correct patient before pill dispensing.

Pill Dispense Confirmation with Load Sensor
Detects if the pill has physically been dispensed using a load cell sensor.

Liquid Medicine Dispenser Add-on
Add functionality for dispensing liquid medications alongside pills.

📦 Hardware Used
Arduino Uno

ESP32 & ESP32-CAM (for future facial detection)

MAX30102 Pulse Sensor

Ultrasonic Sensor

SG90 Servo Motors (×5)

L298S Motor Driver

DC Motors (×4)

Firebase Realtime Database

ThingSpeak IoT Cloud

NTPClient (IST time sync)

Load Sensor (planned)

Buzzer, LEDs, jumper wires, chassis, battery pack
