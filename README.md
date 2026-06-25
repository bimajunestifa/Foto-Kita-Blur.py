# ✌️ Peace Blur Detector

A Computer Vision project that automatically blurs the webcam feed when a peace sign (✌️) is detected.

Built with Python, OpenCV, and MediaPipe.

---

## Features

* Real-time webcam detection
* Peace sign (✌️) recognition
* Automatic blur effect
* Lightweight and beginner-friendly
* Works with a standard webcam

---

## Requirements

Before running the project, make sure you have:

* Python 3.11.x
* Webcam
* Windows 10/11

> ⚠️ This project was tested with **Python 3.11** and **MediaPipe 0.10.14**. Newer Python versions may cause compatibility issues.

---

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/bimajunestifa/Foto-Kita-Blur.git
cd Foto-Kita-Blur
```

### 2. Install dependencies

```bash
py -3.11 -m pip install -r requirements.txt
```

### 3. Run the project

```bash
py -3.11 blur.py
```

Press **ESC** to exit.

---

## requirements.txt

```txt
mediapipe==0.10.14
opencv-python
numpy
```

---

## Troubleshooting

### Error: No module named 'mediapipe'

Install MediaPipe manually:

```bash
py -3.11 -m pip install mediapipe==0.10.14
```

### Error: module 'mediapipe' has no attribute 'solutions'

You are using the wrong MediaPipe version.

Remove the current version:

```bash
py -3.11 -m pip uninstall mediapipe -y
```

Install the supported version:

```bash
py -3.11 -m pip install mediapipe==0.10.14
```

### Black Camera Window

Try changing:

```python
cap = cv2.VideoCapture(0)
```

to:

```python
cap = cv2.VideoCapture(0, cv2.CAP_DSHOW)
```

### CameraReservedByAnotherApp Error

Another application is currently using the camera.

Close:

* Discord
* Zoom
* Google Meet
* OBS Studio
* Camera App

Then run the program again.

---

## How It Works

1. Webcam captures video.
2. MediaPipe detects hand landmarks.
3. The program checks finger positions.
4. If a peace sign (✌️) is detected:

   * Blur effect is enabled.
5. If the gesture disappears:

   * Video returns to normal.

---

## Developer

**Bima Junestifa**

* SMK Student (Software and Game Development)
* Python Developer
* Computer Vision Enthusiast
* Cybersecurity Learner

Instagram: @bima_junestifa17

GitHub: https://github.com/bimajunestifa

---

## License

This project is open-source and intended for educational purposes.

⭐ Don't forget to star this repository if you like the project!
