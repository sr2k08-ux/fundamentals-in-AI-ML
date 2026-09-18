# 🎨 AI Finger Painting

> An interactive painting application that allows users to create digital artwork using their fingers through a real-time webcam.

## 📌 Project Overview

AI Finger Painting is a computer vision project that allows users to draw on a virtual canvas without using a mouse, keyboard, or touchscreen.

The application uses a real-time camera to capture the user's hand movements and detect finger positions. The finger acts as a virtual brush, allowing users to draw directly on the screen.

OpenCV is used for webcam access and image processing, while hand-tracking technology detects the position and movement of the fingers. The project demonstrates how artificial intelligence and computer vision can be combined to create an interactive and touchless digital painting experience.

## ✨ Features

* 🖐️ Real-time finger tracking
* 🎨 Drawing using finger movements
* 📷 Live webcam-based interaction
* 🖌️ Virtual canvas painting
* ✍️ Smooth digital brush strokes
* 🧠 Hand landmark detection
* 🧹 Canvas clearing functionality
* 🎨 Interactive and touchless painting
* ⚡ Real-time camera processing

## 🧰 Technologies Used

| Technology | Purpose                             |
| ---------- | ----------------------------------- |
| Python     | Main programming language           |
| OpenCV     | Webcam access and image processing  |
| MediaPipe  | Hand and finger tracking            |
| NumPy      | Virtual canvas and image operations |

## 📂 Project Structure

```text
AI-Finger-Painting/
│
├── ai_finger_painting.py
├── README.md
└── requirements.txt
```

## ⚙️ Installation

### Step 1: Install Python

Install Python on your computer.

Check your Python version:

```bash
python --version
```

Python 3.10 or 3.11 is recommended for compatibility with the required libraries.

### Step 2: Install Required Libraries

Open Command Prompt or the VS Code terminal and run:

```bash
pip install opencv-python mediapipe numpy
```

If a `requirements.txt` file is available, you can install all dependencies using:

```bash
pip install -r requirements.txt
```

## ▶️ How to Run the Project

Open the project folder in VS Code or Command Prompt.

Run the Python file:

```bash
python ai_finger_painting.py
```

After running the program, the webcam will open automatically.

Make sure your hand is visible in front of the camera. Move your finger to interact with the virtual canvas and create your painting.

## 🎮 Controls

| Action          | Control                                             |
| --------------- | --------------------------------------------------- |
| Draw            | Move your finger on the screen                      |
| Select/Interact | Use the detected finger position                    |
| Clear Canvas    | Use the clear option/key implemented in the program |
| Exit            | Use the exit option/key implemented in the program  |

> The exact controls may vary depending on the implementation of the Python program.

## 🖐️ How the Project Works

The project works through the following steps:

1. The webcam captures live video.
2. OpenCV reads the camera frames.
3. The video frame is processed in real time.
4. MediaPipe detects the user's hand.
5. Hand landmarks are identified.
6. The position of the finger is determined.
7. The finger position is treated as the virtual brush position.
8. The program tracks the movement of the finger.
9. OpenCV draws strokes according to the finger movement.
10. The strokes are stored on a virtual canvas.
11. The canvas is displayed together with the live camera feed.
12. The user can continue moving their finger to create digital artwork.

## ☝️ Finger Tracking

MediaPipe detects important landmark points on the hand.

The application can use the detected finger-tip position as the brush location.

For example:

| Finger Point        | Landmark ID |
| ------------------- | ----------: |
| Index Finger Tip    |           8 |
| Index Finger Joint  |           6 |
| Middle Finger Tip   |          12 |
| Middle Finger Joint |          10 |

The program uses these landmarks to understand finger positions and movements.

### Drawing

When the required finger gesture is detected, the application starts drawing.

The current finger position is connected with the previous position to create a continuous digital stroke.

### Erasing

If an erasing gesture is implemented, the application can use a different finger gesture to remove existing strokes from the canvas.

## 📸 Example Output

When the program starts, the webcam displays a live camera feed.

The user can place their hand in front of the camera and move their finger across the screen. The detected finger acts as a virtual brush, and the movement creates digital strokes on the virtual canvas.

The final output is an interactive webcam window containing the live camera feed and the user's digital painting.

## ⚠️ Requirements

The project requires:

* A computer or laptop
* Python installed
* A working webcam
* OpenCV
* MediaPipe
* NumPy
* Proper lighting

Good lighting helps the hand-tracking system detect the user's fingers more accurately.

The hand should remain clearly visible inside the webcam frame.

## 🛠️ Possible Improvements

The current project can be extended with additional painting and computer vision features.

Possible improvements include:

* 🌈 Multiple brush colours
* 🖌️ Adjustable brush size
* 🧽 Improved eraser
* 💾 Save paintings as image files
* ↩️ Undo and redo functionality
* 🎨 Colour selection using hand gestures
* 🔷 Automatic shape recognition
* 🖼️ Background image support
* 🖐️ Multiple-hand tracking
* 🧑‍🎨 Different brush styles
* ✨ Special drawing effects
* 🗂️ Drawing tools menu
* 📱 Improved user interface

## 🐞 Troubleshooting

### Webcam Not Opening

The webcam may not open if another application is currently using the camera or if camera permissions are disabled.

Try the following:

* Check that the webcam is connected.
* Close other applications using the camera.
* Enable camera permissions.
* Restart the program.

If necessary, try changing the camera index:

```python
cap = cv2.VideoCapture(0)
```

If you have multiple cameras, you may need to try another camera index.

### MediaPipe Installation Error

Make sure you are using a compatible Python version and that MediaPipe is installed correctly.

Try:

```bash
pip install mediapipe
```

### OpenCV or NumPy Error

Install the required libraries again:

```bash
pip install opencv-python numpy
```

### Black Screen

A black screen can occur because of camera permissions, an incorrect camera index, or another application using the webcam.

Check that:

* The webcam is working.
* Camera permission is enabled.
* Other camera applications are closed.
* The correct camera index is being used.

### Finger Tracking Is Not Accurate

Finger detection can become less accurate when the hand is difficult to see.

For better results:

* Use sufficient lighting.
* Keep your hand inside the camera frame.
* Keep your fingers clearly visible.
* Avoid very fast movements.
* Use a simple background.
* Maintain a suitable distance from the webcam.

## 📚 Learning Outcomes

Developing this project provides practical experience with computer vision, artificial intelligence, and real-time video processing.

The main concepts include:

* Accessing a webcam using OpenCV
* Processing real-time video frames
* Detecting hands using MediaPipe
* Tracking finger landmark positions
* Recognising hand movements
* Creating a virtual drawing canvas
* Drawing using finger coordinates
* Using NumPy for image processing
* Combining multiple Python libraries
* Building a real-time interactive application

This project demonstrates how computer vision can be used to create a touchless human-computer interaction system.

## 🎯 Use Cases

AI Finger Painting can be used for:

* 🎨 Digital drawing
* 🧑‍🏫 Interactive classroom demonstrations
* 📚 Educational projects
* 🖥️ Touchless computer interaction
* 🖌️ Gesture-based painting
* 🤖 Artificial intelligence demonstrations
* 👨‍💻 Computer vision learning
* 🧪 Real-time hand-tracking experiments
* 🎭 Interactive art applications

## 🔍 Core Concepts Used

* Computer Vision
* Artificial Intelligence
* Hand Gesture Recognition
* Finger Tracking
* Image Processing
* Real-Time Video Processing
* Hand Landmark Detection
* Virtual Canvas Creation
* Human-Computer Interaction
* Coordinate Tracking

## 👨‍💻 Author

**Name:** Your Name
**Course:** Computer Science / Artificial Intelligence
**Project:** AI Finger Painting
**Programming Language:** Python
**Technologies Used:** OpenCV, MediaPipe, NumPy
**Project Type:** Computer Vision and Artificial Intelligence

This project was developed as part of a learning experience in Python, artificial intelligence, and computer vision.

## 📜 License

This project is created for educational purposes.

You are free to study, modify, and improve the project for learning and experimentation.
