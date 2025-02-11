# SIMPLE KEYLOGGER

## DESCRIPTION
This is a basic keylogger built using Python and the `pynput` library. It logs all keystrokes and saves them in a file named `keylog.txt`. It is designed for educational and ethical use only. Unauthorized use of keyloggers is illegal and against ethical guidelines.

## Ethical Considerations
- Always Inform & Obtain Consent before using a keylogger.
- Use it in a Safe, Controlled Environment (e.g., personal system, ethical hacking labs).
- Do Not Store Sensitive Information (e.g., passwords, banking details).
- Remove Keyloggers After Use to prevent misuse.
- Follow Cybersecurity Laws & Ethical Hacking Guidelines.

## Requirement
```
pip install pynput
```
*After installation: Run the script*

## How Does It Work?

**1. Listening for Keystrokes**
   - The script uses `pynput.keyboard.Listener` to detect key presses.
   - Every time a key is pressed, the `on_press` function is triggered.

**2. Logging the Keystrokes**
   - If the key is a regular character (letters, numbers, spaces), it is written as it is.
   - If the key is a special key (like Enter, Shift, Backspace), it is logged in brackets: `[ENTER]`, `[SHIFT]`, etc.
   - All keystrokes are appended to `keylog.txt`.

**3. Stopping the Keylogger**
   - The script runs indefinitely unless stopped manually.
   - Pressing `ESC` will stop the keylogger.

**4. Viewing the Logs**
   - Open `keylog.txt` after running the script.
   - The `keylog.txt` file will be created in the same directory as the Script (code) File.
   - You’ll see a log of all recorded keystrokes.

## Example Output
---
The logged keystrokes will be saved in keylog.txt. For example:

```
Hello[Key.shift]World[Key.space]My[Key.space]name[Key.space]is[Key.space]Ujjawal.
```
