# SG90 Servo Motor Interfacing with Arduino: Complete Beginner Guide (2026)

![Hero Banner](images/sg90-servo-motor/Hero%20Banner.png)

![License](https://img.shields.io/github/license/talha88001/chip-pk-knowledge-hub?style=for-the-badge)
![Arduino](https://img.shields.io/badge/Arduino-Uno-blue?style=for-the-badge)
![Electronics](https://img.shields.io/badge/Electronics-Tutorial-red?style=for-the-badge)
![Robotics](https://img.shields.io/badge/Robotics-SG90-green?style=for-the-badge)

---

## 📖 Introduction

The **SG90 Micro Servo Motor** is one of the most popular servo motors used in Arduino, robotics, IoT, automation, and educational electronics projects. It provides accurate angular movement between **0° and 180°**, making it perfect for applications where precise positioning is required.

Unlike a standard DC motor, an SG90 servo uses an internal feedback mechanism that allows it to rotate to an exact angle based on a PWM (Pulse Width Modulation) signal from a microcontroller such as an Arduino Uno.

This guide covers everything you need to know, including specifications, pinout, wiring, Arduino programming, troubleshooting, FAQs, and practical applications.

---

# 📑 Table of Contents

- Introduction
- What is an SG90 Servo Motor?
- SG90 Specifications
- SG90 Pinout
- How the SG90 Servo Works
- Components Required
- Arduino Wiring
- Arduino Programming
- Code Explanation
- Troubleshooting
- Applications
- FAQs
- Recommended Products
- Continue Learning

---

# What is an SG90 Servo Motor?

![SG90 Servo Motor Overview](images/sg90-servo-motor/SG90%20Servo%20Motor%20Overview.png)

The **SG90 Micro Servo Motor** is a lightweight servo actuator designed for precise angular control. It contains a small DC motor, plastic gear train, position feedback potentiometer, and an internal control circuit that work together to accurately position the output shaft.

Because of its low cost and compact design, it has become one of the most widely used servo motors for beginners and professionals alike.

### Common Applications

- Arduino Projects
- Robotics
- IoT Systems
- Smart Home Automation
- RC Vehicles
- Camera Pan-Tilt Systems
- Robotic Arms
- STEM Education
- DIY Electronics

---

# SG90 Servo Specifications

| Feature | Specification |
|----------|---------------|
| Operating Voltage | 4.8V – 6V |
| Recommended Voltage | 5V |
| Rotation Angle | 180° |
| Control Method | PWM |
| Weight | Approx. 9g |
| Stall Torque | Approx. 1.8 kg·cm |
| Speed | 0.12 sec / 60° |
| Gear Material | Plastic |

---

# SG90 Servo Pinout

![SG90 Servo Pinout](images/sg90-servo-motor/SG90%20Servo%20Pinout.png)

The SG90 servo motor has three wires.

| Wire Color | Function |
|------------|----------|
| Brown | Ground (GND) |
| Red | +5V Power |
| Orange | PWM Signal |

### Brown Wire

Connects to Arduino GND.

### Red Wire

Connects to Arduino 5V.

### Orange Wire

Receives the PWM control signal from the Arduino.

---

# How the SG90 Servo Motor Works

Unlike conventional DC motors, servo motors use a **closed-loop control system**.

The internal controller continuously compares the desired shaft position with the actual shaft position using a potentiometer. If the two positions differ, the motor rotates until the desired angle is reached.

The Arduino controls the SG90 by sending PWM signals:

| Pulse Width | Servo Position |
|--------------|----------------|
| 1.0 ms | 0° |
| 1.5 ms | 90° |
| 2.0 ms | 180° |

The Arduino Servo Library automatically generates these PWM signals, making servo programming simple.

---

# Components Required

To complete this project, you'll need:

- Arduino Uno R3
- SG90 Micro Servo Motor
- Breadboard
- Jumper Wires
- USB Cable
- Arduino IDE

---

# Arduino Wiring Diagram

![Arduino SG90 Wiring Diagram](images/sg90-servo-motor/Arduino%20SG90%20Wiring%20Diagram.png)

| Arduino Uno | SG90 Servo |
|--------------|------------|
| 5V | Red Wire |
| GND | Brown Wire |
| Digital Pin 9 | Orange Wire |

---

# Real Hardware Connection

![Real Project Connection](images/sg90-servo-motor/Real%20Project%20Connection.png)

The real hardware setup includes:

- Arduino Uno
- SG90 Servo Motor
- Breadboard
- Jumper Wires
- USB Connection

Always verify the wiring before uploading the Arduino sketch.

---

## Continue to Part 2 →

Part 2 includes:

- Arduino Code
- Code Explanation
- Servo Rotation
- Troubleshooting
- Applications
- FAQs
- Recommended Products
- Continue Learning
- License

  # Arduino Programming

## Arduino Servo Library

The Arduino IDE includes a built-in **Servo Library**, making it easy to control SG90 and other standard servo motors.

Simply include the library:

```cpp
#include <Servo.h>
```

No additional installation is required.

---

# Complete Arduino Code

![Arduino IDE Code Screenshot](images/sg90-servo-motor/Arduino%20IDE%20Code%20Screenshot.png)

```cpp
#include <Servo.h>

Servo myServo;

void setup()
{
    myServo.attach(9);
}

void loop()
{
    myServo.write(0);
    delay(1000);

    myServo.write(90);
    delay(1000);

    myServo.write(180);
    delay(1000);
}
```

Upload this sketch to your Arduino Uno. The servo will rotate to:

- **0°**
- **90°**
- **180°**

and repeat continuously.

---

# Code Explanation

### Include the Servo Library

```cpp
#include <Servo.h>
```

Loads Arduino's built-in Servo Library.

---

### Create a Servo Object

```cpp
Servo myServo;
```

Creates a servo object named **myServo**.

---

### Attach the Servo

```cpp
myServo.attach(9);
```

Connects the servo signal wire to **Digital Pin 9**.

---

### Rotate to 0°

```cpp
myServo.write(0);
```

Moves the servo shaft fully to the left.

---

### Rotate to 90°

```cpp
myServo.write(90);
```

Moves the servo to the center position.

---

### Rotate to 180°

```cpp
myServo.write(180);
```

Moves the servo fully to the right.

---

# Servo Rotation

![Servo Rotation Diagram](images/sg90-servo-motor/Servo%20Rotation%20Diagram.png)

The SG90 responds to PWM signals by rotating to a specific angle.

| PWM Pulse | Servo Position |
|-----------|----------------|
| 1.0 ms | 0° |
| 1.5 ms | 90° |
| 2.0 ms | 180° |

Never force the servo beyond its mechanical limits, as this may damage the internal gears.

---

# Troubleshooting

| Problem | Solution |
|----------|----------|
| Servo does not move | Verify wiring and power supply. |
| Servo vibrates | Use a stable 5V power supply. |
| Arduino resets | Power the servo from an external regulated 5V supply and connect the grounds together. |
| Servo rotates randomly | Check the PWM signal wire. |
| Servo becomes hot | Reduce the mechanical load. |
| Servo only rotates partially | Verify the Arduino code and ensure the servo is not obstructed. |

---

# Best Practices

- Use a regulated 5V power supply.
- Double-check wiring before powering the circuit.
- Never rotate the servo horn manually while powered.
- Keep jumper wires short and secure.
- Test the servo using a simple sketch before integrating it into larger projects.
- Avoid overloading the SG90 servo.

---

# Applications

![SG90 Servo Motor Applications Overview](images/sg90-servo-motor/SG90%20servo%20motor%20applications%20overview.png)

The SG90 Servo Motor is widely used in:

- Robotic Arms
- Pan-Tilt Camera Systems
- Smart Door Locks
- RC Airplanes
- Robot Cars
- Educational Robotics
- Automation Projects
- DIY Electronics
- Sensor Positioning
- STEM Learning Kits

---

# Frequently Asked Questions (FAQs)

## Can I power the SG90 directly from the Arduino?

Yes, for small demonstration projects. For multiple servos or heavier loads, use an external regulated 5V power supply.

---

## What is the operating voltage?

The SG90 operates between **4.8V and 6V**, with **5V** recommended.

---

## Which Arduino pin should I use?

This guide uses **Digital Pin 9**, but the Servo Library supports multiple digital pins.

---

## Can the SG90 rotate continuously?

No. A standard SG90 rotates approximately **180°**. Continuous rotation servo motors are different products.

---

## Can I connect multiple servos?

Yes. The Arduino Servo Library supports multiple servo motors. Use a suitable external power supply for reliable operation.

---

## Why does my servo jitter?

Servo jitter is commonly caused by:

- Low supply voltage
- Loose wiring
- Electrical noise
- Insufficient current

---

# Recommended Products

Build your own Arduino servo project with these components from **Chip.pk**:

- **SG90 Micro Servo Motor**  
  https://www.chip.pk/search?q=SG90+Micro+Servo+Motor

- **Arduino Uno R3**  
  https://www.chip.pk/search?q=Arduino+Uno+R3

- **Breadboard & Jumper Wire Kit**  
  https://www.chip.pk/search?q=Breadboard+Jumper+Wire+Kit

- **ESP32 30-Pin ESP-WROOM-32 Development Board**  
  https://www.chip.pk/search?q=ESP32+30-Pin+ESP-WROOM-32

- **Raspberry Pi Pico RP2040**  
  https://www.chip.pk/search?q=Raspberry+Pi+Pico+RP2040

- **Raspberry Pi Pico 2 RP2350**  
  https://www.chip.pk/search?q=Raspberry+Pi+Pico+2+RP2350

- **PCA9685 16-Channel Servo Driver Module**  
  https://www.chip.pk/search?q=PCA9685+16-Channel+Servo+Driver

- **Servo Extension Cable**  
  https://www.chip.pk/search?q=Servo+Extension+Cable

---

# Continue Learning

Explore more beginner-friendly electronics and robotics guides from the **Chip.pk Knowledge Hub**:

- Arduino Uno Complete Guide
- Arduino vs ESP32
- Relay Module Complete Guide
- Relay Module Interfacing with Arduino
- Raspberry Pi Pico vs Raspberry Pi Pico 2
- ESP32 Beginner Guide
- Top 5 Beginner Electronics Projects

Visit our Knowledge Hub:

https://www.chip.pk/blogs/chip-pk-knowledge-hub

---

# Contributing

Found an error or have a suggestion?

Feel free to open an issue or submit a pull request. Contributions that improve the quality and accuracy of the documentation are always welcome.

---

# License

This project is part of the **Chip.pk Knowledge Hub**.

All tutorials, diagrams, and educational content are intended to help students, hobbyists, makers, and professionals learn electronics, embedded systems, robotics, and IoT technologies.

---

⭐ **If you found this guide helpful, consider starring this repository to support the Chip.pk Knowledge Hub and help others discover high-quality electronics tutorials.**

**Website:** https://www.chip.pk

**Knowledge Hub:** https://www.chip.pk/blogs/chip-pk-knowledge-hub

**GitHub Repository:** https://github.com/talha88001/chip-pk-knowledge-hub
