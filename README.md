# Real-Time Face and Eye Detection

This project demonstrates **real-time face and eye detection** using Python and OpenCV. It uses pre-trained Haar cascades to detect faces and eyes from a webcam feed and highlights them with rectangles.

## Features

- Detects faces in real-time using `haarcascade_frontalface_default.xml`
- Detects eyes within detected faces using `haarcascade_eye.xml`
- Draws rectangles around detected faces (blue) and eyes (green)
- Works on a live webcam feed

## Demo

When you run the program, a window will open showing the webcam feed with:

- **Blue rectangles** around detected faces
- **Green rectangles** around detected eyes

Press `Esc` to exit the application.

## Requirements

- Python 3.x
- OpenCV (`opencv-python`)
- NumPy

## Usage

Make sure the Haar cascade XML files are in the same directory:

haarcascade_frontalface_default.xml

haarcascade_eye.xml

**Run the script:**

python face_eye_detection.py

The webcam feed will open, detecting faces and eyes in real-time. Press Esc to close.

## How It Works

Captures video frames from the webcam.

Converts each frame to grayscale.

Uses the face cascade to detect faces in the grayscale image.

For each detected face, uses the eye cascade to detect eyes within the face region.

Draws blue rectangles around detected faces and green rectangles around detected eyes on the original colored frame.

Continuously updates the display in real-time until the user presses Esc.

## References

OpenCV Haar Cascades: https://github.com/opencv/opencv/tree/master/data/haarcascades

**Clone the repository:**

````markdown
git clone <https://github.com/Rou-maissa/Face_eye_detection.git>
