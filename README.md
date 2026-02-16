# UltraSonicTabSwitcher

A small project that allows automated control and switching between tabs or inputs using an Arduino sensor system. The project demonstrates basic integration between Python and Arduino, reading sensor input and using it to trigger tab changes or other events on a computer.

## 📂 Project Structure

- `main.py` — Python script that reads input from the Arduino and triggers tab switching logic.
- `sensor.ino` — Arduino sketch that collects sensor data (e.g., button, IR, or proximity sensor) and sends it to the computer via Serial communication.
- `.gitattributes` — Git configuration file for managing text file encoding and line endings.

## 🚀 How It Works

1. The Arduino board runs the `sensor.ino` sketch and reads input from a sensor.
2. The sensor data is sent over serial to the computer.
3. `main.py` listens to the serial port and triggers tab changes based on the received data (can be extended to control browser tabs, apps, or perform hotkey simulations).

## 🧰 Requirements

### Hardware:
- Arduino board (Nano, Uno, etc.)
- Sensor (e.g., button, proximity sensor, etc.)
- USB cable

### Software:
- Python 3.x
- `pyserial` library (`pip install pyserial`)
- Arduino IDE

## 🛠️ Setup

1. Upload `sensor.ino` to your Arduino using the Arduino IDE.
2. Run `main.py` on your computer to listen for serial data and respond to sensor input.
3. Customize the logic inside `main.py` to match your system's behavior (e.g., keyboard simulation, window switching, etc.).

## 💡 Use Cases

- Assistive tech: change tabs with hand gestures or buttons
- Custom hardware input for accessibility
- Hackathon projects involving human-computer interaction

## 📜 License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).

---

Feel free to modify the behavior and contribute improvements!
