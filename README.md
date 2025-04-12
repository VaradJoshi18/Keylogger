# ⌨️ Keylogger

**Keylogger** is a simple Python keylogging tool that captures and logs keystrokes into a file. Built using the `pynput` library, this project is intended for educational and testing purposes only. **Use responsibly and only on systems where you have explicit permission to do so.**

---

## Table of Contents

- [Features](#features-)
- [Requirements](#requirements-)
- [Installation](#installation-)
- [Usage](#usage-)
- [How It Works](#how-it-works-)
- [Disclaimer & Legal Notice](#disclaimer--legal-notice-)
- [Contributing](#contributing-)

---

## Features ✨

- **Real-time Key Capture:** Logs every key pressed in real time.
- **Simple File Logging:** Writes captured keystrokes to a file (`keylog.txt`).
- **Graceful Termination:** Automatically stops logging when the `Esc` key is pressed.
- **Minimalistic Implementation:** A straightforward and concise keylogger built with Python.

---

## Requirements 🛠

- **Python 3.x**: Ensure you have Python 3 installed on your system.
- **pynput Library:** Used to capture keyboard events.

---

## Installation 💾

1. **Clone or Download the Repository:**

   ```bash
   git clone https://github.com/yourusername/keylogger.git
   cd keylogger
   ```

2. **Create a Virtual Environment (Optional):**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the Required Package:**

   ```bash
   pip install pynput
   ```

---

## Usage 🚀

1. **Run the Keylogger:**

   Execute the script using Python:

   ```bash
   python keylogger.py
   ```

2. **Start Logging:**

   - Once running, the keylogger will capture all keystrokes.
   - All keys will be appended to the `keylog.txt` file in real time.

3. **Stop Logging:**

   - To stop the keylogger, press the `Esc` key. The listener will then cease logging, and the program will exit.

4. **View Log File:**

   - Open the `keylog.txt` file to review the captured keystrokes.

---

## How It Works 🔍

- **Key Capture:**
  - Uses `pynput.keyboard.Listener` to capture key presses via the `functionPerKey` callback.
  - Each captured key is appended to an in-memory list.

- **File Logging:**
  - After each key press, the keys are written to `keylog.txt`.
  - The file writes keys in succession, using a delimiter replacement to prevent issues with formatting.

- **Graceful Exit:**
  - The listener watches for the `Esc` key to shut down logging and end the program.

---

## Disclaimer ⚠️

> **Important:** This tool is for **educational purposes only**.  
> Unauthorized use on systems without explicit permission is illegal and unethical.  
> **I am not responsible for any misuse of this code.**  
> Always obtain proper consent before using a keylogger or any similar monitoring tool.

---
