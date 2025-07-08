# 🐘 Elephant Detection System Using YOLOv8 and Flask

## 🚀 Overview

This project is a **real-time elephant detection system** built using the YOLOv8 object detection model and deployed via a Flask web application. It is designed to assist in **wildlife monitoring** and **human-elephant conflict mitigation**, especially in forest borders and farmland areas.

- 🔍 **Detects elephants from static images or live webcam feeds**
- 📩 **Sends instant SMS alerts via Twilio**
- 💾 **Logs detection events to a SQLite database**
- 🧠 **Trained on infrared (night-time) images for round-the-clock use**

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **Backend:** Flask
- **AI Model:** YOLOv8 (Ultralytics)
- **Computer Vision:** OpenCV
- **Database:** SQLite3
- **SMS Alerts:** Twilio API
- **Front-end:** HTML (Jinja2 templating)

---

## 📦 Features

| Feature                  | Description                                             |
|--------------------------|---------------------------------------------------------|
| 🧠 Custom YOLOv8 Model   | Trained on night-time IR elephant images                |
| 📷 Real-Time Detection    | Webcam-based video stream detection                     |
| 📤 Image Upload           | Detect elephants in uploaded `.jpg` / `.png` images     |
| 📩 Twilio SMS Alerts      | Sends alert to predefined numbers on detection          |
| 📝 SQLite Logging         | Stores history of detections and alerts for review      |
| 🔐 Basic Security         | Handles file upload validations                         |

---

## 🖼️ System Architecture

```plaintext
User --> Flask Web App --> YOLOv8 Model --> Detection Result
                               ↓
                        Twilio SMS Alert
                               ↓
                           SQLite Log
