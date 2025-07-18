# Virtual Steering Wheel and Racing Controller

This application provides a virtual Xbox 360 controller on your Windows PC, allowing you to map numpad keys for steering and other keyboard keys for essential racing game controls. It features a simple graphical user interface (GUI) for custom keybinding setup and can be packaged into a standalone executable.

## Features

* **Numpad Steering Wheel:** Maps numpad keys (1, 4, 7, 8, 9, 6, 3) to a virtual steering axis, providing granular control from full left to full right.

* **Basic Racing Controls:** Includes default mappings for acceleration, braking, gear shifting, handbrake, horn, and lights toggle.

* **Custom Keybinds:** A user-friendly GUI allows you to easily reassign any control to your preferred keyboard key. This version uses hardware scan codes for robust key detection, ensuring numpad keys and others are correctly recognized regardless of NumLock state or keyboard layout.

* **Standalone Executable:** The application can be compiled into a portable `.exe` file, so you don't need Python installed on the target machine.

## Controls Mapping

By default, the following controls are mapped:

| **Action** | **Default Key** | **Virtual Controller Output** |
| :---------------- | :---------- | :----------------------------------------- |
| **Steering** | | (Left Joystick X-axis) |
| Full Left | `Numpad 1` | -1.0 |
| Mid Left | `Numpad 4` | -0.66 |
| Slight Left | `Numpad 7` | -0.33 |
| Center | `Numpad 8` | 0.0 |
| Slight Right | `Numpad 9` | 0.33 |
| Mid Right | `Numpad 6` | 0.66 |
| Full Right | `Numpad 3` | 1.0 |
| **Acceleration** | `W` | Right Trigger (Analog) |
| **Brake** | `S` | Left Trigger (Analog) |
| **Gear Up** | `E` | Right Shoulder Button |
| **Gear Down** | `Q` | Left Shoulder Button |
| **Handbrake** | `Spacebar` | A Button |
| **Horn** | `Numpad 5` | X Button |
| **Lights Toggle** | `Numpad *` | Y Button (toggles on/off state) |

## Prerequisites

Before running or building the application, ensure you have:

* **Python 3.x:** Installed on your system.

* **Administrator Privileges:** Required to install the `vgamepad` driver and run the application, as it creates a virtual device.

## **Using the GUI:**

    * The application window will appear.

    * Click the "Start Controller" button to activate the virtual gamepad.

    * To change a keybind, click the "Change" button next to the action you wish to modify. A prompt will appear, and you simply press the desired key on your keyboard. The new keybind (including its reliable scan code) will be saved automatically.

    * Click "Stop Controller" to deactivate the virtual gamepad.

    * Close the window to exit the application.
