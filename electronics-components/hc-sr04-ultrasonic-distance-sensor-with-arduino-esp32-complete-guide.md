# HC-SR04 Ultrasonic Distance Sensor with Arduino & ESP32 – Complete Guide

The **HC-SR04 Ultrasonic Distance Sensor** is one of the most widely used distance-measuring modules for **Arduino**, **ESP32**, robotics, and IoT projects. It uses ultrasonic sound waves to accurately measure the distance between the sensor and an object, making it ideal for obstacle avoidance robots, parking systems, water-level monitoring, smart dustbins, and automation projects.

---

# Hero Banner

![Hero Banner](relay-module/images/hc-sr04/Hero%20Banner.png)

---

# Features

- Measuring Range: 2cm – 400cm
- Operating Voltage: 5V
- Operating Frequency: 40kHz
- Accuracy: ±3mm
- Easy Arduino & ESP32 Interface
- Low Cost & Beginner Friendly

---

# HC-SR04 Front View

![HC-SR04 Front View](../images/electronics-components/hc-sr04/HC-SR04%20Front%20View.png)

The HC-SR04 has four pins:

- VCC
- TRIG
- ECHO
- GND

It measures distance by transmitting ultrasonic pulses and calculating the time required for the echo to return.

---

# Pinout Diagram

![Pinout](../images/electronics-components/hc-sr04/HC-SR04%20Pinout%20Diagram.png)

The **TRIG** pin sends the ultrasonic pulse, while the **ECHO** pin receives the reflected signal. The measured time is converted into distance.

---

# Working Principle

![Working Principle](../images/electronics-components/hc-sr04/How%20HC-SR04%20Works%20%28Working%20Principle%29.png)

The controller sends a 10µs trigger pulse. The HC-SR04 emits a 40kHz ultrasonic wave and waits for the reflected echo. The travel time is then used to calculate the distance.

---

# Arduino Wiring

![Arduino Wiring](../images/electronics-components/hc-sr04/HC-SR04%20Arduino%20Wiring%20Diagram.png)

| HC-SR04 | Arduino Uno |
|----------|-------------|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D10 |

---

# ESP32 Wiring

![ESP32 Wiring](../images/electronics-components/hc-sr04/HC-SR04%20ESP32%20Wiring%20Diagram.png)

When connecting the HC-SR04 to an **ESP32**, use a voltage divider or level shifter on the **ECHO** pin because the ESP32 uses 3.3V GPIO logic.

---

# Arduino IDE

![Arduino IDE](../images/electronics-components/hc-sr04/Arduino%20IDE%20Code%20Screenshot.png)

The HC-SR04 can be programmed using the standard Arduino IDE with simple code and no additional libraries.

---

# Applications

![Applications](../images/electronics-components/hc-sr04/Applications%20Infographic.png)

Typical applications include:

- Obstacle Avoidance Robots
- Smart Parking Systems
- Automatic Dustbins
- Water Tank Level Monitoring
- Distance Measuring Devices
- Home Automation
- Robotics Projects

---

# Comparison

![Comparison](../images/electronics-components/hc-sr04/Comparison%20Image.png)

Compared to basic IR sensors, the HC-SR04 offers longer range, better distance measurement, and improved accuracy, making it an excellent choice for robotics and automation.

---

# Recommended Products

Build your project with genuine electronic components from **Chip.pk**.

- HC-SR04 Ultrasonic Sensor
- Arduino Uno R3
- ESP32 Development Board
- Breadboard
- Jumper Wires
- SG90 Servo Motor
- L298N Motor Driver
- Robot Car Chassis
- 16×2 LCD with I2C

🌐 **Website:** https://www.chip.pk

---

# Read the Complete Tutorial

For complete wiring diagrams, Arduino & ESP32 code, troubleshooting, FAQs, and detailed explanations, visit the Chip.pk Knowledge Hub.

👉 https://www.chip.pk/blogs/chip-pk-knowledge-hub

---

## License

MIT License

**© Chip.pk Knowledge Hub**
