# AirCanvas
AirCanvas is a virtual drawing application that uses computer vision and hand gesture recognition to enable touch-free drawing. Users can select colors and draw on a canvas using only their hands, captured through a webcam.

# Key Components
1. Imports
  OpenCV (cv2): For capturing webcam feed and processing frames.
  NumPy (np): For handling numerical operations.
  Mediapipe: For hand tracking and gesture detection.
  Deque (from collections): For managing color-specific points in the drawing queue.
2. Initialization
  Separate deques for different color points.
  Color and index initialization for easy switching between colors.
  Configured canvas (paintWindow) with color selection buttons for clear, blue, green,      red, and yellow.
3. Mediapipe Setup
  Uses Mediapipe’s hand tracking for detecting hand landmarks and interpreting gestures.
4. Webcam Feed
  Captures frames from the webcam, flips them for a mirrored view, and processes them in    real-time.
5. Main Drawing Loop
  Processes each frame to detect hand landmarks.
  Uses finger positions to interpret gestures for:
  Color Selection: Switch colors based on finger position over the color buttons.
  Clear Canvas: Erase the canvas by selecting the "CLEAR" button.
  Drawing: Tracks finger movement to draw lines on the canvas.
6. Display Output
  Displays the live drawing and color selection interface in separate OpenCV windows.
7. Termination
  Press the q key to exit, releasing the webcam and closing all windows.
# Usage
  1.Run the Script: Ensure you have the required libraries and launch the script.
  2.Interact with the Interface: Use hand gestures to draw, change colors, or clear the       canvas.
  3.Exit: Press q to close the application.
