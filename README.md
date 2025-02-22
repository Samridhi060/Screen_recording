# Screen Recorder

A simple screen recording script that captures your screen and saves it as an MP4 video file using OpenCV and PyAutoGUI.

## Requirements

Before running the script, ensure you have the following Python packages installed:

- `opencv-python`
- `pyautogui`
- `numpy`
- `pywin32`

You can install the required packages using pip:

## Code Explanation

- **Imports**:
  - `cv2`: Used for video processing.
  - `pyautogui`: Used for taking screenshots.
  - `numpy`: Used for array manipulation.
  - `win32api`: Used to get the screen dimensions.
  - `time`: Used for timing the recording duration.

- **Screen Dimensions**:
  - The script retrieves the width and height of the screen using `GetSystemMetrics`.

- **Video Writer**:
  - The script initializes a video writer object with the specified codec (XVID) and frame rate (30 FPS).

- **Recording Loop**:
  - The script takes screenshots in a loop and writes them to the video file until the specified duration is reached.

- **Release Resources**:
  - Once the recording is complete, the script releases the video writer resources.

## Notes

- Make sure to run the script in an environment where you have permission to capture the screen.
- The output video file will be saved in the same directory as the script.
