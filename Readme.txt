# Smart SRD Analysis – Student Dress Code Detection System

Smart SRD Analysis is an AI-based student dress code detection system that uses computer vision to identify whether a student follows basic dress code requirements. The system can analyze uploaded images and also supports real-time detection through webcam streaming.

## Project Overview

This project was developed to detect student dress code compliance using object detection. The system identifies key attire components such as collar, lanyard, and shoes. Based on the detection result, the system displays whether the student is **compliant** or **not compliant**.

## Features

- Upload a student image for dress code analysis
- Real-time webcam-based detection
- Detects collar, lanyard, and shoes
- Displays annotated detection results
- Shows final compliance status
- Web-based interface using Flask
- YOLOv8 object detection model integration

## Tech Stack

- Python
- Flask
- YOLOv8
- Ultralytics
- OpenCV
- HTML
- CSS

## Detection Components

The system checks for the following dress code items:

- Collar
- Lanyard / Student ID
- Shoes

A student is considered compliant when all required items are detected.

## Project Structure

```txt
srd-detection/
│
├── app.py
├── srd_infer.py
├── requirements.txt
├── README.md
│
├── templates/
│   └── index.html
│
├── static/
│   ├── uploads/
│   └── results/
│
├── test_images/
│
└── runs/
    └── detect/
        └── trained_model_weights/
