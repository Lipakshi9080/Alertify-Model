# 🔔 Alertify — Fire & Smoke Detection Model (YOLOv8)

Alertify is a real-time hazard detection system focused on **fire and smoke detection** using deep learning.  
This repository contains the **trained YOLOv8 model weights** used for testing and deployment.

---

## 🚀 Project Overview

Delayed detection of fire hazards can lead to severe loss of life and property.  
Alertify addresses this by using a **vision-based deep learning model** to automatically detect fire and smoke in real time and trigger alerts.

---

## 🧠 Model Details

- **Model Architecture:** YOLOv8 (Ultralytics)
- **Task:** Object Detection
- **Classes:**
  - `0` → Fire 🔥
  - `1` → Smoke 💨
- **Training Platform:** Google Colab (GPU)
- **Deployment Target:** Real-time systems / Edge devices

---

## 📊 Training Performance

After 25 epochs of training, the model achieved:

| Metric | Value |
|------|------|
| Precision | 98.3% |
| Recall | 97.0% |
| mAP@50 | 99.1% |
| mAP@50–95 | 93.8% |

These results demonstrate strong accuracy and suitability for **real-time hazard detection**.

---

## 📁 Repository Contents

---

## ▶️ How to Test the Model

1️⃣ Install YOLOv8
pip install ultralytics
2️⃣ Run Detection on an Image
yolo detect predict model=best.pt source=fire.jpg conf=0.4
3️⃣ Run Detection on a Video
yolo detect predict model=best.pt source=video.mp4 conf=0.4


