# HC-SR04 Ultrasonic Distance Sensor with Arduino & ESP32 – Complete Guide

The **HC-SR04 Ultrasonic Distance Sensor** is one of the most popular distance-measuring sensors used in Arduino, ESP32, robotics, and IoT projects. It measures the distance between the sensor and an object using ultrasonic sound waves, making it ideal for obstacle avoidance robots, parking systems, automatic dustbins, water-level monitoring, and smart automation.

---

# Hero Banner

![HC-SR04 Hero Banner](../images/electronics-components/hc-sr04/Hero%20Banner.png)

---

# What You'll Learn

- HC-SR04 Overview
- Technical Specifications
- Pinout
- Working Principle
- Arduino Wiring
- ESP32 Wiring
- Sample Arduino Code
- Real Applications
- Common Problems
- Recommended Products

---

# HC-SR04 Overview

![Front View](../images/electronics-components/hc-sr04/HC-SR04%20Front%20View.png)

The HC-SR04 uses ultrasonic waves at approximately **40kHz** to calculate the distance between the sensor and an object.

Typical specifications include:

- Measuring Range: 2cm – 400cm
- Operating Voltage: 5V
- Measuring Angle: 15°
- Accuracy: ±3mm
- Frequency: 40kHz

---

# HC-SR04 Pinout

![Pinout](../images/electronics-components/hc-sr04/HC-SR04%20Pinout%20Diagram.png)

Pins:

- VCC
- TRIG
- ECHO
- GND

---

# Working Principle

![Working Principle](../images/electronics-components/hc-sr04/How%20HC-SR04%20Works%20%28Working%20Principle%29.png)

The controller sends a 10µs trigger pulse.

The HC-SR04 transmits an ultrasonic burst, waits for the reflected echo, and calculates the distance based on the time taken for the signal to return.

---

# Arduino Wiring

![Arduino Wiring](../images/electronics-components/hc-sr04/HC-SR04%20Arduino%20Wiring%20Diagram.png)

Typical connections:

| HC-SR04 | Arduino Uno |
|----------|-------------|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D10 |

---

# ESP32 Wiring

![ESP32 Wiring](../images/electronics-components/hc-sr04/HC-SR04%20ESP32%20Wiring%20Diagram.png)

When using an ESP32, reduce the HC-SR04 ECHO signal to 3.3V using a voltage divider before connecting it to a GPIO pin.

---

# Arduino IDE

![Arduino IDE](../images/electronics-components/hc-sr04/Arduino%20IDE%20Code%20Screenshot.png)

The sensor can be used with simple Arduino code and does not require any special library.

---

# Distance Measurement Example

![Distance Measurement](../images/electronics-components/hc-sr04/Distance%20Measurement%20Example.png)

The Serial Monitor displays the measured distance in centimeters.

---

# Real Hardware Setup

![Hardware Setup](../images/electronics-components/hc-sr04/Real%20Hardware%20Setup.png)

The HC-SR04 can easily be integrated with:

- Arduino Uno
- ESP32
- Breadboard
- LCD Display
- Robot Chassis
- Servo Motors
- Buzzers

---

# Applications

![Applications](../images/electronics-components/hc-sr04/Applications%20Infographic.png)

Common applications include:

- Obstacle Avoidance Robot
- Smart Dustbin
- Water Level Monitoring
- Parking Sensor
- Smart Home Automation
- Distance Meter
- Robotics Projects

---

# HC-SR04 Comparison

![Comparison](../images/electronics-components/hc-sr04/Comparison%20Image.png)

The HC-SR04 offers a longer measuring range and more accurate distance measurement than basic IR obstacle sensors, making it an excellent choice for robotics and automation projects.

---

# Recommended Products

Build your project using genuine electronic components from **Chip.pk**.

- HC-SR04 Ultrasonic Sensor
- Arduino Uno R3
- ESP32 Development Board
- Breadboard
- Jumper Wires
- SG90 Servo Motor
- L298N Motor Driver
- Robot Car Chassis
- 16×2 LCD with I2C
- Resistor Kit

Browse products:

https://www.chip.pk/

---

# Read the Complete Guide

This GitHub article is a shortened version.

📖 Read the complete tutorial with wiring diagrams, Arduino code, ESP32 interfacing, troubleshooting, FAQs, and project ideas:

https://www.chip.pk/blogs/chip-pk-knowledge-hub/

---

## License

MIT License

© Chip.pk Knowledge Hub
