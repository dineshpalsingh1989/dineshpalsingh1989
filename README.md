# 👋 Hi, I’m Dineshpal Singh

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/dineshpalsingh1989/)
[![Email](https://img.shields.io/badge/Email-Contact_Me-red?style=for-the-badge&logo=gmail)](mailto:your-email@example.com)

### 🔧 Industrial IoT Specialist | Condition Monitoring | Predictive Maintenance

I design and deploy end-to-end **Industrial IoT (IIoT)** systems specifically for monitoring rotating equipment. My work bridges the gap between raw sensor data and actionable maintenance insights, utilizing secure pipelines, real-time dashboards, and edge analytics.

> *"Turning vibration into value."*

---

### 🚀 What I'm Building Now

#### 📡 Milesight Dashboard V2.0

A self-hosted **LoRaWAN and MQTT dashboard** for Milesight sensors and gateways, with **Firebase Firestore** storage and optional **Telegram + Gemini** sensor questions.

- **Live monitoring:** device cards, history charts, CSV export, storage usage, and a workspace debug stream.
- **Expanded sensor coverage:** 24 named device profiles, including 17 additions for leak detection, pulse metering, tank distance, water level, soil, pipe pressure, current, visitor counting, temperature, tilt, and weather. New profiles use gateway-decoded JSON.
- **Two-way MQTT:** readings flow from sensors to the dashboard; owners can publish commands through the gateway's Embedded Network Server.
- **Device controls:** hexadecimal/Base64 command previews, configurable workspace topics, FPort and confirmation options, UC300 DO1/DO2 presets, and command history. MQTT publication does not confirm sensor execution.
- **Local demo:** 24 sample devices with charts, CSV downloads, settings, and simulated commands. No Firebase credentials or gateway needed.
- **Deployment:** Docker or Node.js, workspace access controls, protected Firebase setup, and GitHub Actions checks.

[**View project**](https://github.com/dineshpalsingh1989/milesight-dashboard) | [**Setup & sensor list**](https://github.com/dineshpalsingh1989/milesight-dashboard#readme) | [**Latest updates**](https://github.com/dineshpalsingh1989/milesight-dashboard/blob/main/CHANGELOG.md)

![Milesight Dashboard architecture: sensor readings and MQTT commands](https://raw.githubusercontent.com/dineshpalsingh1989/milesight-dashboard/main/docs/architecture.svg)

Try the demo after cloning the project and installing dependencies:

```sh
npm ci
npm run demo
```

Open **http://localhost:8081**. Demo data and commands are simulated; physical gateway and sensor delivery remain unverified.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white)
![MQTT](https://img.shields.io/badge/MQTT-3C5280?style=flat&logo=eclipse-mosquitto&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

#### 🚦 IRIV Speed Console (Sensata AI Speed)
A local-first speed-enforcement dashboard for the **Cytron IRIV PiControl CM5** and **Milesight TS4466 / TS8266** LPR cameras.

* Live and historical speed/plate records with search, pagination and image evidence
* Telegram and email alerts with a persistent outbox, so no alert is lost when offline
* Workflow automation, analytics and hardware controls
* SQLite storage, single-file build, systemd service, CI with Bandit security scans
* Illustrated user manual and offline PowerPoint guide

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white)
*(Private repository, contact me for a demo.)*

#### 📈 Open-Source Vibration Monitoring Projects
| Project | What it does |
| :--- | :--- |
| [Wilcoxon-883M RTU to TCP and MQTT](https://github.com/dineshpalsingh1989/Wilcoxon-883M_RTU-to-TCP-and-MQTT) | ESP32 (C++) firmware bridging Wilcoxon 883M Modbus RTU sensors to Modbus TCP and MQTT |
| [Wilcoxon-ILA200-DashboardESP32](https://github.com/dineshpalsingh1989/Wilcoxon-ILA200-DashboardESP32) | ESP32 firmware with edge FFT analysis, Modbus TCP and MQTT for the Wilcoxon ILA200 |
| [Wilcoxon-VDS](https://github.com/dineshpalsingh1989/Wilcoxon-VDS) | Real-time vibration dashboard using Python Dash, MQTT, OPC and SQLite |

---

### 👀 Focus Areas

* 🏭 **Machine Health:** Rotating equipment monitoring & diagnostics with [![Wilcoxon 883M](https://img.shields.io/badge/Wilcoxon_883M-Sensor-4ABDAC?style=flat)](https://www.wilcoxon.com/product/883M) and [![VDS](https://img.shields.io/badge/VDS-Vibration_System-FF6F61?style=flat)](https://www.vds.com)  
* 📡 **Edge Hardware & Sensors:** [![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white)](), [![ESP32-C3](https://img.shields.io/badge/ESP32-C3%2FS3-E7352C?style=flat&logo=espressif&logoColor=white)](), [![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-C51A4A?style=flat&logo=raspberry-pi&logoColor=white)](), [![LoRa](https://img.shields.io/badge/LoRa-0091BD?style=flat&logo=lora&logoColor=white)](), [![BLE](https://img.shields.io/badge/BLE-0082FC?style=flat&logo=bluetooth&logoColor=white)](), [![Wilcoxon 883M](https://img.shields.io/badge/Wilcoxon_883M-Sensor-4ABDAC?style=flat)](https://www.wilcoxon.com/product/883M), [![VDS](https://img.shields.io/badge/VDS-Vibration_System-FF6F61?style=flat)](https://www.vds.com) 


---

### 🧰 Tech Stack Snapshot

| **Hardware & Edge** | **Protocols & Comms** | **Cloud & Backend** | **Visualization** |
| :--- | :--- | :--- | :--- |
| ![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white) **ESP32-C3** | ![MQTT](https://img.shields.io/badge/MQTT-3C5280?style=flat&logo=eclipse-mosquitto&logoColor=white) **Secure MQTT** | ![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=google-cloud&logoColor=white) **GCP** | ![Dash](https://img.shields.io/badge/Dash-0081CB?style=flat&logo=plotly&logoColor=white) **Plotly Dash** |
| ![WIZnet](https://img.shields.io/badge/WIZnet_W5500-005696?style=flat&logo=ethernet&logoColor=white) **Ethernet** | ![Modbus](https://img.shields.io/badge/Modbus-RTU%2FTCP-orange?style=flat) **Modbus** | ![HiveMQ](https://img.shields.io/badge/HiveMQ-F39C12?style=flat&logo=hivemq&logoColor=white) **HiveMQ** | ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white) **Streamlit** |
| ![Sensors](https://img.shields.io/badge/Sensors-Industrial-green?style=flat) **Vibration** | ![LoRaWAN](https://img.shields.io/badge/LoRaWAN-0091BD?style=flat&logo=lora&logoColor=white) **LoRa** | ![Node-RED](https://img.shields.io/badge/Node--RED-8F0000?style=flat&logo=nodered&logoColor=white) **Node-RED** | ![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat&logo=grafana&logoColor=white) **Grafana** |

---
🌱 Currently Exploring

🛡️ Secure Edge & Broker Comms: Deploying TLS-secured MQTT streams between ESP32-C3 and mqtt.com.my, ensuring enterprise-grade encrypted telemetry for sensitive industrial environments.

📲 Remote Lifecycle Management (FOTA): Implementing Online Firmware-Over-The-Air updates for ESP32 nodes integrated with Wilcoxon 883M vibration sensors. This enables remote logic refinement and sensor recalibration without physical site access.

☁️ Google Cloud & Firebase IIoT:

⚡ Real-time Ingestion: Utilizing Firebase Realtime Database/Firestore for live streaming of high-frequency vibration data.

📦 Cloud Archival: Leveraging Google Cloud Storage for long-term vibration waveform and FFT data archiving.

⚙️ System Orchestration: Using Cloud Functions for automated processing, intelligent alerts, and seamless scaling from prototype to industrial production.

📊 Hybrid Dashboards & Automation:

Architecting unified views combining Firebase (Real-time) with SQL/InfluxDB (Historical Analytics).

Integrating Telegram Bots for instant threshold notifications and Automated PDF/Excel Reporting generated via Python backends.

🚦 Edge Vision: LPR cameras and speed-enforcement workflows (Cytron IRIV CM5, Milesight).

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



