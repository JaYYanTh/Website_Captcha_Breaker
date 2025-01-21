# Website_Captcha_Breaker
Python Script for Brute-Forcing and CAPTCHA Breaking
This Python script demonstrates a proof-of-concept for brute-forcing usernames and passwords on a login page. It also includes functionality to bypass CAPTCHA challenges using automation tools. However, this script works only when modified and configured for a specific target system, ensuring that the coordinates, browser settings, and logic align with the intended setup.

Key Features:
Brute-Forcing:

Automates attempts to try different username and password combinations.
Uses a list of predefined credentials for testing purposes.
CAPTCHA Handling:

Utilizes Selenium to automate browser interactions and handle CAPTCHA challenges.
Leverages Google Lens to analyze and save CAPTCHA images.
Automates CAPTCHA entry into the designated input field.
Automation via PyAutoGUI:

Simulates mouse clicks and keyboard inputs for seamless interaction with the login interface.
Tools and Libraries:
PyAutoGUI: Handles mouse and keyboard automation for clicking specific regions on the screen.
Selenium: Automates browser operations, such as opening a page, interacting with input fields, and handling CAPTCHA analysis.
Google Lens API (or similar OCR tool): Decodes CAPTCHA images to text, which is then submitted in the input field.
How It Works:
Setup:

The script launches the login page using Selenium.
Initializes PyAutoGUI for clicking predefined regions on the screen.
Brute-Forcing:

Loops through a list of potential usernames and passwords.
Submits each pair via automated form interaction.
CAPTCHA Decoding:

Captures the CAPTCHA image using Selenium’s screenshot functionality.
Opens the Google Lens API (or equivalent) to decode the CAPTCHA.
Pastes the decoded text back into the CAPTCHA field.
Iteration:

Repeats the brute-forcing process until successful login or completion of the credential list.
Disclaimer:
This script is intended for educational purposes only to understand how brute-forcing and CAPTCHA handling work in ethical, controlled environments. It should never be used for unauthorized access or malicious purposes, as doing so is illegal and unethical. Always obtain proper authorization before testing any system.
