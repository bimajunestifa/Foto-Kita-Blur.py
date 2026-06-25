# ✌️ Peace Blur Detector

A Computer Vision project that automatically blurs the webcam feed when a peace sign (✌️) is detected.

Built using Python, OpenCV, and MediaPipe.

---

## 📌 Overview

Peace Blur Detector is a real-time hand gesture recognition project that uses MediaPipe Hand Tracking and OpenCV image processing. When the system detects a peace sign gesture, the webcam view is automatically blurred.

This project was created as a learning project to explore Computer Vision, hand gesture recognition, and real-time image processing with Python.

---

## ✨ Features

* Real-time webcam detection
* Peace sign (✌️) recognition
* Automatic blur effect
* Fast and lightweight processing
* Beginner-friendly code structure
* Built with modern Computer Vision tools

---

## 🛠️ Requirements

### Recommended

* Python 3.11.x
* Webcam
* Windows 10/11

### Important

This project uses the MediaPipe Solutions API:

```python
mp.solutions.hands
```

For compatibility reasons, it is recommended to use:

* Python 3.11
* MediaPipe 0.10.14

Python 3.14 and newer versions may cause compatibility issues with MediaPipe.

---

## 📦 Installation

Clone this repository:

```bash
git clone https://github.com/bimajunestifa/Foto-Kita-Blur.git
cd Foto-Kita-Blur
```

Create a virtual environment (recommended):

```bash
py -3.11 -m venv venv
venv\Scripts\activate
```

Install dependencies:

```bash
py -3.11 -m pip install --upgrade pip
py -3.11 -m pip install -r requirements.txt
```

If you do not use requirements.txt:

```bash
py -3.11 -m pip install mediapipe==0.10.14
py -3.11 -m pip install opencv-python
```

---

## 📄 requirements.txt

Create a file named `requirements.txt`:

```txt
mediapipe==0.10.14
opencv-python
numpy
```

---

## ▶️ Run the Project

```bash
py -3.11 blur.py
```

If you are using VS Code:

1. Press `Ctrl + Shift + P`
2. Select `Python: Select Interpreter`
3. Choose Python 3.11

Press `ESC` to close the application.

---

## 📖 How It Works

1. The webcam captures live video.
2. MediaPipe detects hand landmarks.
3. The program analyzes finger positions.
4. When a peace sign (✌️) is detected:

   * The camera feed is blurred automatically.
5. When the gesture disappears:

   * The video returns to normal.

---

## ❗ Troubleshooting

### Error: No module named 'mediapipe'

Install MediaPipe:

```bash
py -3.11 -m pip install mediapipe==0.10.14
```

### Error: module 'mediapipe' has no attribute 'solutions'

Make sure MediaPipe version is:

```bash
py -3.11 -m pip show mediapipe
```

Expected output:

```txt
Version: 0.10.14
```

If not:

```bash
py -3.11 -m pip uninstall mediapipe -y
py -3.11 -m pip install mediapipe==0.10.14
```

### Webcam does not open

Make sure:

* Webcam is connected
* No other application is using the camera
* Camera permissions are enabled in Windows

---

## 🎯 Learning Objectives

This project was developed to learn:

* Computer Vision fundamentals
* Hand tracking with MediaPipe
* Image processing using OpenCV
* Real-time video analysis
* Python application development

---

## 👨‍💻 About the Developer

Hi, I'm **Bima Junestifa**.

An SMK student majoring in Software and Game Development (PPLG) who enjoys learning and building projects in:

* Python Programming
* Cybersecurity
* Computer Vision
* Web Development
* Open Source Development

This project is part of my learning journey and portfolio as a student developer.

---

## 📬 Contact

Instagram: @bima_junestifa17

GitHub: https://github.com/bimajunestifa

---

## 📄 License

This project is open-source and intended for educational and learning purposes.

---

⭐ If you found this project useful, consider giving it a star and sharing it with others.
