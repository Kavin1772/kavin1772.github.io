---
title: "EMG Controlled Music Player (ClenchTune)"
excerpt: "Hands-free music playback using palm EMG signals, Arduino, and Python."
collection: portfolio
header:
  teaser: /images/emg_teaser.jpg
---

## 🎥 Demo
<video width="100%" controls muted>
  <source src="/videos/emg_demo.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

---

## 🧠 Overview
ClenchTune is a **hands-free music control system** that leverages **electromyography (EMG)**
signals to enable intuitive, gesture-based media playback. By capturing muscle activity
from **palm muscles** using dual EMG sensors, the system maps natural clenching gestures
to playback commands such as **play/pause** and **track skipping**.

This project demonstrates the feasibility of **biosignal-driven human–computer interaction**
and highlights the potential of EMG-based interfaces in **assistive technology, rehabilitation,
and immersive systems**.

---

## 🎯 Motivation
Traditional input devices such as keyboards, mice, and touchscreens may not be accessible
to all users, particularly individuals with physical impairments. EMG-based interfaces
offer an alternative interaction method by translating **muscle activity into control commands**.
This project explores palm muscle EMG sensing as a reliable and low-cost solution for
hands-free media control.

---

## 🏗 System Architecture
![System Block Diagram](/images/emg_block_diagram.png)

The system follows a real-time signal processing pipeline:

1. EMG signal acquisition from palm muscles  
2. Noise filtering, rectification, and smoothing  
3. Feature extraction and threshold-based gesture detection  
4. Serial communication via Arduino  
5. Media control execution on host system  

This modular design enables fast response times and reliable gesture recognition.

---

## 🔧 Hardware Implementation
- Dual surface EMG sensors (left and right palm muscles)
- Arduino microcontroller
- USB serial communication interface
- Laptop used for processing and audio playback

The EMG sensors detect electrical activity produced by voluntary muscle contractions.
These analog signals are digitized by the Arduino and transmitted to the host computer
for real-time analysis.

---

## 💻 Software Implementation
- **Embedded C (Arduino):**
  - Continuous EMG signal acquisition
  - Serial transmission at 9600 baud

- **Python:**
  - Serial data parsing
  - Moving average filtering for noise reduction
  - Threshold-based gesture recognition
  - Media playback control using the `pygame` library

Two EMG channels are mapped to distinct actions:
- **Channel A0:** Play / Pause
- **Channel A1:** Skip Track

A **1.5-second cooldown mechanism** prevents false triggering due to rapid muscle fluctuations.

---

## 📊 Signal Processing & Gesture Recognition
- Sampling interval: **50 ms**
- Noise rejection outside valid EMG range
- Moving average smoothing
- Threshold-based gesture classification:
  - Play/Pause: 300–500
  - Track Skip: 260–480

Resting hand states produced minimal EMG activity, while clenched gestures generated
high-amplitude signals (>600), enabling clear gesture separation.

---

## ✅ Results
- **~93% gesture recognition accuracy** during experimental testing
- Low-latency real-time response
- Reliable differentiation between open and clenched hand gestures
- Stable performance after calibration

The system responded intuitively to user gestures, providing seamless hands-free
music control.

---

## 🌍 Applications
- Assistive technology for users with limited mobility
- Rehabilitation and physiotherapy interfaces
- Gesture-based entertainment systems
- Human–computer interaction research

---

## 🚀 Future Work
- Machine learning–based gesture classification
- Wireless communication (BLE)
- Expanded gesture set (volume control, previous track)
- Improved robustness to sensor placement variation

---

## 👥 Team Contribution
- **Rafi:** EMG signal acquisition and Arduino interfacing  
- **Kavin & Ratchagan:** Python software development, signal processing,
  gesture recognition logic, and media control integration  
- All members contributed to testing, documentation, and final presentation

---

## 🔗 Source Code
👉 [View full source code on GitHub](https://github.com/kavin1772/emg-controlled-music-player)
