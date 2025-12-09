# 🚨 Smart Helmet for Accident Detection and Emergency Alerts
Smart Helmet | Arduino-based accident detection with GPS + GSM emergency alerts (offline, low-cost, scalable)


A **low-cost, standalone smart helmet system** that detects two-wheeler accidents and
automatically alerts emergency contacts with the rider’s live GPS location via SMS —
**without requiring internet or smartphones**.

This project was developed as part of the **Development Engineering Project (CP301) at IIT Ropar**.

---

## 📌 Key Features
- **Accident Detection:** ADXL345 accelerometer monitors impacts and detects crashes.
- **Real-Time Alerts:** SIM900A GSM module sends SMS + initiates a call to emergency contacts.
- **Location Tracking:** NEO-6M GPS module provides live coordinates (Google Maps link).
- **Standalone System:** Arduino Uno + 12V battery → works without apps or internet.
- **Affordable:** Prototype built for under ₹5,000 (~$45).
- **Expandable:** Alcohol detection (MQ-3), app integration, and solar charging in future versions.

---

## 🛠️ System Architecture
1. **Detection Module** – ADXL345 accelerometer senses abnormal impacts.
2. **Processing Module** – Arduino Uno processes sensor data and triggers alerts.
3. **Location Module** – NEO-6M GPS provides live coordinates.
4. **Communication Module** – SIM900A GSM sends SMS/calls to contacts.

![System Architecture](hardware/circuit_schematic.png)

---

## 📊 Results
- **Impact Detection:** ~95% accuracy for >20g crashes.
- **False Positives:** <5%.
- **GPS Accuracy:** 2.5 m (open field), 8–12 m (urban).
- **GSM Reliability:** 97% SMS success, ~8s delivery time.
- **Battery Life:** 9.5 hours continuous operation.

📷 Example alert SMS:  
![SMS Alert Screenshot](results/sms_alert_screenshot.png)

---

## 📂 Repository Structure
- `report/` – Full project report, poster, and presentation.  
- `hardware/` – Circuit diagrams, hardware photos, specs.  
- `code/` – Arduino sketches (to be added).  
- `results/` – Test results, screenshots, performance data.  
- `references/` – Key academic references.

---

## 📥 Prototype Testings (Google Drive)
Due to GitHub storage limits, the full setup files are hosted externally.  
👉 [Download Full Setup](https://drive.google.com/drive/folders/1t1garhPQyA8kcemrgB3G1u8s-PZxF-9c?usp=sharing)

---

## 🎓 Team
- Priyanshu Rao  
- Priyanshu Singh  
- Aditya Kumar  
- Aryan Daga  
**Supervisor:** Prof. Harpreet Singh (IIT Ropar)

---

## 📌 Future Work
- Upgrade to **ADXL377 accelerometer** for high-impact crashes.  
- Replace Arduino Uno with **ESP32** (Wi-Fi/Bluetooth + lower power).  
- Add **alcohol detection + ignition control**.  
- Solar-powered battery extension.  
- Develop **mobile app** for real-time tracking & health logs.  

---

## 📜 License
This project is open-source under the **MIT License**.
