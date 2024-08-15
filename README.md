# CorePunk

# User README for Mouse Position Capture Script

## Overview
This Python script is designed to capture the screen's X, Y pixel positions whenever a mouse click is registered. It is particularly useful for scenarios where you need to log or track specific screen coordinates during user interactions.

## Purpose
The primary purpose of this script is to capture and display the X, Y pixel positions on the screen when the mouse is clicked. The script is triggered by pressing a specific key (`v`) and works seamlessly when executed in the Python Integrated Development and Learning Environment (IDLE).

## How to Use
1. **Running the Script:**
   - Open the script in IDLE.
   - Execute the script by pressing `F5` or selecting "Run" from the IDLE menu.

2. **Starting the Capture:**
   - Press the `v` key on your keyboard. This will start the capture process.
   - Once activated, every mouse click on the screen will print the X, Y coordinates of the cursor at the time of the click.

3. **Stopping the Capture:**
   - Press the `v` key again to stop capturing mouse positions.

## Key Features
- **Toggle Capture:** The capture process can be toggled on and off by pressing the `v` key.
- **IDLE Compatibility:** The script is optimized to run within IDLE, ensuring that output is correctly displayed in the IDLE console.
- **Real-Time Feedback:** When running in IDLE, the script provides real-time feedback, indicating when the capture process starts and stops.

## Requirements
- **Python Libraries:** The script requires the following Python libraries:
  - `pyautogui`
  - `pynput`

  These can be installed using pip:
  ```bash
  pip install pyautogui pynput
  ```

## Script Details
- **`on_click(x, y, button, pressed)`:** A callback function that prints the X, Y coordinates when a mouse button is pressed.
- **`on_press(key)`:** A callback function that toggles the capturing state when the `v` key is pressed.
- **`main()`:** The entry point of the script, setting up the keyboard listener and providing user instructions.

## Notes
- **Running in Non-IDLE Environments:** The script is designed to work best in IDLE. If running in a different environment, the output may not display as intended.

## Troubleshooting
- **No Output in Console:** Ensure you are running the script in IDLE. The output is optimized for the IDLE environment.
- **Dependencies Missing:** If you encounter errors related to `pyautogui` or `pynput`, ensure they are installed correctly using pip.

## Conclusion
This script is a simple yet effective tool for capturing screen coordinates via mouse clicks. It provides an easy-to-use interface for toggling capture on and off, with clear output in the IDLE environment.
