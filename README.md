Overview:

The Drowsiness Detection System is a computer vision–based project that monitors a driver’s alertness in real time. It uses OpenCV and dlib to detect facial landmarks and calculate the Eye Aspect Ratio (EAR), determining if the driver’s eyes remain closed for an extended period which is a strong sign of drowsiness. When detected, the system triggers an audio alert to wake the driver and prevent accidents caused by fatigue.

How It Works:

The webcam captures live video of the driver’s face.

dlib’s 68-point facial landmark detector identifies eye coordinates.

The Eye Aspect Ratio (EAR) is computed using distances between specific eye landmarks.

If the EAR value stays below a threshold for a certain number of frames, the system classifies it as drowsiness.

An audio alert plays to warn the driver.

Tech Stack:

Python 3.x

OpenCV – Real-time image and video processing

dlib – Facial landmark detection

NumPy – Numerical computation

Features:

Real-time face and eye detection

EAR-based drowsiness detection logic

Instant audio alerts for safety

Adjustable sensitivity (EAR threshold & frame count)

Lightweight and efficient

Installation:

Clone this repository:

git clone https://github.com/yourusername/drowsiness-detection-system.git
cd drowsiness-detection-system


Install dependencies:

pip install opencv-python dlib numpy imutils

Download the dlib facial landmark predictor:

File: shape_predictor_68_face_landmarks.dat

Download link: Dlib Model Download

Extract and place it in the project directory.

Usage:  

Run the script with:

python project2.py

Make sure your webcam is enabled. The system will start detecting your eyes and trigger an alert if drowsiness is detected.
