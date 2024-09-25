This repository contains a deep learning-based driver drowsiness detection system. The goal of this project is to enhance road safety by detecting signs of driver drowsiness and alerting the driver before accidents occur. The system leverages convolutional neural networks (CNN) for image classification and facial landmark detection to assess the driver’s level of alertness in real time.

Features:
Real-Time Monitoring: Continuously monitors the driver’s face through a live camera feed.
Facial Landmark Detection: Uses facial landmarks (such as eyes, mouth, and head pose) to detect signs of drowsiness.
Blinking and Yawning Detection: Measures blink duration and yawning frequency to determine fatigue levels.
Alert Mechanism: If drowsiness is detected, the system triggers an alert to notify the driver.
Technology Stack:
Deep Learning: Convolutional Neural Networks (CNN) for image classification.
OpenCV: For real-time video processing and facial detection.
TensorFlow/Keras: For building and training the deep learning models.
Dlib: For facial landmark extraction and feature tracking.
Python: Core programming language used for development.
Dataset:
The model is trained on publicly available datasets like UTA-RLDD and Mrl Eye Dataset that contain labeled images of drowsy and alert drivers.

How it Works:
Preprocessing: Captured video frames are preprocessed by extracting the region of interest (driver’s face).
Feature Extraction: Facial landmarks like eyes and mouth are extracted using dlib’s facial landmark predictor.
Model Prediction: The deep learning model classifies the driver’s state as either “Drowsy” or “Alert.”
Alert System: If the driver is detected to be drowsy for a certain threshold of time, the system triggers an alert.
Applications:
Vehicle Safety: Prevents accidents caused by driver fatigue.
Fleet Management: Used in commercial vehicle fleets to monitor driver alertness.
Consumer Vehicles: Can be integrated into cars for personal use.
Getting Started:
Clone the repository:
bash
Copy code
ghttps://github.com/777santosh/Driver-drowsiness-detection-using-deep-learning.git
Install the necessary dependencies:
bash
Copy code
pip install -r requirements.txt
Run the application:
bash
Copy code
python app.py
Contributing:
Feel free to submit pull requests to enhance the system or suggest new features. For major changes, please open an issue first to discuss what you would like to change.

License:
This project is licensed under the MIT License - see the LICENSE file for details.
