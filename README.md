# 💧 Motor Control & Water Saving Timer using Arduino

A simple and affordable Arduino-based project to **automatically turn off water pumps or motors** after a preset time using a **4x4 keypad**, **LCD display**, and **relay control**. The system helps in **saving water** and **avoiding wastage** due to unattended running of electric motors or appliances.

---

## 📌 Features

- Set timer duration via keypad (in seconds)
- Display countdown on LCD
- Automatically turns off motor (or LED for testing) after countdown ends
- Easy to use and low-cost
- Prevents water wastage from overrun motors

---

## 🔧 Components Used

| Component              | Quantity |
|------------------------|----------|
| Arduino UNO / Nano     | 1        |
| 4x4 Matrix Keypad      | 1        |
| 16x2 I2C LCD Display    | 1        |
| Relay Module (1-Channel) | 1        |
| LED (used for demo)    | 1        |
| 220Ω Resistor          | 1        |
| Connecting Wires + Breadboard | 1 |

> You can replace the LED with a motor or pump via a properly rated relay module.

---

## 🔌 Wiring Diagram

| Module | Arduino Pin |
|--------|-------------|
| Keypad R1-R4 | 9, 8, 7, 6 |
| Keypad C1-C4 | 5, 4, 3, 2 |
| LCD SDA/SCL | A4 (SDA), A5 (SCL) |
| Relay IN / LED Anode | D10 |
| Relay VCC / LED Resistor | 5V through 220Ω |
| Relay GND / LED Cathode | GND |

---

## 🧠 How It Works

1. The user enters the number of seconds to run the motor using the keypad.
2. After pressing `#`, the timer starts and the motor (or LED) is turned ON.
3. The remaining time is shown on the LCD display.
4. When the timer reaches 0, the motor (or LED) turns OFF automatically.
5. This helps **save water** by preventing overrun of water pumps.

---

## 📝 Code

The Arduino code is included in the repository under `motor_timer.ino`. It uses the following libraries:

- `Keypad.h`
- `Wire.h`
- `LiquidCrystal_I2C.h`

Make sure you install them using **Arduino Library Manager** before uploading.

---

## 🛠️ Future Improvements

- Add buzzer alert when time ends
- Real-time clock (RTC) for time-based scheduling
- Mobile control using Bluetooth (HC-05)
- EEPROM memory to store last timer value
- Rain sensor integration to stop irrigation when not needed

---

## ♻️ Save Water. Save Energy. Automate Smartly.

This project can be used in households, farms, and gardens to help **conserve water**, avoid damage from overheated motors, and encourage responsible usage.

---

## 📸 Demo

> Upload images or video here showing the project in action (timer running, LED/motor turning off, etc.)

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).
