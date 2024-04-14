# aircanvas

1)Imports:
    OpenCV (cv2): Main library for computer vision tasks.
    NumPy (np): Used for numerical operations.
    Mediapipe (mediapipe): Provides tools for building various types of AI-powered solutions.
    deque from collections: A deque is used as a queue with a maximum length for storing color points.
    pytesseract: A Python wrapper for Google's Tesseract-OCR Engine. However, it's not used in this code.

2)Initialization: 
    Deques are initialized to store points for different colors.
    Index variables are set for each color.A kernel is defined for dilation purposes.Color information and index are initialized.
    The main window for drawing (paintWindow) is created and configured with rectangles and text for different color options.

3)Mediapipe Setup:
    The code sets up hand landmark detection using the Mediapipe library.

4)Webcam Initialization:
  T  he webcam feed is captured and processed frame by frame.

5)Main Loop:
    Within the loop, frames are read from the webcam.
    Landmark detection is performed on each frame.
    Hand landmarks are processed, and finger positions are determined.
    Based on finger positions, the application responds to commands like changing colors or clearing the canvas.
    Drawing on the canvas is done by detecting the position of the hand and using it as a pointer.
    Lines are drawn on both the frame and the canvas based on the movement of the hand.

6)Display:
    The modified frame and the canvas are displayed in separate OpenCV windows.

7)Termination:
    The loop continues until the 'q' key is pressed, upon which the webcam feed is released, and all OpenCV windows are destroyed.
