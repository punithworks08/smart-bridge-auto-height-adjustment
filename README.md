# Smart Bridge — Auto Height Adjustment 🌉

Real-time flood detection and response system that automatically raises a bridge structure when water levels rise, using Arduino, moisture sensors, and UART-based servo control.

## 📖 Overview

Low-lying bridges are prone to flooding during heavy rain or rising water levels, often requiring manual intervention to prevent damage or blockage. This project automates that response — a moisture sensor continuously monitors water level near the bridge, and when a threshold is crossed, a servo motor mechanism lifts the bridge automatically, without any human involvement.

## ⚙️ How It Works

1. A moisture/water-level sensor placed at the base of the bridge continuously reads live data.
2. The Arduino reads sensor values and compares them against a defined safety threshold.
3. When water level exceeds the threshold, the Arduino sends a control signal over UART to trigger the servo motor.
4. The servo motor lifts the bridge mechanism, keeping it clear of rising water.
5. The bridge lowers back automatically once water recedes below the threshold.

## 🛠️ Tech Stack

- **Microcontroller:** Arduino (Uno/Nano)
- **Language:** C++ (Arduino IDE)
- **Sensors:** Moisture / water-level sensor
- **Actuator:** Servo motor
- **Communication:** UART

## 🔩 Hardware Components

| Component | Purpose |
|---|---|
| Arduino board | Main controller running the logic |
| Moisture sensor | Detects rising water level |
| Servo motor | Physically lifts/lowers the bridge |
| Jumper wires, breadboard | Circuit connections |
| Power supply | Powers the Arduino and servo |

## 🚀 Getting Started

### Prerequisites
- [Arduino IDE](https://www.arduino.cc/en/software) installed
- Arduino board connected via USB

### Setup
```bash
# Clone the repository
git clone https://github.com/punithworks08/smart-bridge-auto-height-adjustment.git

# Open the .ino file in Arduino IDE
# Select your board and COM port under Tools
# Click Upload
```

### Wiring
- Moisture sensor signal pin → Arduino analog input
- Servo motor signal pin → Arduino digital PWM pin
- Common ground between sensor, servo, and Arduino

## 📊 Results

The system reliably detects rising water levels and triggers automated bridge lifting within seconds of threshold crossing, removing the need for manual monitoring or intervention.

## 🔮 Future Improvements

- Add a mobile/web dashboard for remote water-level monitoring
- Log sensor data over time for historical flood pattern analysis
- Add solar-powered backup for remote deployment
- Replace threshold logic with a smoother PID-based lift response

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Punith RT**
[LinkedIn](https://linkedin.com/in/punithrt) · punithsan8@gmail.com
