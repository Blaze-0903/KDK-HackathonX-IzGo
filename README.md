# IoT-Based Home Automation System

## 📌 Project Overview
This project focuses on building an **IoT-based home automation system** that allows users to **control home appliances remotely** via a **mobile app**. The system also integrates **sensors to automate tasks**, such as turning off lights when no one is in the room.

## 🔥 Features
- ✅ **Remote control of home appliances** (Lights, Fan, AC) using a mobile app
- ✅ **Real-time sensor monitoring** (Motion, Light, Temperature)
- ✅ **Automation**: Turns off lights when no motion is detected
- ✅ **Wi-Fi communication using ESP32/ESP8266**
- ✅ **Firebase integration for real-time updates**

## 🛠️ Components Used
| Component         | Description                                       |
|------------------|--------------------------------------------------|
| **ESP32/ESP8266** | Microcontroller with Wi-Fi connectivity         |
| **Relay Module**  | Controls switching of appliances                |
| **DHT11/DHT22**   | Temperature & Humidity Sensor                   |
| **PIR Sensor**    | Detects motion to automate lighting             |
| **LDR Sensor**    | Detects ambient light level                     |
| **Firebase**      | Cloud database for real-time data sync          |
| **Flutter App**   | Mobile app to monitor and control appliances    |

## 🚀 How It Works
1. **Sensors** (PIR, LDR, Temperature) collect real-time data.
2. **ESP32/ESP8266** processes the sensor data and updates Firebase.
3. The **Flutter App** retrieves data from Firebase and displays it.
4. Users can **turn appliances ON/OFF** from the app, updating Firebase.
5. The ESP **reads Firebase changes** and toggles the appliances accordingly.

## 📲 Mobile App UI
- **Live Sensor Data Display** (Temperature, Motion, Light Level)
- **Switch Controls** for appliances (Fan, AC, Lights)
- **Real-time updates via Firebase**

## 🖥️ Setup Guide
### **1️⃣ Hardware Setup**
- Connect ESP32/ESP8266 to sensors and relay module.
- Ensure Wi-Fi connectivity.

### **2️⃣ Firebase Setup**
1. Create a **Firebase project** at [Firebase Console](https://console.firebase.google.com/).
2. Enable **Realtime Database** and set rules to "read/write".
3. Get the **API Key & Database URL**.

### **3️⃣ ESP32/ESP8266 Code**
- Install **Firebase ESP32/ESP8266 Library** in Arduino IDE.
- Upload the ESP code to send sensor data and receive control commands.

### **4️⃣ Flutter App Setup**
- Install dependencies:
  ```sh
  flutter pub add firebase_core firebase_database
  ```
- Add Firebase config (`google-services.json`).
- Run the app:
  ```sh
  flutter run
  ```

## 📌 Future Enhancements
- 🌍 **Voice Control Integration** (Google Assistant / Alexa)
- 📡 **MQTT Protocol** for real-time communication
- 📊 **Data Analytics Dashboard** for usage statistics

## 💡 Conclusion
This project **enhances home automation** by providing remote control, real-time monitoring, and automation. Using **ESP32, Firebase, and Flutter**, it creates an **efficient and user-friendly system**.

---

📌 **Contributors:** [Your Name]  
📌 **GitHub Repository:** [Your Repo Link]  
📌 **License:** MIT

