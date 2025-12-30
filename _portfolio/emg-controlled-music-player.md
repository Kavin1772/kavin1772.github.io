---
title: "EMG Controlled Music Player"
excerpt: "Real-time EMG-based gesture control for music playback"
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
This project implements an **EMG-controlled music player** where muscle activity
from both hands is captured using wearable EMG sensors and mapped to playback
controls such as play/pause and track navigation.

---

## 🏗 System Architecture
![System Block Diagram](/images/emg_block_diagram.png)

---

## 🔧 Hardware
- Dual EMG sensors (left & right hand)
- Microcontroller-based acquisition board
- USB serial interface

---

## 💻 Software
- Embedded C for EMG signal acquisition
- Python for signal parsing and music control
- Threshold-based gesture classification

---

## 🔗 GitHub Repository
👉 [View source code on GitHub](https://github.com/kavin1772/emg-controlled-music-player)
