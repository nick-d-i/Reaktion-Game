# Reaction Time Game (Arduino)

A fun 2-player reaction time game built using an Arduino, two buttons, an LCD, and three LEDs. Players compete to react fastest after a countdown, while premature presses award a point to the opponent.

## 📦 Features

- I2C LCD display (16x2) for game status and score
- 3 LED countdown before reaction test
- Early press detection gives opponent a point
- Score tracking up to 5 rounds
- Clean UI using serial monitor and LCD
- Reset and play again feature

## 🛠️ Hardware Required

- Arduino Uno (or compatible)
- 2 push buttons
- 3 LEDs
- 3 resistors (220Ω for LEDs)
- 1 I2C LCD display (16x2, address 0x27 common)
- Breadboard + jumper wires

## 🔌 Wiring Diagram

> You can add an image here under the `images/` folder.

| Component | Arduino Pin |
|----------|-------------|
| Button 1 | D2          |
| Button 2 | D4          |
| LED 1    | D7          |
| LED 2    | D8          |
| LED 3    | D9          |
| I2C SDA  | A4          |
| I2C SCL  | A5          |

## 🚀 Getting Started

1. Open `ReactionGame.ino` in the Arduino IDE.
2. Install the `LiquidCrystal_I2C` library from Library Manager.
3. Upload the sketch to your Arduino board.
4. Open the Serial Monitor at 9600 baud to view debug output.
5. Press both buttons to start a game!

## 📷 Demo

_Add a video or gif here if you can._

## 🧠 How it Works

- The game starts when **both players press their buttons**.
- A countdown begins using 3 LEDs turning off one by one.
- If a player presses too early, the opponent wins the round.
- After the countdown, first to press wins the round.
- Game ends after 5 rounds.

## 📄 License

MIT License (or specify your choice)

---

Made with ❤️ using Arduino.

