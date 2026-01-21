<div align="center">

  <h1>🗑️ IoT Smart Trash Bin System</h1>
  <p>
    <b>An Automated, Touchless Waste Management Solution based on ESP32</b>
  </p>

  <img src="https://img.shields.io/badge/Device-ESP32-red?style=for-the-badge&logo=espressif" alt="ESP32" />
  <img src="https://img.shields.io/badge/Language-C%2B%2B-blue?style=for-the-badge&logo=cplusplus" alt="C++" />
  <img src="https://img.shields.io/badge/Platform-Arduino-teal?style=for-the-badge&logo=arduino" alt="Arduino" />
  <img src="https://img.shields.io/badge/IoT-Telegram_Bot-2CA5E0?style=for-the-badge&logo=telegram" alt="Telegram" />

  <br><br>
  <img width="938" height="285" alt="image" src="https://github.com/user-attachments/assets/b2ae7dd4-576a-4490-a765-c154ebce02ed" />


</div>

<br>

## 📖 Project Overview
This project addresses hygiene and efficiency in waste management. It is a smart trash bin that opens automatically when a user approaches and notifies the owner via smartphone when the bin is full.

Designed as a **Computer Engineering implementation**, this system integrates hardware control (Servos/Sensors) with IoT connectivity (Telegram API).

## ✨ Key Features
* **🙌 Touchless Operation:** Automatically opens the lid using `HC-SR04` Ultrasonic sensors to prevent physical contact.
* **📱 Real-time Notifications:** Sends a "Bin Full" alert to your smartphone via **Telegram Bot** when triggered by the `TCRT5000` IR sensor.
* **🔋 Portable Power:** Powered by `Li-ion 18650` batteries with a TP4056 charging module and DC-DC Booster for stable voltage.

## 🛠️ Tech Stack & Hardware
| Component | Specification | Function |
| :--- | :--- | :--- |
| **Microcontroller** | ESP32 DEVKITC V4 | Main processing unit & Wi-Fi connectivity |
| **Sensors** | HC-SR04 & TCRT5000 | Distance detection (Lid) & Trash Level (IR) |
| **Actuator** | Servo MG996R | High-torque servo to drive the bin lid |
| **Power** | 2x Li-ion 18650 | Rechargeable power source |
| **Software** | C++ (Arduino IDE) | Firmware logic & Telegram API integration |

## ⚙️ System Architecture & Logic
The system operates on a dual-sensor logic:
1.  **Input 1 (Ultrasonic):** Detects object < 30cm -> Triggers Servo to Open.
2.  **Input 2 (Infrared):** Detects obstruction inside bin -> Triggers Wi-Fi module -> Sends Telegram Message.

## 📄 Full Documentation
For detailed technical specifications, electronic schematics, and source code explanation, please refer to the complete proposal document below:

<div align="center">
  <a href="documentation/Projek MM1_Rifan Januar Rifa'i_235150307111026.pdf">
    <img src="https://img.shields.io/badge/Download-Project_PDF-red?style=for-the-badge&logo=adobeacrobatreader" alt="Download PDF" />
  </a>
</div>
