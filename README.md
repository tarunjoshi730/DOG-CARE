# DOG-CARE
HACKATHON
# 🐶 Dog Care – Smart AI-Enabled Pet Health & Safety Monitor

## 🚀 Overview
**Dog Care** is a smart AI + IoT solution designed to help dog owners remotely monitor their pets’ **health, safety, and activity**.  
The system combines a wearable collar device, IoT home sensors, and AI-powered behavior analysis to provide **real-time insights and alerts** via a mobile/web app.  

---

## 🐕 The Real-Life Problem
Dog owners, especially those who leave pets at home or in a yard while at work, often worry about:
- 🌡️ Overheating in hot weather  
- 🚪 Escaping from the yard  
- 🥤 Not eating or drinking enough  
- 🩺 Strange behaviors that might signal illness  
- 🐾 Getting lost if they run away  

👉 Currently, monitoring a dog’s well-being remotely is **difficult and expensive** without professional setups.  

---

## 💡 The Solution
Dog Care provides a **wearable + home IoT monitoring system** with AI integration to track:  

- **Vitals & Activity** – via a lightweight collar (heart rate, temperature, GPS, motion tracking).  
- **Behavior Detection** – AI camera inside home/yard to detect unusual movements (limping, excessive scratching, lethargy, stress barking).  
- **Environmental Safety** – IoT sensors monitor room/yard conditions (temperature, humidity, water bowl level).  
- **Runaway Alerts** – GPS + geofencing alerts when a dog leaves safe zones.  

📱 A **web/mobile app** for owners includes:  
- Live vitals dashboard  
- Behavior anomaly alerts  
- Location tracking map  
- Remote camera feed  

---

## 🧠 How AI Fits In
- **Computer Vision** – Detect abnormal behaviors (e.g., limping, excessive licking) from camera feeds.  
- **ML Predictive Models** – Learn the dog’s daily activity pattern and detect unusual trends.  
- **Image Recognition** – Recognize posture and distinguish between normal rest vs. possible distress.  

---

## 🛠️ Tech Stack

### IoT Layer
- Collar: **ESP32 + GPS + heart rate/temp sensor + accelerometer**  
- Home Node: **Raspberry Pi + DHT11 (temp/humidity) + water level sensor**

### AI Layer
- **TensorFlow Lite** – lightweight ML inference on-device  
- **OpenCV + YOLO** – posture & behavior detection  

### Web/Mobile Layer
- **Backend:** FastAPI / Node.js  
- **Frontend:** HTML CSS JS with code no code  
- **Real-time Communication:** MQTT for IoT devices, WebSockets for alerts  
- **Cloud/Integration:** Firebase or AWS IoT Core  

---

## 🌍 Why It’s Impactful
- 🛡️ **Safety:** Prevents overheating, dehydration, and runaway risks.  
- 🩺 **Health:** Early detection of illness through AI-analyzed behavior changes.  
- 📲 **Peace of Mind:** Real-time monitoring when owners are away.  
- 📈 **Scalability:** Expandable for shelters, vets, and service/working dogs.  

---

## 📐 System Architecture
```mermaid
graph TD
    A[Dog Collar IoT Device] -->|Vitals Data| C[Cloud Backend]
    B[Home IoT Sensors + Camera] -->|Env + Behavior Data| C
    C --> D[AI/ML Engine: TensorFlow Lite + OpenCV]
    D --> E[Mobile App]
    D --> F[Web Dashboard]
    E -->|Live Alerts| User[Dog Owner]
    F -->|Reports/Insights| User
