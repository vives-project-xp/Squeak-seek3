
# ATOM Lite Pinout & Specs

## Pinout

| Pin      | Function    |
|----------|-------------|
| 3V3      | Power       |
| G22      |             |
| G19      | MOSI        |
| G23      | CLK         |
| G33      | MISO / ADC  |
| G21      | SCL         |
| G25      | DAC / SDA   |
| 5V (x2)  | Power       |
| GND (x2) | Ground      |
| G26      | DAC         |
| G32      | ADC         |
| G27      | RGB LED     |
| G37      | Button      |
| G12      | IR          |

## Size

**Dimensions:** 81.0 × 65.0 × 13.0 mm

## connection ways to pololu 3pi
### I2C Connection
- **SCL (G21)** to **SCL** on 3pi
- **SDA (G25)** to **SDA** on 3pi
### UART Connection
- **TX (G19)** to **RX** on 3pi
- **RX (G23)** to **TX** on 3pi
### SPI Connection
- **MOSI (G19)** to **MOSI** on 3pi
- **MISO (G33)** to **MISO** on 3pi
- **CLK (G23)** to **SCK** on 3pi
- **CS (G22)** to **CS** on 3pi
### GPIO Connection
- **G26, G32, G27, G37** can be used as general-purpose input/output pins to interface with various components on the 3pi robot.

---
**Source:** [M5Stack ATOM Lite Documentation](https://docs.m5stack.com/en/core/ATOM%20Lite)