---
title: "IoT Health Monitoring System (PCB-Based)"
excerpt: "Custom PCB-based IoT device for real-time heart rate, SpO₂, and temperature monitoring"
collection: portfolio
header:
  teaser: /images/iot_health_teaser.jpg
---

## 🎥 Demo
<video width="100%" controls muted>
  <source src="/videos/iot_health_demo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## 🧠 Overview
This project presents the **design and implementation of a PCB-based IoT health monitoring system**
capable of continuously measuring **heart rate, blood oxygen saturation (SpO₂), and body temperature**
in real time.

The system integrates biomedical sensors, embedded firmware, and a robust power management
architecture to create a **compact, portable, and low-power healthcare device** suitable for
remote and personalized health monitoring applications.

---

## 🎯 Motivation
Remote health monitoring is essential for early diagnosis and preventive healthcare.
Conventional systems are often bulky or expensive. This project demonstrates a **cost-effective,
PCB-integrated IoT solution** that enables real-time physiological data acquisition with
reliable power delivery and scalability.

---

## 🏗 System Architecture
![System Architecture Diagram](/images/iot_health_architecture.png)

**System Flow:**
1. Biomedical sensors acquire physiological data  
2. ATmega328P processes sensor data  
3. Power management unit ensures stable operation  
4. Data transmitted via serial/IoT interface  

---

## 🔧 Hardware Components

### 🧠 Microcontroller
![ATmega328P](/images/atmega328p.jpg)

- **ATmega328P**
- Low-power embedded microcontroller
- Handles sensor interfacing, processing, and communication

---

### ❤️ Sensors
![MAX30102 Pulse Oximeter](/images/max30102.jpg)
![MAX30205 Temperature Sensor](/images/max30205.jpg)

- **MAX30102** – Heart rate and SpO₂ sensor (PPG-based)
- **MAX30205** – Clinical-grade digital temperature sensor (I2C)

These sensors provide accurate, non-invasive physiological measurements.

---

### 🔋 Power Management
![TP4056 Charger](/images/tp4056.jpg)
![TPS63020 Buck-Boost Converter](/images/tps63020.jpg)

- **TP4056** Li-ion battery charging module
- **TPS63020** automatic buck-boost DC-DC converter
- Single-cell Li-ion battery (3.6V)

Ensures **stable voltage output** and efficient energy usage across varying load conditions.

---

### 🔌 Programming & Communication
![FT232RL USB to Serial](/images/ft232rl.jpg)

- **FT232RL USB-to-Serial** interface
- Used for bootloading, debugging, and firmware updates

---

## 🖨 Schematic Design
![Schematic Design](/images/iot_health_schematic.png)

The schematic was designed using **KiCad**, following manufacturer datasheets for:
- Decoupling capacitors
- Clock circuitry (8 MHz crystal)
- I2C sensor connections
- Power regulation and battery charging

---

## 🧩 PCB Layout

### PCB Layout (With Connections)
![PCB Layout With Connections](/images/iot_health_pcb_connections.png)

### PCB Layout (Without Connections)
![PCB Layout Without Connections](/images/iot_health_pcb_no_connections.png)

- Multi-module PCB designed in **KiCad**
- Gerber files generated and sent to fabrication vendor
- Layout optimized for signal integrity and power stability

---

## 🛠 Fabricated PCB & Prototype
![Final Assembled PCB](/images/iot_health_final_board.jpg)

The final fabricated PCB integrates:
- Power management modules
- Biomedical sensors
- OLED display
- ATmega328P microcontroller

The prototype was tested for continuity, voltage stability, and end-to-end functionality.

---

## 💻 Firmware & Software
- Embedded C firmware for ATmega328P
- Sensor communication via **I2C**
- Serial data transmission for monitoring
- Bootloader-based firmware upload

---

## 🧪 Testing & Validation
- Functional testing of all sensors
- Power stability verification under varying load
- Signal validation using multimeters and oscilloscopes
- End-to-end testing on fabricated PCB

---

## ✅ Results
- Accurate real-time heart rate, SpO₂, and temperature readings
- Stable voltage regulation using buck-boost topology
- Compact, portable PCB-based design
- Reliable operation in real-world testing

---

## 🌍 Applications
- Remote patient monitoring
- Wearable healthcare devices
- IoT-based medical diagnostics
- Preventive healthcare systems

---

## 🚀 Future Improvements
- Wireless connectivity (Bluetooth / Wi-Fi)
- Cloud integration (AWS IoT / Google Cloud IoT)
- Data logging and trend analysis
- Custom wearable enclosure
- Further power optimization using sleep modes

---

## 👥 Team Contribution
- **Kavin K:** PCB design, power management integration, firmware development  
- **Gonela Sreeman:** Sensor integration, testing, validation, documentation  
- Supervised by **Dr. Rohit Singh**

---

## 🔗 Source Code & Design Files
👉 [View project repository on GitHub](https://github.com/kavin1772/iot-health-monitoring-system)
