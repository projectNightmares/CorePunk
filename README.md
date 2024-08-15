# CorePunk - Mouse Position Capture & Auto Pin Creator


# User README for Mouse Position Capture Script
# (Feel free to use)

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
- Python (tons of 4 min vids on youtube)
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

# User README for Game Map Pin Placement Script

## Overview
This Python script automates the placement and deletion of pins on a game map. The script is designed to work with a game running on a 24inch 1080p (1920x1080) resolution screen. For accurate pin placement, ensure that the game map is zoomed in, centered on the screen, and that the character remains stationary.

## Key Features
- **Automated Pin Placement('`', 1, 2, 3, 4, 5) :** The script allows you to place various types of pins on the map at the position of the character.
- **Manual Pin Placement(6, 7, 8):** For these pins, open the map, move your mouse to the position of your choice, and click the key.
- **Pin Deletion(0):** The script can also delete pins that are positioned at the center of the screen. (Prolly won't work as intended, might need to modify it).

## Requirements
- **Python Libraries:** The script uses `pyautogui` and `pynput` libraries. Install them using pip:
  ```bash
  pip install pyautogui pynput
  ```

## How to Use
1. **Running the Script:**
   - Python (tons of 4 min vids on youtube)
   - Run the script in IDLE or another Python environment.
   - The script will start and listen for specific key inputs.

2. **Enable/Disable Macros:**
   - Press the `Shift` key to toggle the macros on or off.
   - When enabled, a message indicating "Macros enabled: ENABLED [TRUE]" will appear.
   - When disabled, "Macros enabled: DISABLED [FALSE]" will be shown.

3. **Automated Key Functions:**
   - **Grave (`) Key:** Places a green pin on the map.
   - **1 Key:** Place a green pin and types "Magic Tree" on the map.
   - **2 Key:** Places a green pin and types "Herb" on the map.
   - **3 Key:** Places a yellow pin on the map.
   - **4 Key:** Place a yellow pin and types "Tier Three."
   - **5 Key:** Places a red pin and marks it as a "Turtle" location.
   - **6 Key:** Allows manual placement of a purple pin marked as "BMS."
   - **7 Key:** Allows manual placement of a purple pin marked as "Wolves."
   - **8 Key:** Allows manual placement of a purple pin marked as "Imps."
   - **0 Key:** Deletes the pin located at the center of the screen.

## Important Usage Notes
- **Map Positioning:** The game map must be precisely centered on the screen and zoomed in for the script to function correctly.
- **Screen Resolution:** This script has been tested on a 1080p (1920x1080) screen resolution. Ensure your screen matches this resolution for accurate performance. Otherwise, use the Pixel_Position_Helper to modify the x,y values. 
- **Character Stationary:** Ensure that your in-game character remains stationary when placing pins to avoid inaccuracies.

## Manual Pin Placement
For manual pin placement (`6`, `7`, and `8` keys):
- Open the map.
- Move your mouse to the desired location on the map.
- Press the respective key (`6`, `7`, or `8`) to place the pin.

## Script Details
- **`move_and_click(x, y)`:** Moves the mouse to the specified (x, y) coordinates and clicks.
- **`press_key(key)`:** Simulates pressing a keyboard key.
- **`type_and_enter(text)`:** Types the specified text and presses Enter.
- **`delete_only()`:** Deletes the pin located at the center of the screen.

## Troubleshooting
- **Incorrect Pin Placement:** Ensure your screen resolution is set to 1920x1080 and that the game map is centered and zoomed in. Otherwise, use the Pixel_Position_Helper to modify the x,y values. 
- **Macros Not Triggering:** Verify that macros are enabled by pressing the `Shift` key and checking the status message.

## Conclusion
This script automates the process of marking locations on a game map, making it easier to track important points of interest. Ensure that your screen setup matches the required resolution and that your game map is properly positioned for optimal results.
