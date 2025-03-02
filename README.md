# Hand Gesture Recognition

This project uses OpenCV and MediaPipe to recognize hand gestures in real-time from your webcam feed. It processes each frame captured by the webcam, detects hand landmarks, and then classifies the gesture based on the hand landmarks. The recognized gesture is displayed on the screen with a label.

## Features
- Real-time hand gesture recognition using webcam.
- Recognizes multiple gestures, including:
  - Spiderman
  - What? (Confused gesture)
  - Thumbs Up
  - Peace
  - Fist
  - OK
  - Stop
  - Call Me
- Draws hand landmarks on the screen.

## Requirements
- Python 3.x
- OpenCV
- Mediapipe

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/ManasaMusunuri/Project-GestureCam.git
    cd hand-gesture-recognition
    ```

2. Install the required libraries:
    ```bash
    pip install opencv-python mediapipe
    ```

3. Run the program:
    ```bash
    python hand_gesture_recognition.py
    ```

## Usage

Once the program is running, it will open the webcam feed and display the camera view on the screen. The hand gestures will be recognized, and the corresponding label will be displayed on the screen near the hand. The recognized gestures include:
- **Spiderman**: When the index finger and the thumb are extended and the rest are folded.
- **What?**: When the thumb is extended and the index finger is pointed upwards.
- **Thumbs Up**: When the thumb is extended and other fingers are folded.
- **Peace**: When the index and middle fingers are extended in a "V" shape.
- **Fist**: When all fingers are clenched into a fist.
- **OK**: When the thumb and index finger form a circle.
- **Stop**: When all fingers are extended but slightly bent.
- **Call Me**: When the pinky and thumb are extended while the rest of the fingers are folded.

Press `q` to quit the application.

## How It Works

- **MediaPipe Hands**: MediaPipe is used to detect hand landmarks in real-time. It tracks the keypoints of the hand and provides coordinates of those points.
- **Gesture Recognition**: Based on the relative positions of the hand landmarks, the code classifies the hand gesture.
- **OpenCV**: OpenCV is used to capture the webcam feed and display the results.

## Contributing

Feel free to fork this repository and make contributions. To report bugs or request new features, please create an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
