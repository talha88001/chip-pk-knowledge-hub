# HC-SR04 Ultrasonic Distance Sensor with Arduino & ESP32 – Complete Guide

The **HC-SR04 Ultrasonic Distance Sensor** is one of the most popular distance measurement modules used in Arduino, ESP32, robotics, and IoT projects. It measures the distance between the sensor and an object using ultrasonic sound waves, making it ideal for obstacle avoidance robots, smart parking systems, automatic dustbins, water level monitoring, and automation projects.

---

## What is HC-SR04?

The HC-SR04 is a low-cost ultrasonic distance sensor that uses a transmitter and receiver operating at **40kHz**. It sends ultrasonic pulses and measures the time taken for the echo to return, allowing accurate distance calculation.

---

## Key Features

- Measuring Range: **2cm to 400cm**
- Operating Voltage: **5V DC**
- Operating Frequency: **40kHz**
- Accuracy: **±3mm**
- Measuring Angle: **15°**
- Fast and Reliable Distance Measurement
- Compatible with Arduino, ESP32, STM32, Raspberry Pi, and other microcontrollers

---

## Pin Configuration

The HC-SR04 module has four pins:

- **VCC** – 5V Power Supply
- **TRIG** – Trigger Input
- **ECHO** – Echo Output
- **GND** – Ground

---

## Working Principle

The microcontroller sends a **10µs trigger pulse** to the TRIG pin. The HC-SR04 then transmits an ultrasonic wave and waits for the reflected signal. The ECHO pin stays HIGH until the reflected wave returns. By measuring the travel time, the distance between the sensor and the object can be calculated.

---

## Arduino Interface

Typical connections with Arduino Uno:

| HC-SR04 | Arduino Uno |
|----------|-------------|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D10 |

The module works directly with Arduino Uno without additional components.

---

## ESP32 Interface

The HC-SR04 also works with ESP32. Since the ESP32 uses **3.3V GPIO**, it is recommended to use a **voltage divider or logic level converter** on the ECHO pin to protect the ESP32 input.

---

## Common Applications

- Obstacle Avoidance Robots
- Smart Parking Systems
- Water Tank Level Monitoring
- Automatic Dustbins
- Distance Measuring Devices
- Smart Home Automation
- Robotics and STEM Projects

---

## Why Choose HC-SR04?

The HC-SR04 offers excellent accuracy, a long measuring range, and simple interfacing at an affordable price. It is one of the best ultrasonic sensors for beginners, students, hobbyists, and professional embedded system developers.

---

## Recommended Products

- HC-SR04 Ultrasonic Distance Sensor
- Arduino Uno R3
- ESP32 Development Board
- Breadboard
- Jumper Wires
- SG90 Servo Motor
- L298N Motor Driver
- Robot Car Chassis
- 16×2 LCD Display with I2C Module

Browse genuine electronic components at:

**🌐 https://www.chip.pk**

---

## Learn More

For detailed tutorials, wiring diagrams, Arduino & ESP32 code examples, troubleshooting tips, and project ideas, visit the **Chip.pk Knowledge Hub**.

**Website:** https://www.chip.pk

---

### About Chip.pk

Chip.pk is Pakistan's trusted online electronics marketplace, offering genuine Arduino, ESP32, Raspberry Pi, STM32, robotics modules, sensors, displays, power supplies, development boards, and embedded system components for students, makers, engineers, and industries.
