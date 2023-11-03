# AI Virtual Keyboard

## Introduction
The AI Virtual Keyboard is an innovative application that allows users to interact with a virtual keyboard interface using hand gestures. This touchless typing solution leverages computer vision and hand tracking technology to capture gestures through a webcam, enabling users to type without physical contact with a keyboard.

## Features
- Real-time hand gesture recognition for typing
- Customizable keyboard layout with resizable buttons
- Visual feedback on key presses
- Special keys for functionalities like delete and clear

## Prerequisites
Before you begin, ensure you have met the following requirements:
- Python 3.6 or higher installed
- OpenCV library installed (`cv2` module)
- NumPy library installed
- HandTrackingModule (custom module for hand tracking)

## Installation
To install the AI Virtual Keyboard, follow these steps:
1. Clone the repository to your local machine:
   ```shell
   git clone https://github.com/raoofaltaher/aivirtualkeyboard.git




### Button Class
The Button class encapsulates the properties and behaviors of each key on the virtual keyboard:

### Position, size, and text on the button.
Drawing the button on the screen, with a gradient color or a solid color when clicked.
Detecting 'clicks' by checking if the hand is positioned over the button and if the click delay has passed since the last click.
Keyboard Initialization
The keyboard layout is defined in a list of lists, where each sublist represents a row of keys, including special function keys for deleting text and exiting the application. The initialize_keyboard function creates and positions these buttons according to the specified layout.

### Main Function
This is the entry point of the application, which:

Initializes the webcam and sets its properties.
Creates a HandDetector instance for tracking the user's hands.
Enters a loop to read frames from the webcam, detect hands, and process user interactions.
Draws the virtual keyboard, detects key presses based on hand positions, and updates the text area with the inputted text.
Provides the option to exit the application either by pressing an "EXIT" button or the 'q' key on the keyboard.
User Interaction
When the application is running, the user's hands are tracked in real-time.
The user can 'press' the virtual keys by positioning their hands over the keys, which is recognized by the hand detector and processed by the application.
The entered text is displayed at the bottom of the window in a text area.
Running the Application
To start the virtual keyboard, the main function needs to be invoked. If the script is executed directly (not imported), the main function will automatically run, launching the virtual keyboard interface.

### Conclusion
The AI Virtual Keyboard project is an interactive system that combines hand tracking with a virtual keyboard interface, allowing for a touch-free typing experience. It can be particularly useful in scenarios where touchless interaction is desired, such as interactive kiosks, augmented reality environments, or accessibility tools for users with mobility impairments.
