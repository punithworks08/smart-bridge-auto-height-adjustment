# Smart Bridge — Automatic Height Adjustment During Flood 🌉

A mini-project (VTU BEC586) that automatically raises a bridge structure when water levels rise, using Arduino, a soil moisture sensor, and a servo motor — with a buzzer alert on detection.

## 📖 Abstract

Floods cause significant loss of life and property, especially where infrastructure lacks the technology to respond dynamically. Bridges are critical infrastructure, and bridge failure during flooding can have catastrophic consequences. This project implements a **smart bridge** that senses rising water levels in its environment and automatically reacts — lifting itself to safety and sounding a buzzer alert — without manual intervention.

**Keywords:** Arduino, Servo Motor, Buzzer, Soil Moisture Sensor

## ⚙️ How It Works

1. A soil moisture sensor placed near the bridge base continuously monitors water level.
2. The Arduino Uno reads sensor values and compares them against a defined safety threshold.
3. When water level crosses the threshold:
   - A **buzzer** sounds to alert nearby people
   - A **servo motor** lifts the bridge structure automatically
4. The bridge lowers back once water recedes below the threshold.

## 🛠️ Tech Stack

- **Microcontroller:** Arduino Uno
- **Language:** Embedded C
- **IDE:** Arduino IDE
- **Sensors:** Soil moisture sensor
- **Actuator:** Servo motor
- **Alert:** Buzzer

## 🔩 Hardware Components

| Component | Purpose |
|---|---|
| Arduino Uno | Main controller running the logic |
| Soil moisture sensor | Detects rising water level |
| Servo motor | Physically lifts/lowers the bridge |
| Buzzer | Audible alert on flood detection |
| Jumper wires, Sun board | Circuit assembly |
| Power supply | Powers the Arduino, servo, and buzzer |

## 🎯 Objectives

- Design a bridge structure that automatically adjusts its height in response to rising floodwaters
- Develop a system that autonomously detects rising water levels
- Minimize the risk of bridge submersion or structural failure during floods

## 🚀 Getting Started

### Prerequisites
- [Arduino IDE](https://www.arduino.cc/en/software) installed
- Arduino Uno connected via USB

### Setup
```bash
# Clone the repository
git clone https://github.com/punithworks08/smart-bridge-auto-height-adjustment.git

# Open the .ino file in Arduino IDE
# Select your board (Arduino Uno) and COM port under Tools
# Click Upload
```

### Wiring
- Soil moisture sensor signal pin → Arduino analog input
- Servo motor signal pin → Arduino digital PWM pin
- Buzzer signal pin → Arduino digital output pin
- Common ground between sensor, servo, buzzer, and Arduino

## 🔮 Future Improvements

- Add IoT connectivity to send remote flood alerts (SMS/app notification)
- Log sensor data over time for historical flood pattern analysis
- Replace threshold logic with a smoother, sensor-fused response
- Add solar-powered backup for remote deployment

## 👥 Team

This project was developed as a mini-project (BEC586) at East West Institute of Technology, Department of ECE, under the guidance of **Prof. Bhagya**.

- Punith R T
- Sagar S
- Madhu B R
- Rakesh C

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 👤 Contact

**Punith RT**
[LinkedIn](https://linkedin.com/in/punithrt) · punithsan8@gmail.com
