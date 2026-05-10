### 🔹📡 Real-Time Ultrasonic Distance Measurement & Signal Processing System

## 🚀 Overview

This project demonstrates a **real-time distance measurement system** using an ultrasonic sensor integrated with LabVIEW.
It goes beyond basic sensing by implementing **advanced signal processing techniques** such as noise modeling, PSD analysis, band-pass filtering, and smoothing.

## 🧠 Key Features

* Real-time distance measurement using ultrasonic sensing
* Hardware interfacing via LINX toolkit
* Gaussian noise simulation for robustness testing
* Frequency-domain analysis using PSD
* Band-pass filtering for noise reduction
* Smoothing filter for signal stabilization
* Live waveform visualization in LabVIEW

## 📁 Project Structure

```
Ultrasonic-Distance-LabVIEW/
│── README.md
│── docs/
│   └── ultrasonic filtering using labview rami hesham.pdf
│── labview/
│   └── ultrasonic_filtering.vi
│── images/
│   ├── circuit diagram
│   ├── block diagram for ultrasonic readings before filtering
│   ├── block diagram for ultrasonic readings after filtering
│   ├── Labview front panel
│   └── prototype
```

## 🏗️ System Architecture

The system is composed of:

* Ultrasonic Sensor (HC-SR04)
* Arduino (as hardware interface)
* LabVIEW (data acquisition + processing)

Distance is computed using:

d = (v × t) / 2

Where:

* d = distance
* v = speed of sound (343 m/s)
* t = echo time

## 🔌 Hardware Setup

| Component | Connection |
| --------- | ---------- |
| VCC       | 5V         |
| GND       | GND        |
| Trig      | Pin 9      |
| Echo      | Pin 10     |

## 🧪 Signal Processing Pipeline

1. Raw signal acquisition from ultrasonic sensor
2. Gaussian noise addition
3. Power Spectral Density (PSD) analysis
4. Band-pass filtering
5. Smoothing filter
6. Final clean signal output

## 🖼️ System Screenshots

### 🔹 Circuit diagram

<img width="755" height="517" alt="circuit diagram" src="https://github.com/user-attachments/assets/23009cf5-ce4f-46cf-82e6-1686d3931331" />

### 🔹 Block diagram for ultrasonic readings before filtering

<img width="762" height="467" alt="block diagram for ultrasonic readings before filtering" src="https://github.com/user-attachments/assets/864daea0-bc3b-49a8-9477-7e05063dc7cb" />


### 🔹 Block diagram for ultrasonic readings after adding Filtering Pipeline

<img width="887" height="517" alt="block diagram for ultrasonic readings after filtering" src="https://github.com/user-attachments/assets/011be761-5a7f-42f6-b2bf-ab2fd3bb6175" />


### 🔹 Labview front panel

<img width="882" height="357" alt="labview front panel" src="https://github.com/user-attachments/assets/f4ae6d1d-e651-4482-af66-7b51e0a48884" />


### 🔹 Prototype

<img width="407" height="436" alt="prototype" src="https://github.com/user-attachments/assets/428bd0fc-b125-4682-acd4-e9a888744ee4" />


## 🛠️ Requirements

* LabVIEW
* LINX Toolkit
* Arduino Uno
* HC-SR04 Ultrasonic Sensor

## ⚙️ How to Run

1. Upload LINX firmware to Arduino
2. Connect Arduino via USB
3. Open LabVIEW VI
4. Select COM port
5. Run the VI

## 📊 Results

* Measurement Range: 2 cm – 400 cm
* Accuracy: ±3 mm
* Real-time filtered signal visualization

## 🎯 Project Highlights

This project demonstrates:

* Real-time embedded system integration
* Practical signal processing implementation
* Hardware-in-the-loop design

## 👨‍💻 Author

**Rami Hesham**
Mechatronics & Robotics Engineer

## ⭐ Future Improvements

* ROS integration
* Sensor fusion with LiDAR
