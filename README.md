# advanced-medication-system



```markdown
# 🚗💊 Smart Medicine Dispenser Robo Car

A smart healthcare and robotics prototype that combines autonomous movement, pulse validation, real-time cloud monitoring, and scheduled medicine dispensing. Built using Arduino Uno, ESP32, Firebase, and ThingSpeak, this system ensures timely and safe delivery of medication with cloud-based updates and notifications.

---

## 🔧 Features (Implemented)

### 🤖 Autonomous Obstacle Avoidance  
- Robo car uses an **ultrasonic sensor** mounted on a **servo motor** to detect obstacles.
- It scans left and right to find a clear path and move accordingly.

### ⏰ Scheduled Pill Dispensing  
- ESP32 retrieves **scheduled time and dose count** from **Firebase Realtime Database**.
- Based on time, one of the **four servo-controlled compartments** (morning, afternoon, evening, night) dispenses the pill.

### ❤️ Pulse Check Before Dispensing  
- **MAX30102 pulse sensor** checks the user's pulse.
- Dispensing occurs only if pulse is detected, ensuring basic health validation.

### 📧 Email Notification & Cloud Logging  
- Sends an **email alert** to the registered patient after each successful pill dispense.
- Logs the event on a **custom dashboard** using **Firebase** and **ThingSpeak**, viewable in real-time.

### 📊 Dashboard Integration (Completed)  
- A **web dashboard** displays real-time logs of pill dispensing and patient data.
- Built using Firebase and ThingSpeak for easy access and monitoring by caregivers.

### 🔄 Modular Microcontroller Integration  
- **Arduino Uno**: Controls DC motors, ultrasonic sensor, and obstacle avoidance.
- **ESP32**: Handles Firebase sync, real-time clock, pulse monitoring, email notifications, and servo control.

---

## 🧪 Work in Progress / Planned Features

- **🧠 Facial Recognition (ESP32-CAM)**  
  Detect and verify the correct patient before dispensing using face detection.

- **⚖️ Load Sensor Integration**  
  Use a load cell to confirm whether the pill has actually been dispensed.

- **💧 Liquid Medicine Dispenser**  
  Add-on to support dispensing of liquid medicines alongside pills.

---

## 📦 Hardware Used

- Arduino Uno  
- ESP32  
- ESP32-CAM *(planned)*  
- MAX30102 Pulse Sensor  
- Ultrasonic Sensor + SG90 Servo Motor  
- SG90 Servo Motors   
- L298S Motor Driver  
- DC Motors (×4)  
- Firebase Realtime Database  
- ThingSpeak IoT Cloud  
- NTPClient (for IST time synchronization)  
- Load Sensor *(planned)*  
- Buzzer, LEDs, Chassis, Wires, Battery Pack

---

## 🌐 Cloud Integration

- **Firebase Realtime Database** for storing schedule, dispensing logs, and email IDs.
- **ThingSpeak** for IoT data visualization and dashboard metrics.
- **NTPClient** for accurate real-time scheduling in IST.

---

## 📸 Project Status

✅ Pill compartments  
✅ Time-based dispensing  
✅ Pulse sensor validation  
✅ Firebase & ThingSpeak dashboard  
✅ Email alerts  
🔜 Facial recognition  
🔜 Load sensor confirmation  
🔜 Liquid dispenser

---

## 💡 Author

Smart Healthcare Project by my team mates Bhoomika DH , Madhumitha P, Pruthvi S and Vaishnavi R Katti  
Inspired by real-world IoT healthcare applications  
*For academic and prototyping use only.*

---
