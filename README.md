# watt_a_mess — AI-Powered Self-Healing Protection for Power Grids**

*A dual-node, edge-intelligent system that predicts transformer failures **before** they happen.*

---

## ⚡ **Overview**

**Watt a mess** is an industrial-grade, intelligent monitoring system designed for high-voltage substations.
It listens, learns, predicts, and protects — turning reactive maintenance into **proactive grid safety**.

> **Mission:** Prevent transformer explosions, eliminate blind-spot failures, and protect both infrastructure and humans.

---

## 🧠 **Core Features**

### 🔹 **Dual-Node Architecture**

* **Node-A (The Scout):** Arduino-powered wireless sensor head using **433 MHz RF** for safe, galvanically-isolated data transmission.
* **Node-B (The Brain):** ESP32-based AI hub running **Edge-Impulse TinyML** models for real-time fault prediction.

### 🔹 **Edge AI Fault Detection**

* Acoustic FFT + Spectrogram analysis
* Detects high-frequency arcing, sparks, loose coils
* Classification confidence > 90% in live tests

### 🔹 **Active Cooling & Self-Healing**

* Automatic thermal mitigation via **TIP122-driven Fan System**
* Real-time response even without WiFi or cloud

### 🔹 **Grid Protection Logic**

* **Green LED:** Circuit Breaker Closed
* **Red LED:** Trip Mode / Fault Isolation
* Prevents catastrophic failures during transformer stress events

### 🔹 **IoT + Forensics**

* Live alerts to **Blynk App**
* Local data logging via **SD-Card Black Box**
* Fully functional during network outages (Edge Resilience)

---

## 🔧 **Hardware Stack**

* Arduino UNO (Remote Node)
* ESP32 DevKit V1 (AI Node)
* 433MHz RF Tx/Rx
* DHT11, CZN-15E Microphone, SW-420 Vibration Sensor
* TIP122 Darlington Transistor
* DC Cooling Fan
* OLED Display
* SD Card Logger

---

## 🎯 **Why Grid-Guardian?**

* Predicts failures **days earlier** than temperature-based systems
* No wired sensors — **Air-Gap Safety** against lightning & HV surges
* Fully autonomous real-time protection
* Industrial, scalable, field-ready hardware design
* A perfect fusion of **IoT + Edge AI + Power System Safety**

---

## 🛰️ **Tech Stack**

**Languages:** C, C++, Arduino, ESP-IDF
**AI Tools:** Edge Impulse, TinyML, FFT Spectral Analysis
**Protocols:** RF Telemetry, WiFi, Blynk IoT
**Hardware:** ESP32 Dual Core, Arduino, SD Logging, TIP122, Sensors

---

## 🧩 **System Diagram**

```
Node A (Arduino UNO) ----(433 MHz RF)----> Node B (ESP32 AI Core)
          |                                        |
     DHT11 Sensor                           Mic + Vibration
                                                |
                                           AI Inference
                                                |
                             Fan Control • Trip LEDs • IoT Alerts
```

---

## 🚀 **Status**

✔️ Prototype Complete
✔️ Live Demo Successful
✔️ Predictive Fault Detection Validated
🔜 Next: Cloud Dashboard + Multi-Transformer Scaling

