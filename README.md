# ☁️ IoT Cloud FAQ System with Firebase

This is an advanced version of the FAQ system that integrates **Firebase Realtime Database** for dynamic data management. Users can update questions and answers in Firebase, and the device will automatically fetch the latest info.

## 🚀 Key Upgrades
- **Cloud Integration:** Data is fetched from Firebase in real-time.
- **Dynamic Content:** No need to re-upload code to change questions.
- **Persistent Stats:** View counts are saved globally in the cloud database.

## 🛠️ Hardware Setup
- **ESP8266 (NodeMCU)**
- **I2C LCD (20x4)**
- **3 Push Buttons** (Up, Down, Select)

## 🔧 Software Requirements
- Arduino IDE
- `Firebase-ESP8266` Library
- `LiquidCrystal_I2C` Library

## 📂 Firebase Structure
To run this code, set up your Firebase Realtime Database like this:
```json
{
  "faq": {
    "0": {
      "question": "What is DIU?",
      "answer": "Daffodil International University",
      "views": 0
    },
    ...
  }
}
