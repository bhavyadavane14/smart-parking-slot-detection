# Smart Parking Slot Occupancy Detection using YOLOv8

AI-powered parking slot occupancy detection system built using YOLOv8, Computer Vision, and Deep Learning.  
This project detects whether parking slots are occupied or empty using custom-trained object detection models and real-time webcam monitoring.

---

# Project Overview

The goal of this project is to automate parking slot monitoring using Artificial Intelligence and Computer Vision techniques.  

The system was trained on a custom dataset of parking slot images collected manually and processed through augmentation and annotation techniques.  
The trained YOLOv8 model was then deployed for real-time detection using mobile camera streaming through IP Webcam.

---

# Features

- Parking Slot Occupancy Detection
- Custom YOLOv8 Model Training
- Image Augmentation
- Image Annotation
- Real-Time Detection
- Mobile Camera Integration
- IP Webcam Streaming
- Deep Learning-based Object Detection
- Google Colab Training Pipeline

---

# Technologies Used

- Python
- YOLOv8
- Ultralytics
- OpenCV
- PyTorch
- Roboflow
- Google Colab
- IP Webcam
- Computer Vision
- Deep Learning

---

# Workflow

## 1. Dataset Collection
- Captured parking slot images manually
- Collected images for:
  - Occupied Slots
  - Empty Slots

## 2. Image Augmentation
Performed augmentation techniques to increase dataset diversity:
- Rotation
- Flipping
- Brightness Adjustment
- Scaling
- Cropping

## 3. Annotation
- Annotated images using Roboflow
- Created bounding boxes for parking slots
- Exported dataset in YOLOv8 format

## 4. Model Training
- Trained custom YOLOv8 model using Google Colab
- Used GPU acceleration with Tesla T4
- Fine-tuned model on custom parking dataset

## 5. Model Deployment
- Exported trained `.pt` model
- Integrated model into mobile application
- Connected mobile camera using IP Webcam

## 6. Real-Time Testing
- Performed real-time parking occupancy detection
- Tested live webcam stream detection

---

# Project Structure

```bash
smart-parking-slot-detection/
│
├── notebooks/
│   └── parking_slot_occupancy01.ipynb
│
├── scripts/
│   ├── detect.py
│   └── ip_webcam_detection.py
│
├── models/
│   └── best.pt
│
├── images/
│   ├── annotations/
│   ├── predictions/
│   └── samples/
│
├── requirements.txt
├── README.md
└── .gitignore
