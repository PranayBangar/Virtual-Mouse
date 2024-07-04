# Virtual-Mouse
Mouse Control using Hand Gestures
This project uses computer vision to control the mouse cursor with hand gestures. It leverages OpenCV, MediaPipe, PyAutoGUI, and Pynput libraries to achieve real-time hand tracking and cursor control.

Features
Hand Tracking: Detects and tracks the hand using MediaPipe.
Mouse Control: Moves the mouse cursor based on the position of the index finger tip.
Gesture Detection: Includes utility functions to calculate angles and distances for more complex gesture detection.
Requirements
Python 3.6+
OpenCV
MediaPipe
PyAutoGUI
Pynput
Installation
Install the required libraries using pip:

sh
pip install opencv-python mediapipe pyautogui pynput
Usage
Run the Jupyter notebook to start the hand tracking and mouse control:

sh
jupyter notebook mouse_2_project.ipynb
Alternatively, you can convert the notebook to a Python script and run it:

sh
jupyter nbconvert --to script mouse_2_project.ipynb
python mouse_2_project.py
Project Structure
mouse_2_project.ipynb: Jupyter notebook containing the code for hand tracking and mouse control.
Utility functions:
get_angle: Calculates the angle between three points.
get_distance: Calculates the distance between two landmarks.
find_finger_tip: Finds the index finger tip from hand landmarks.
move_mouse: Moves the mouse cursor based on the index finger tip position.
How it Works
Initialize: The project initializes the hand tracking model and sets up screen dimensions.
Capture Frames: Captures video frames from the webcam.
Process Frames: Converts frames to RGB and processes them using MediaPipe to detect hand landmarks.
Move Cursor: Moves the mouse cursor based on the position of the index finger tip.
Contributing
Feel free to open issues or submit pull requests if you find any bugs or have suggestions for improvements.

License
This project is licensed under the MIT License.

