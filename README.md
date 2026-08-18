# 🚗 IoT-Based Driver Fatigue Detection System

An **IoT-based Driver Fatigue Detection System** designed to monitor driver behavior and detect potential signs of drowsiness in real time. The system uses an **ESP32, accelerometer, IR sensors, vibration motor, and buzzer** to identify abnormal head movements or resting posture and immediately alert the driver.

The main objective is to improve road safety by providing an affordable and real-time solution for detecting driver fatigue.

---

## 📌 Table of Contents

* [Overview](#-overview)
* [Objective](#-objective)
* [Abstract](#-abstract)
* [Key Features](#-key-features)
* [System Architecture](#-system-architecture)
* [Hardware Requirements](#-hardware-requirements)
* [Working Principle](#-working-principle)
* [Results](#-results)
* [Advantages](#-advantages)
* [Applications](#-applications)
* [Future Enhancements](#-future-enhancements)
* [Project Images](#-project-images)
* [Conclusion](#-conclusion)

---

## 🔍 Overview

Driver fatigue is one of the major factors contributing to road accidents. A fatigued driver may experience reduced concentration, slow reaction time, frequent head tilting, and unintended resting posture.

This project proposes a **low-cost IoT-based driver fatigue detection system** that continuously monitors the driver's physical state. When the system detects signs that may indicate fatigue, it activates a **vibration motor and buzzer** to immediately alert the driver.

The system is designed to operate in **real time** and can be implemented using affordable and easily available components.

---

## 🎯 Objective

The primary objective of this project is to develop an **IoT-Based Driver Fatigue Detection System** capable of:

* Monitoring the driver's head movement and posture.
* Detecting abnormal head tilts associated with fatigue.
* Identifying a resting head position using IR sensors.
* Processing sensor information using an ESP32.
* Providing immediate alerts through a vibration motor and buzzer.
* Improving driver awareness and road safety.
* Providing a low-cost alternative to complex fatigue-monitoring systems.

---

## 📝 Abstract

Driver fatigue is a major cause of road accidents, and detecting drowsiness before it becomes dangerous is challenging. This project presents an **IoT-based Driver Fatigue Detection System** that monitors the driver's physical state using sensors.

An **accelerometer** is used to detect head movements and tilting, while **IR sensors** help identify whether the driver's head remains in a resting position for a prolonged period. The sensor data is processed using an **ESP32 microcontroller**.

When the system identifies conditions that may indicate driver fatigue, it activates a **vibration motor and buzzer** to provide immediate multisensory feedback to the driver.

The proposed system is **low-cost, real-time, easy to implement, and suitable for applications where driver safety is a priority**.

---

## ⭐ Key Features

* 🚗 Real-time driver fatigue monitoring
* 📐 Head tilt detection using an accelerometer
* 👤 Head-position detection using IR sensors
* 🔔 Immediate buzzer alert
* 📳 Vibration-based alert mechanism
* ⚡ ESP32-based processing
* 💰 Low-cost implementation
* 🔧 Simple and easy-to-build hardware
* ⏱️ Fast response with minimal detection delay

---

## 🏗️ System Architecture

The overall system consists of sensors, a processing unit, and an alert mechanism.

### Block Diagram

<p align="center">
  <img src="https://github.com/user-attachments/assets/5009c672-3ee0-47b7-b449-4ddc53aed284"
       alt="IoT Driver Fatigue Detection System Block Diagram"
       width="700">
</p>

### System Flow

```text
Driver
   │
   ▼
┌───────────────────────┐
│  Sensors              │
│                       │
│  • Accelerometer      │
│  • IR Sensors         │
└───────────┬───────────┘
            │
            ▼
┌───────────────────────┐
│       ESP32           │
│  Sensor Data Analysis │
└───────────┬───────────┘
            │
            ▼
    Fatigue Detected?
       /          \
     NO            YES
     │              │
     ▼              ▼
 Continue      Alert System
 Monitoring    ┌─────────────┐
               │ Buzzer      │
               │ Vibration   │
               │ Motor       │
               └─────────────┘
```

---

## 🔧 Hardware Requirements

| Component            | Purpose                                  |
| -------------------- | ---------------------------------------- |
| **ESP32**            | Main microcontroller and processing unit |
| **Accelerometer**    | Detects head movement and head tilting   |
| **IR Sensor**        | Detects driver's head/resting position   |
| **Vibration Motor**  | Provides tactile alert to the driver     |
| **Buzzer**           | Provides audible warning                 |
| **Power Supply**     | Powers the complete system               |
| **Connecting Wires** | Hardware connections                     |
| **Breadboard**       | Prototype assembly                       |

---

## 💻 Software Requirements

* Arduino IDE
* Embedded C / Arduino Programming
* ESP32 Board Package
* Required sensor libraries
* Serial Monitor for debugging and testing

---

## ⚙️ Working Principle

### 1. Sensor Monitoring

The system continuously monitors the driver's physical condition using the accelerometer and IR sensors.

### 2. Head Movement Detection

The accelerometer detects changes in the driver's head orientation. Significant or prolonged head tilting can indicate a possible fatigue condition.

### 3. Head Position Detection

IR sensors are used to identify whether the driver's head has moved into a resting position.

### 4. Data Processing

The ESP32 receives the sensor readings and evaluates them according to the predefined fatigue-detection conditions.

### 5. Fatigue Detection

If the detected sensor conditions indicate potential drowsiness, the ESP32 activates the alert mechanism.

### 6. Driver Alert

The system activates:

* 🔊 **Buzzer** — audible warning
* 📳 **Vibration Motor** — physical/tactile warning

This provides the driver with immediate feedback and encourages them to regain attention.

---

## 📊 Results

The developed prototype was tested under typical operating conditions.

The following observations were obtained:

* The **accelerometer successfully detected head tilting movements**.
* The **IR sensors detected the driver's head/resting position**.
* The **vibration motor responded effectively** when fatigue conditions were detected.
* The **buzzer provided an immediate audible warning**.
* The system operated in **real time with no significant delay** during testing.
* Multisensory feedback improved the effectiveness of the warning mechanism.

### Prototype Testing

<p align="center">
  <img src="https://github.com/user-attachments/assets/d74d4543-9610-4f53-afc4-06177284099d"
       alt="Driver Fatigue Detection Prototype"
       width="850">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/5ad30169-501b-4cf3-ae64-59631698875c"
       alt="Driver Fatigue Detection Testing"
       width="600">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/3510c916-5bde-4045-92a8-d9f2e3a2b32d"
       alt="Driver Fatigue Detection Hardware"
       width="650">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/ae01cf61-86cf-496e-990f-853a1121132c"
       alt="Driver Fatigue Detection System"
       width="650">
</p>

---

## ✅ Advantages

### 💰 Low Cost

The system uses affordable components such as an ESP32, IR sensors, accelerometer, buzzer, and vibration motor.

### ⚡ Real-Time Alerts

The system continuously monitors the driver and provides an alert immediately when potential fatigue conditions are detected.

### 🔧 Easy to Build

The prototype uses commonly available electronic components and can be implemented without complex hardware.

### 🛡️ Improved Safety

Early warning can help the driver recognize possible fatigue and take appropriate action.

### 📳 Multisensory Feedback

Combining audible and vibration alerts provides multiple forms of feedback to the driver.

---

## 🚘 Applications

The system can potentially be used in:

* 🚛 Commercial trucks
* 🚌 Public transportation
* 🚗 Passenger vehicles
* 🚕 Taxi and cab services
* 🚚 Logistics and delivery vehicles
* 🏭 Industrial vehicle operations
* 🛣️ Long-distance transportation

---

## 🚀 Future Enhancements

The current prototype can be extended with additional intelligent features:

* 🧠 **AI/ML-based fatigue classification**
* 👁️ **Camera-based eye-blink detection**
* 😴 **Yawning detection**
* 📱 **Mobile application integration**
* ☁️ **Cloud-based driver monitoring**
* 📍 **GPS-based vehicle tracking**
* 📊 **Driver fatigue history and analytics**
* 🚨 **Emergency notification system**
* 📡 **IoT dashboard for remote monitoring**
* 🔋 **Low-power operation for long-term deployment**

---

## 📷 Project Images

### Hardware Prototype

<p align="center">
  <img src="https://github.com/user-attachments/assets/d74d4543-9610-4f53-afc4-06177284099d"
       width="850"
       alt="Hardware Prototype">
</p>

### Sensor Testing

<p align="center">
  <img src="https://github.com/user-attachments/assets/5ad30169-501b-4cf3-ae64-59631698875c"
       width="600"
       alt="Sensor Testing">
</p>

### System Demonstration

<p align="center">
  <img src="https://github.com/user-attachments/assets/3510c916-5bde-4045-92a8-d9f2e3a2b32d"
       width="650"
       alt="System Demonstration">
</p>

<p align="center">
  <img src="https://github.com/user-attachments/assets/ae01cf61-86cf-496e-990f-853a1121132c"
       width="650"
       alt="Final System">
</p>

---

## 🧪 Testing

The prototype was evaluated by simulating different driver head positions and movements.

| Test Condition            | Expected Response        | Observed Response               |
| ------------------------- | ------------------------ | ------------------------------- |
| Normal head position      | No alert                 | ✅ No alert                      |
| Head tilting              | Detect abnormal movement | ✅ Detected                      |
| Resting head position     | Fatigue warning          | ✅ Alert triggered               |
| Fatigue condition         | Buzzer + vibration       | ✅ Both activated                |
| Normal condition restored | Stop alert               | ✅ System returned to monitoring |

---

## 🔮 Conclusion

The **IoT-Based Driver Fatigue Detection System** provides a simple and affordable approach for detecting potential driver fatigue in real time.

By combining an **ESP32, accelerometer, IR sensors, vibration motor, and buzzer**, the system can monitor driver movements and provide immediate warnings when fatigue-related conditions are detected.

The prototype successfully demonstrated real-time detection and multisensory alert generation. With future integration of **AI/ML, computer vision, cloud connectivity, GPS, and mobile applications**, the system can be further developed into a more advanced intelligent driver-monitoring platform.

---

## 👨‍💻 Project Information

**Project:** IoT-Based Driver Fatigue Detection System
**Domain:** IoT / Embedded Systems / Automotive Safety
**Controller:** ESP32
**Detection:** Accelerometer + IR Sensors
**Alert:** Buzzer + Vibration Motor

---

## ⭐ Support

If you find this project useful, consider giving the repository a ⭐ **Star**!

<p align="center">
  <b>🚗 Drive Safe • Stay Alert • Save Lives 🚗</b>
</p>
