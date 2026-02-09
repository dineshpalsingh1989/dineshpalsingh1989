# 👋 Hi, I’m Dineshpal Singh

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/dineshpalsingh1989/)
[![Email](https://img.shields.io/badge/Email-Contact_Me-red?style=for-the-badge&logo=gmail)](mailto:your-email@example.com)

### 🔧 Industrial IoT Specialist | Condition Monitoring | Predictive Maintenance

I design and deploy end-to-end **Industrial IoT (IoT)** systems specifically for monitoring rotating equipment. My work bridges the gap between raw sensor data and actionable maintenance insights, utilizing secure pipelines, real-time dashboards, and edge analytics.

---

### 👀 Focus Areas

* 🏭 **Machine Health:** Systems for rotating equipment monitoring & diagnostics.
* 📡 **Edge Hardware:** ESP32 (C3/S3), LoRa, BLE, and CircuitPython integration.
* 🔄 **Data Pipelines:** Modbus RTU/TCP, Secure MQTT, and Node-RED flows.
* 📊 **Visualization:** Custom, high-speed dashboards using Dash/Plotly & Streamlit.

---

### 🧰 Tech Stack Snapshot

| **Hardware & Edge** | **Protocols & Comms** | **Cloud & Backend** | **Visualization** |
| :--- | :--- | :--- | :--- |
| ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white) **ESP32-C3** | ![MQTT](https://img.shields.io/badge/MQTT-3C5280?style=flat&logo=eclipse-mosquitto&logoColor=white) **Secure MQTT** | ![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=google-cloud&logoColor=white) **GCP** | ![Dash](https://img.shields.io/badge/Dash-0081CB?style=flat&logo=plotly&logoColor=white) **Plotly Dash** |
| ![WIZnet](https://img.shields.io/badge/WIZnet_W5500-005696?style=flat&logo=ethernet&logoColor=white) **Ethernet** | ![Modbus](https://img.shields.io/badge/Modbus-RTU%2FTCP-orange?style=flat) **Modbus** | ![HiveMQ](https://img.shields.io/badge/HiveMQ-F39C12?style=flat&logo=hivemq&logoColor=white) **HiveMQ** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) **Streamlit** |
| ![Sensors](https://img.shields.io/badge/Sensors-Industrial-green?style=flat) **Vibration** | ![LoRaWAN](https://img.shields.io/badge/LoRaWAN-0091BD?style=flat&logo=lora&logoColor=white) **LoRa** | ![Node-RED](https://img.shields.io/badge/Node--RED-8F0000?style=flat&logo=nodered&logoColor=white) **Node-RED** | ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white) **Grafana** |

---
╔══════════════════════════════════════════════════════════════╗
║        INDUSTRIAL IIOT VIBRATION MONITORING PLATFORM        ║
║   ESP32 (883M Wilcoxon) • MQTT • Firebase • Google Cloud    ║
║                 Remote OTA • Real-Time Analytics           ║
╚══════════════════════════════════════════════════════════════╝

┌──────────────────────────────────────────────────────────────┐
│ 🏗️ ARCHITECTURE DIAGRAM                                      │
├──────────────────────────────────────────────────────────────┤
│                                                              │
│   [ESP32 Nodes]                                              │
│       │ MQTT/TLS                                             │
│       ▼                                                      │
│   [MQTT Broker]                                              │
│       │                                                      │
│   ┌───────────────┐     ┌───────────────────────────────┐   │
│   │ Firebase      │     │ Google Cloud Storage / SQL    │   │
│   │ Realtime DB   │     │ / InfluxDB                    │   │
│   └───────────────┘     └───────────────────────────────┘   │
│                                                              │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ 🔐 SECURE EDGE & BROKER COMMUNICATION                       │
├──────────────────────────────────────────────────────────────┤
│ Architecture:                                               │
│   ESP32 → TLS MQTT Broker → Cloud Backend                  │
│                                                              │
│ • TLS-encrypted MQTT communication                          │
│ • Certificate-based authentication                          │
│ • Secure payload transmission                               │
│ • Hardened edge configuration                               │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ 🗄️ INDUSTRIAL DATA MODELING                                 │
├──────────────────────────────────────────────────────────────┤
│ • InfluxDB – High-frequency vibration & FFT time-series    │
│ • SQL (PostgreSQL / SQLite) – Asset & maintenance records  │
│ • Optimized schema for:                                     │
│     - Trend analysis                                        │
│     - Anomaly detection                                     │
│     - Predictive maintenance                                │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ 🔥 HYBRID REAL-TIME DASHBOARDS                              │
├──────────────────────────────────────────────────────────────┤
│ • Firebase Realtime DB / Firestore – Live telemetry        │
│ • SQL-based historical analytics                            │
│ • Python (Streamlit / Custom Web UI) dashboards            │
│ • MQTT-driven instant updates                               │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ ☁️ GOOGLE CLOUD & FIREBASE BACKEND                          │
├──────────────────────────────────────────────────────────────┤
│ • Firebase – Real-time sensor ingestion                     │
│ • Google Cloud Storage – Waveform & FFT archive            │
│ • Cloud Functions – Processing & alert automation          │
│ • IAM – Secure device identity management                   │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ 🚀 OTA FIRMWARE UPDATE SYSTEM                               │
│    ESP32 (883M Wilcoxon Monitoring Node)                    │
├──────────────────────────────────────────────────────────────┤
│ Update Workflow:                                            │
│ 1. Device checks firmware version (HTTPS / MQTT trigger)   │
│ 2. Downloads firmware from GCS or Secure VPS               │
│ 3. Verifies SHA256 integrity                                │
│ 4. Dual-partition OTA flash                                 │
│ 5. Automatic rollback on failure                            │
│                                                              │
│ Security Features:                                          │
│ • TLS-secured firmware delivery                             │
│ • Integrity verification                                    │
│ • Optional firmware signing                                 │
│ • Safe rollback mechanism                                   │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ 📡 SYSTEM CAPABILITIES                                      │
├──────────────────────────────────────────────────────────────┤
│ • Real-time vibration streaming                             │
│ • FFT data acquisition                                      │
│ • Cloud-based analytics                                     │
│ • Automated alerting                                        │
│ • Secure MQTT communication                                 │
│ • Remote OTA firmware management                            │
│ • Scalable industrial deployment                            │
└──────────────────────────────────────────────────────────────┘


┌──────────────────────────────────────────────────────────────┐
│ ⚡ QUICK START GUIDE                                        │
├──────────────────────────────────────────────────────────────┤
│ 1️⃣ Clone the repo:                                         │
│     git clone https://github.com/yourusername/iiot-vib.git  │
│                                                              │
│ 2️⃣ Install dependencies:                                   │
│     • Python: pip install -r requirements.txt              │
│     • MQTT Broker: Configure TLS certificates              │
│     • Firebase / GCP: Setup projects & credentials         │
│                                                              │
│ 3️⃣ Flash ESP32 nodes:                                      │
│     • Configure WiFi & MQTT settings                        │
│     • Enable OTA via HTTPS / MQTT trigger                   │
│                                                              │
│ 4️⃣ Launch dashboards:                                      │
│     • Streamlit / Web UI                                   │
│     • Realtime telemetry via Firebase                       │
│     • Historical analytics via SQL / InfluxDB               │
└──────────────────────────────────────────────────────────────┘

---

🌐 **Platforms:**  
![MQTT](https://img.shields.io/badge/MQTT-Broker-blue?style=flat&logo=eclipse-mosquitto&logoColor=white)  
**mqtt.com.my** – MQTT Broker & Industrial IIoT Messaging Platform  

🗄️ **Databases:**  
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat&logo=postgresql&logoColor=white)
![InfluxDB](https://img.shields.io/badge/InfluxDB-22ADF6?style=flat&logo=influxdb&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)  

SQL (MySQL / PostgreSQL), InfluxDB, Firebase  

🚨 **Alerts & Automation:**  
![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=flat&logo=telegram&logoColor=white)
![Automation](https://img.shields.io/badge/Automation-Reports-green?style=flat)  

Telegram Bot alerts, automated reports, threshold-based alarms


---
🔧 **Hardware:**  
![ESP32](https://img.shields.io/badge/ESP32-ESP32%2FC3-E7352C?style=flat&logo=espressif&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-Edge-C51A4A?style=flat&logo=raspberry-pi&logoColor=white)
![LoRa](https://img.shields.io/badge/LoRa-Long_Range-0091BD?style=flat&logo=lora&logoColor=white)
![BLE](https://img.shields.io/badge/BLE-Bluetooth-0082FC?style=flat&logo=bluetooth&logoColor=white)
![Sensors](https://img.shields.io/badge/Industrial-Sensors-green?style=flat)  

ESP32 / ESP32-C3, **Raspberry Pi**, LoRa, BLE, Industrial Sensors  

📡 **Protocols & Communication:**  
![MQTT](https://img.shields.io/badge/MQTT-Eclipse-blue?style=flat&logo=eclipse-mosquitto&logoColor=white)
![Modbus](https://img.shields.io/badge/Modbus-RTU%2FTCP-orange?style=flat)
![HTTP](https://img.shields.io/badge/HTTP-REST-lightgrey?style=flat)
![BLE](https://img.shields.io/badge/BLE-Bluetooth-0082FC?style=flat&logo=bluetooth&logoColor=white)  

MQTT, Modbus RTU/TCP, HTTP, BLE  

☁️ **Cloud & Tools:**  
![Node-RED](https://img.shields.io/badge/Node--RED-Flow--Based-8F0000?style=flat&logo=nodered&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-GCP-4285F4?style=flat&logo=google-cloud&logoColor=white)
![HiveMQ](https://img.shields.io/badge/HiveMQ-MQTT-F39C12?style=flat&logo=hivemq&logoColor=white)
![InfluxDB](https://img.shields.io/badge/InfluxDB-TimeSeries-22ADF6?style=flat&logo=influxdb&logoColor=white)  

Node-RED, Google Cloud, HiveMQ, InfluxDB  

📊 **Visualization & Dashboards:**  
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboards-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![Dash](https://img.shields.io/badge/Dash-Plotly-0081CB?style=flat&logo=plotly&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-Interactive-3F4F75?style=flat&logo=plotly&logoColor=white)  

Streamlit, Dash, Plotly  

🚨 **Alerts & Reporting:**  
![Telegram](https://img.shields.io/badge/Telegram-Bot-26A5E4?style=flat&logo=telegram&logoColor=white)
![Reports](https://img.shields.io/badge/Automated-Reports-green?style=flat)  

Telegram Bot alerts, automated reporting

---
🌐 **Live IIoT Dashboards & Proof-of-Concepts**

🔧 **Industrial Monitoring Dashboard**  
![Dashboard](https://img.shields.io/badge/Live-Dashboard-0081CB?style=flat&logo=plotly&logoColor=white)
![IIoT](https://img.shields.io/badge/IIoT-Monitoring-green?style=flat)
![Status](https://img.shields.io/badge/Status-Online-brightgreen?style=flat)  
🔗 http://176.97.117.59/

📊 **Real-Time Analytics & Visualization App**  
![Streamlit](https://img.shields.io/badge/Streamlit-Live_App-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![Realtime](https://img.shields.io/badge/Realtime-Data-blue?style=flat)
![Cloud](https://img.shields.io/badge/Cloud-IIoT-4285F4?style=flat&logo=google-cloud&logoColor=white)  
🔗 http://213.111.157.130:8050/  or 213.111.157.130

---
### 🤝 Open to Collaboration

I am actively looking to collaborate on projects involving:
* **Predictive Maintenance Algorithms** (FFT analysis, anomaly detection).
* **Smart Industrial Sensors** (Custom PCB design or firmware).
* **Scalable IIoT Architectures** (From sensor to cloud dashboard).

> *"Turning vibration into value."*

[**📫 Let’s connect & build reliable industrial systems!**](https://github.com/dineshpalsingh1989)



