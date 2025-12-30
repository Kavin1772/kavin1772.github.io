---
title: "IoT Health Monitoring System (PCB-Based)"
excerpt: "Custom PCB-based IoT device for real-time heart rate, SpO₂, and temperature monitoring"
collection: portfolio
header:
  teaser: /images/iot_health_teaser.png
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

## 🏗 System Architecture
![System Architecture Diagram](/images/iot_health_architecture.png)

The system consists of:
- Biomedical sensors for physiological data acquisition  
- ATmega328P microcontroller for processing  
- Power management circuitry  
- Serial/IoT interface for data transmission  

---

## 🔧 Key Hardware Components

### 🧠 Microcontroller
![ATmega328P](/images/ATmega328P.jpg)

- ATmega328P low-power microcontroller
- Handles sensor interfacing and data processing

---

### ❤️ Sensors
![MAX30102 Pulse Oximeter](/images/MAX30102%20Pulse%20Oximeter.jpg)
![MAX30205 Temperature Sensor](/images/MAX30205%20Temperature%20Sensor.jpg)

- **MAX30102** – Heart rate and SpO₂ monitoring  
- **MAX30205** – Clinical-grade digital temperature sensor  

---

### 🔋 Power Management
![TP4056 Charger](/images/TP4056%20Charger.jpg)
![TPS63020 Buck-Boost Converter](/images/TPS63020%20Buck-Boost%20Converter.jpg)

- TP4056 Li-ion battery charging module  
- TPS63020 automatic buck-boost DC-DC converter  

---

### 🔌 Programming & Communication
![FT232RL USB to Serial](/images/USB.png)

- FT232RL USB-to-Serial interface
- Used for bootloading and debugging

---

## 🖨 Schematic Design
![Schematic Design](/images/iot_health_schematic.png)

The schematic was designed using **KiCad**, following manufacturer datasheets for:
- Clock circuitry (8 MHz crystal)
- I2C sensor connections
- Power regulation and battery charging

---

## 🧩 PCB Layout

### PCB Layout (With Connections)
![PCB Layout With Connections](/images/iot_health_pcb_connections.png)

### PCB Layout (Without Connections)
![PCB Layout Without Connections](/images/iot_health_pcb_no_connections.jpg)

---

## 🛠 Fabricated PCB & Final Prototype
![Final Assembled PCB](/images/iot_health_final_board.png)

The final fabricated PCB integrates:
- Power management modules
- Biomedical sensors
- OLED display
- ATmega328P microcontroller

The board was tested for voltage stability, connectivity, and real-world operation.

---

## 💻 Firmware & Software
- Embedded C firmware for ATmega328P
- Sensor interfacing via **I2C**
- Serial communication for data output
- Bootloader-based firmware upload

---

## 🧪 Testing & Validation
- Functional testing of heart rate, SpO₂, and temperature sensors
- Power stability verification under varying load
- Signal validation using multimeters and oscilloscopes
- End-to-end testing on fabricated PCB

---

## ✅ Results
- Accurate real-time physiological measurements
- Stable voltage regulation using buck-boost topology
- Compact, portable PCB-based implementation
- Reliable operation in practical testing

---

## 🌍 Applications
- Remote patient monitoring
- Wearable healthcare devices
- IoT-based medical diagnostics
- Preventive healthcare systems

---

## 🚀 Future Improvements
- Wireless connectivity (Bluetooth / Wi-Fi)
- Cloud integration for data logging
- Power optimization using sleep modes
- Custom wearable enclosure

---

## 👥 Team Contribution
- **Kavin K:** PCB design, power management, firmware development  
- **Gonela Sreeman:** Sensor integration, testing, documentation  

---

## 🔗 Source Code & Design Files
👉 [View project repository on GitHub](https://github.com/kavin1772/iot-health-monitoring-system)
