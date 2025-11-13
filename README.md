# Real-Time Driver Drowsiness Detection System

This project is a computer vision-based system built with Python, OpenCV, and Keras/TensorFlow to monitor a driver's eyes in real-time. It is designed to prevent accidents by detecting signs of driver fatigue and triggering an immediate audio-visual alert.

The core of the system monitors the driver's **Eye Aspect Ratio (EAR)**. When the calculated EAR drops below a specific threshold for a set number of frames, the system concludes the driver is drowsy and activates an alarm.

---

## Tech Stack

* **Language:** Python
* **Core Libraries:** OpenCV (for real-time video capture and processing)
* **Machine Learning:** Keras with TensorFlow (for building and training the model)
* **Facial Landmarks:** dlib (for real-time facial landmark detection)
* **Data Handling:** NumPy (for numerical operations)


## What I Learned (Project Highlights)

This project was a deep dive into building an end-to-end computer vision pipeline. The key skills I developed were:

* **Machine Learning Implementation:** Successfully implemented and trained a Convolutional Neural Network (CNN) to classify eye states (open vs. closed).
* **Computer Vision:** Gained hands-on experience using OpenCV to capture video, process images, and draw contours and text on-screen in real-time.
* **Algorithm Development:** Researched and implemented the Eye Aspect Ratio (EAR) formula from a scientific paper, translating academic theory into a practical, working algorithm.
* **Problem-Solving:** Managed the challenge of integrating a high-speed video feed with a predictive ML model, all while running in a single, responsive application.


**Note:** The large trained model file (e.g., `.h5` or `.dat`) is not included in this repository due to GitHub's file size limits. The scripts `project2.py` contain the core logic for running and training the model.
## Install dependencies:
* **pip install opencv-python dlib numpy imutils**
* **Download the dlib facial landmark predictor:** **File: shape_predictor_68_face_landmarks.dat*
**Extract and place it in the project directory.**
## Usage:
* **Run the script with:** python project2.py

* **Make sure your webcam is enabled. The system will start detecting your eyes and trigger an alert if drowsiness is detected.**
