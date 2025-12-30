---
title: "IoT Health Monitoring System (PCB-Based)"
excerpt: "PCB-based IoT device for real-time monitoring of heart rate, SpO₂, and body temperature"
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
This project focuses on the **design and implementation of a PCB-based IoT health monitoring system**
capable of continuously measuring **heart rate, blood oxygen saturation (SpO₂), and body temperature**
in real time.

The system integrates biomedical sensors, power management circuitry, and a microcontroller
to create a **compact, low-power, and portable healthcare device** suitable for remote and
personalized health monitoring.

---

## 🎯 Motivation
Continuous health monitoring is critical for early detection of medical conditions and
remote patient care. Conventional systems are often bulky or expensive.
This project demonstrates a **cost-effective, PCB-integrated IoT solution**
that enables real-time physiological data acquisition and transmission.

---

## 🏗 System Architecture
![System Architecture](/images/iot_health_architecture.png)

The system consists of the following blocks:
1. Biomedical sensors for physiological data acquisition  
2. ATmega328P microcontroller for data processing  
3. Power management unit (battery, charger, buck-boost converter)  
4. Serial/IoT interface for data transmission  

---

## 🔧 Hardware Implementation

### Microcontroller
- **ATmega328P**
- Handles real-time sensor data acquisition and processing
- Optimized for low-power operation

### Sensors
- **MAX30102** – Pulse oximeter and heart-rate sensor  
- **MAX30205** – Clinical-grade digital temperature sensor  

These sensors provide accurate, non-invasive physiological measurements.

### Power Management
- **TP4056** Li-ion battery charging module  
- **TPS63020** buck-boost DC-DC converter  
- Single-cell Li-ion battery (3.6V)

This three-stage power system ensures **stable voltage output** and efficient energy usage
across varying load conditions.

---

## 💻 Software & Firmware
- Embedded C firmware for ATmega328P
- Sensor interfacing via **I2C**
- Serial communication for data output
- Bootloader-based firmware upload using **FT232RL USB-to-Serial**

The firmware supports reliable sensor polling, data formatting, and transmission.

---

## 🖨 PCB Design & Fabrication
![PCB Layout](/images/iot_health_pcb.png)

- Schematics and PCB layout designed using **KiCad**
- Component footprints verified using manufacturer datasheets
- Gerber files generated and sent to PCB fabrication vendor
- Final PCB tested for continuity, signal integrity, and functionality

---

## 🧪 Testing & Validation
- Functional testing of all sensors
- Power stability verification under varying load conditions
- Signal validation using multimeters and oscilloscopes
- End-to-end system testing on fabricated PCB

The device demonstrated reliable operation in both simulated and real-world scenarios.

---

## ✅ Results
- Accurate real-time measurement of heart rate, SpO₂, and temperature
- Stable voltage regulation using buck-boost topology
- Compact and portable PCB-based implementation
- Suitable for continuous health monitoring applications

---

## 🌍 Applications
- Remote patient monitoring
- Wearable healthcare devices
- IoT-based medical diagnostics
- Preventive healthcare systems

---

## 🚀 Future Improvements
- Wireless connectivity (Bluetooth / Wi-Fi)
- Cloud integration (AWS IoT, Google Cloud IoT)
- Data logging and trend analysis
- Custom wearable enclosure
- Further power optimization using sleep modes

---

## 👥 Team Contribution
- **Kavin K:** PCB design, power management integration, firmware development  
- **Gonela Sreeman:** Sensor integration, testing, validation, and documentation  
- Project supervised by **Dr. Rohit Singh**

---

## 🔗 Source Code & Design Files
👉 [View project repository on GitHub](https://github.com/kavin1772/iot-health-monitoring-system)
