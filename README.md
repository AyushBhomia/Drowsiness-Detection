PERCLOS Drowsiness Detection System
This project implements a real-time drowsiness detection system using the PERCLOS metric (Percentage of Eye Closure). It uses computer vision techniques to monitor eye activity and triggers an alert when signs of drowsiness are detected.

Features
Real-time detection of facial landmarks and eye regions using Dlib.
Eye Aspect Ratio (EAR) calculation using Manhattan Distance.
PERCLOS calculation to measure eye closure over time.
Audio alert to notify users of drowsiness.
Full-screen display for user feedback with frame annotations.
Requirements
Python 3.x
OpenCV
Dlib
pyttsx3
Installation
Clone this repository:

bash
Copy code
git clone https://github.com/yourusername/drowsiness-detector.git
cd drowsiness-detector
Install the required dependencies:

bash
Copy code
pip install opencv-python dlib pyttsx3
Download the Dlib shape predictor file:

shape_predictor_68_face_landmarks.dat
Extract it and update the shape_predictor_path in the script to point to the .dat file.
Usage
Connect a camera to your system.

Run the script:

bash
Copy code
python output.py
The application will:

Detect your face and eyes.
Calculate the PERCLOS metric.
Alert you if drowsiness is detected.
Press Esc to exit the application.

File Structure
output.py: Main script for the PERCLOS drowsiness detection system.
shape_predictor_68_face_landmarks.dat: Pre-trained Dlib model for detecting facial landmarks (must be downloaded separately).
Key Functions
calculate_manhattan: Computes Manhattan Distance for EAR calculation.
PERCLOS_Detector: Class handling the PERCLOS metric and alerting logic.
trigger_alert: Triggers an audio alert when drowsiness is detected.
Screenshots
Add screenshots or GIFs showing the system in action.

Troubleshooting
Ensure your camera is properly connected and accessible by OpenCV.
Verify the path to shape_predictor_68_face_landmarks.dat.
If Dlib fails to load, check your system's compatibility and installation of prerequisites.
License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgments
Dlib for the facial landmark predictor.
OpenCV for real-time video processing.
