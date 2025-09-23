
# Drowsiness Detection System

A real-time driver drowsiness and distraction detection system built with Python, OpenCV, and MediaPipe. The system monitors a driver's facial landmarks to detect signs of fatigue and sends alerts to a Firebase-powered dashboard.

## ✨ Features

- **Real-Time Drowsiness Detection:** Monitors Eye Aspect Ratio (EAR) to detect closed eyes.
- **Yawn Detection:** Monitors Mouth Aspect Ratio (MAR) to identify yawns.
- **Distraction Detection:** Uses head pose estimation to check if the driver is looking away from the road.
- **Fatigue Score:** Calculates a cumulative fatigue level based on events.
- **Firebase Integration:** Sends real-time SOS alerts with GPS coordinates to a Flutter dashboard app.
- **Audible Alerts:** Plays warning sounds and voice alerts ("Wake up," "Pay Attention").

## ⚙️ Setup

To run this project, you need to set up the Python environment and Firebase.

1.  **Clone the repository:**
    `git clone <your-repository-url>`

2.  **Install the required libraries:**
    `pip install -r requirements.txt` 
    *(Note: You will need to create a `requirements.txt` file for this to work)*

3.  **Set up Firebase:**
    - Create a Firebase project in the Firebase Console.
    - Go to Project Settings > Service accounts.
    - Click "Generate new private key" to download your `serviceAccountKey.json` file.
    - **Important:** Place this file in the project's root directory but do not commit it to Git. The `.gitignore` file is already configured to ignore it.

## ▶️ How to Run

1.  Make sure your webcam or DroidCam stream is active.
2.  Run the main Python script from your terminal:
    `python main.py`

The application will start, calibrate, and begin monitoring. Press 'q' to quit the program.
