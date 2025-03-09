
<img width="781" alt="Screenshot 2024-09-30 at 17 55 27" src="https://github.com/user-attachments/assets/6802b40c-6694-4046-a7f6-c14b2840126a">

![Screenshot 2025-03-09 at 17 42 48](https://github.com/user-attachments/assets/e3bcb6bc-0e81-4c80-ad4e-9424c113f4d5)




# Facial Recognition and Hand Tracking

This project uses computer vision techniques to perform real-time facial recognition, face mesh rendering, and hand tracking using a webcam feed.

## Features

- Face mesh detection and rendering
- Mouth landmark highlighting
- Hand tracking and landmark rendering
- Real-time processing of webcam feed

## Requirements

- Python 3.7+
- OpenCV
- MediaPipe

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/your-username/facial-recognition-hand-tracking.git
   cd facial-recognition-hand-tracking
   ```

2. Install the required packages:
   ```
   pip install opencv-python mediapipe
   ```

## Usage

Run the main script:

- The application will open your webcam feed and start detecting face meshes and hand landmarks.
- Press 'q' to quit the application.

## How it works

- The script uses MediaPipe's Face Mesh solution to detect and render facial landmarks.
- It specifically highlights mouth landmarks for easier tracking of mouth movements.
- Hand tracking is implemented using MediaPipe's Hands solution.
- All detections are rendered in real-time on the webcam feed.

## Customization

- Adjust the `min_detection_confidence` and `min_tracking_confidence` parameters in the `FaceMesh` and `Hands` initializations to balance between accuracy and speed.
- Modify the `MOUTH_LANDMARKS` list to highlight different facial features.
