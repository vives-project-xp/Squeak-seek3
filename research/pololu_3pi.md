
# Pololu 3pi Robot — Pinout & Usage Guide

---

## Overview

The **Pololu 3pi robot** is a compact, versatile platform for robotics enthusiasts and educators. It features an ATmega168 or ATmega328 microcontroller and offers several accessible pins for various functions.

---

## Pinout Overview

The 3pi robot provides several accessible pins located between the two motors on the PCB. Some pins are connected to internal components by default (e.g., PC5 to IR sensor emitters) and can be repurposed if jumpers are removed.

### Accessible Pins

| Pin         | Default Connection/Function                                 | Notes                                      |
|-------------|-------------------------------------------------------------|--------------------------------------------|
| **PC5**     | IR sensor emitters (ADC5)                                  | Digital I/O or analog input if jumper off  |
| **ADC6**    | Battery voltage divider                                     | Analog input if jumper off                 |
| **ADC7**    | User trimmer potentiometer                                  | Analog input if jumper off                 |
| **PD0 (RX)**| Serial receive                                             |                                            |
| **PD1 (TX)**| Serial transmit                                            |                                            |
| **PD2–PD7** | General-purpose digital I/O                                |                                            |
| **PB0–PB5** | General-purpose digital I/O                                |                                            |

### Motor Driver Connections

- **Motor A:**
  - **PWM:** PD3
  - **DIR:** PD4
- **Motor B:**
  - **PWM:** PD5
  - **DIR:** PD6

### Other Features

- **IR Sensors:** Five for line following
- **LCD Display:** Mounted on top for user interface
- **Buzzer:** Audio feedback
- **Buttons:** Three user buttons

---

## Usage

### On board Components
#### IR Sensors
The 3pi robot includes five infrared sensors for line following and obstacle detection. These sensors are connected to the microcontroller's ADC pins, allowing for analog readings of reflected IR light intensity.

### Buzzer
The onboard buzzer can be controlled via a digital pin to produce sound for alerts or feedback.

### Buttons
The 3pi robot has three user buttons connected to specific digital pins, allowing for user input and interaction with the robot's programs.

### Powering Up

The 3pi robot is powered by four AA batteries. Ensure correct installation and sufficient charge. An onboard voltage regulator manages power distribution.

### Programming

Program the 3pi robot using the Arduino IDE. See the [Pololu 3pi Robot User’s Guide](https://www.pololu.com/docs/0J21/) for setup instructions.

### Expansion

A 2x7 header exposes several I/O pins for expansion (sensors, actuators, etc.). See the user guide for detailed pinout.

---

## Resources

- 📖 [Pololu 3pi Robot User’s Guide](https://www.pololu.com/docs/0J21/)
- 🗺️ [Simplified Schematic Diagram](https://www.pololu.com/picture/view/0J1164)

---

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
