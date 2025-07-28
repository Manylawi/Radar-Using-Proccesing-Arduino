# 📡 Arduino Radar System with GUI (Ultrasonic + Servo + Processing)

This project presents a **radar simulation system** built using an **ultrasonic sensor** (HC-SR04), a **servo motor**, and an **Arduino Uno**, with real-time **graphical visualization** developed in **Processing IDE**. The system continuously scans a sector and displays detected objects and distances in a radar-like user interface.

---

## 👨‍🎓 Team Members

- Ahmed Mohamed Ahmed Fouad El-Manylawi  
- Ahmed Saeed Mohamed Imam Zayed  
- Ahmed Reda Kamel Abdelghany  
- Ahmed Mohamed Ali Mohamed  
- Aziz Emad Aziz Labib  
- Abdallah Mohamady Mohamady Hafour  
- Seif El-Din Mohamed Youssef  

**Supervisor**: Dr. Amany Mohamed  
**Faculty**: Faculty of Engineering – Helwan National University  
**Year**: 2024

---

## 📘 Project Overview

The radar system works by rotating an ultrasonic sensor horizontally via a servo motor and measuring the distance to objects in its field of view. The measured angle and distance are transmitted to a computer via serial communication, where a radar-like interface is drawn using **Processing IDE**.

---

## 🔩 Components & Functionality

| Component              | Functionality                                                                 |
|------------------------|-------------------------------------------------------------------------------|
| **Ultrasonic Sensor**  | Measures distance to objects using sound wave pulses (HC-SR04)               |
| **Servo Motor (SG90)** | Rotates sensor from 15° to 165° to scan area                                 |
| **Arduino**            | Reads sensor data, controls servo, and sends data to computer                |
| **Processing IDE**     | Graphically displays radar in real time based on sensor data                 |

---

## ⚙️ System Features

### 1. 🧮 Distance Measurement
- Ultrasonic sensor emits a pulse and waits for the echo
- Distance calculated using:  
  `distance = (duration × 0.0343) / 2`

### 2. 🔁 Servo Motor Rotation
- Sweeps sensor back and forth between **15° and 165°**
- Captures object distances at different angles

### 3. 📊 Radar Display (Processing)
- Displays radar interface using arcs and lines
- Shows angle, range lines, and object positions in real time
- Displays "Out of Range" if distance exceeds detection threshold

### 4. 📡 Real-Time Communication
- Arduino sends angle and distance over serial port in format:  
  `angle,distance`
- Processing reads this data and draws the radar frame

---

## 📐 How It Works (Step-by-Step)

1. **Setup**:  
   - `trigPin` and `echoPin` configured for HC-SR04  
   - Servo motor connected to control pin  
2. **Scan**:  
   - Servo rotates the ultrasonic sensor between 15° and 165°  
   - At each step, the ultrasonic module measures the distance  
3. **Data Transmission**:  
   - Arduino sends formatted data (e.g. `90,125`) to PC via serial  
4. **Radar Visualization**:  
   - Processing IDE reads data, maps it, and renders it as a live radar display

---

## 🖼️ User Interface (Radar GUI)

The radar interface includes:
- **Green sweeping arm**
- **Distance arcs**
- **Live object dots**
- Real-time updates showing angle and distance data

---

## 🧪 Applications & Educational Goals

- Learn sensor interfacing (ultrasonic, servo)  
- Real-time data processing with Arduino  
- Serial communication and GUI development  
- Ideal for projects in **IoT**, **robotics**, and **embedded systems**

---

## 📬 Contact

**Ahmed El-Manylawi**  
📧 ahmed.elmanylawi@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/ahmed-el-manylawi-67b6162aa)

---

> 📚 **This project is for academic and educational demonstration only. All rights reserved to the authors.**
