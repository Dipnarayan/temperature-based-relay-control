<div align="center">

# 🌡️ Temperature-Based Relay Control

### Smart Temperature Monitoring and Automated Device Control

An embedded automation system that continuously monitors ambient temperature using a DHT11 sensor and automatically controls connected electrical devices through relay switching.

![Embedded Systems](https://img.shields.io/badge/Domain-Embedded%20Systems-blue)
![IoT](https://img.shields.io/badge/Application-IoT%20Automation-green)
![Arduino](https://img.shields.io/badge/Platform-Arduino-orange)
![Sensor](https://img.shields.io/badge/Sensor-DHT11-red)
![Automation](https://img.shields.io/badge/Type-Automation-purple)

</div>

---

# 📖 Overview

Automation systems play an important role in modern homes, industries, and safety-critical environments.

This project introduces a temperature-based relay control system that automatically activates or deactivates electrical devices based on ambient temperature readings.

The system continuously monitors environmental conditions through a DHT11 temperature sensor and performs intelligent switching operations through a relay module.

The framework can be used for:

- Smart fan control
- Heater automation
- Overheat protection
- Home automation
- Industrial monitoring
- Environmental control systems

The project demonstrates the integration of sensors, microcontrollers, actuators, and feedback mechanisms within a simple embedded control architecture. :contentReference[oaicite:1]{index=1}

---

# 🎯 Objectives

The primary objectives of this project are:

- Monitor ambient temperature in real time
- Automate electrical device control
- Reduce manual intervention
- Improve energy efficiency
- Provide overheat protection
- Demonstrate sensor-actuator integration
- Build a low-cost automation system

---

# ✨ Key Features

## 🌡️ Real-Time Temperature Monitoring

The system continuously measures ambient temperature using the DHT11 sensor.

### Captured Data

- Temperature
- Environmental conditions

---

## ⚡ Automatic Relay Switching

The relay automatically changes state whenever the measured temperature crosses a predefined threshold.

This enables automatic control of connected devices such as:

- Fans
- Heaters
- Cooling systems
- Warning systems

---

## 💡 Visual Status Indication

An LED indicator provides visual feedback whenever the relay state changes.

Benefits include:

- Quick status verification
- Easy troubleshooting
- Improved usability

---

## 🔄 Autonomous Operation

Once powered, the system operates without human intervention.

---

# 🏗️ System Architecture

```text
Ambient Temperature
         │
         ▼
DHT11 Sensor
         │
         ▼
Microcontroller
         │
 ┌───────┴────────┐
 │                │
 ▼                ▼
Relay Module    LED Indicator
 │
 ▼
Connected Device
(Fan / Heater / Alarm)
```

---

# ⚙️ Working Principle

The system follows a simple control loop.

### Step 1

The DHT11 sensor measures ambient temperature.

### Step 2

Temperature data is sent to the microcontroller.

### Step 3

The controller compares the reading against a predefined threshold.

### Step 4

If the temperature exceeds the threshold:

```text
Relay = ON
```

or

```text
Relay = OFF
```

depending on the application logic.

### Step 5

The LED briefly illuminates to indicate a relay state transition.

### Step 6

The system resumes continuous monitoring.

---

# 🔌 Hardware Components

## DHT11 Temperature Sensor

Responsible for:

- Temperature sensing
- Environmental monitoring

### Features

- Low cost
- Easy interfacing
- Reliable operation

---

## Microcontroller

Responsible for:

- Sensor communication
- Data processing
- Relay control
- LED control

The microcontroller acts as the central processing unit of the system.

---

## Relay Module

Responsible for:

- Electrical switching
- Load control
- Device automation

The relay isolates the low-voltage control circuit from high-power electrical devices.

---

## LED Indicator

Responsible for:

- State visualization
- Relay activity indication

---

## Power Supply

Provides stable voltage to:

- Microcontroller
- DHT11 sensor
- Relay module
- LED indicator

---

# 🔧 Circuit Connections

## DHT11 Sensor

| Pin | Connection |
|-------|------------|
| Data | Digital Pin 4 |
| VCC | 5V |
| GND | Ground |

---

## Relay Module

| Pin | Connection |
|-------|------------|
| Signal | Digital Pin 2 |
| VCC | Power |
| GND | Ground |

---

## LED Indicator

| Pin | Connection |
|-------|------------|
| Anode | Digital Pin 13 |
| Cathode | Ground through 220Ω resistor |

---

# 📊 System Behavior

## Normal State

```text
Temperature < Threshold
```

The relay remains in its default state while monitoring continues.

---

## High Temperature State

```text
Temperature > Threshold
```

The relay changes state to control the connected device.

Example:

- Turn ON cooling fan
- Turn OFF heater

---

## State Transition

Whenever a relay state changes:

```text
LED = Blink
```

This provides immediate visual feedback.

---

# 🌍 Applications

## Smart Homes

- Automatic fan control
- Room temperature regulation

## Industrial Automation

- Equipment cooling systems
- Machine protection

## Safety Systems

- Overheat detection
- Emergency shutdown systems

## Agriculture

- Greenhouse climate control
- Environmental monitoring

## Laboratories

- Temperature-sensitive equipment protection

---

# 🚀 Advantages

### Low Cost

Uses inexpensive and widely available components.

### Energy Efficient

Operates only when required.

### Autonomous

Requires minimal human intervention.

### Scalable

Can be extended with:

- Wi-Fi modules
- IoT dashboards
- Cloud monitoring
- Mobile applications

### Reliable

Provides real-time response to environmental changes.

---

# 🔮 Future Enhancements

Potential future improvements include:

## IoT Integration

- Cloud connectivity
- Remote monitoring

## Mobile Applications

- Real-time notifications
- Remote control

## Data Logging

- Historical temperature analysis
- Trend monitoring

## Multiple Sensors

- Humidity monitoring
- Air quality monitoring

## AI-Based Control

- Predictive cooling systems
- Intelligent energy management

---

# 🏛 Academic Contribution

This project contributes to:

- Embedded Systems
- Sensor-Based Automation
- IoT Applications
- Smart Control Systems
- Environmental Monitoring
- Actuator Control

The work demonstrates how simple sensor-actuator architectures can be used to automate real-world control systems efficiently and economically.

---

# 📚 Technologies Used

- Arduino C/C++
- DHT11 Sensor
- Relay Module
- LED Indicator
- Embedded Programming
- Digital Electronics

---

# 📖 Citation

```bibtex
@misc{TemperatureRelayControl2024,
  title={Temperature-Based Relay Control Using DHT11 Sensor},
  author={Project Documentation},
  year={2024}
}
```

---

# 📚 Keywords

- Embedded Systems
- DHT11
- Relay Control
- Automation
- Temperature Monitoring
- Arduino
- IoT
- Smart Home
- Industrial Automation
- Environmental Monitoring
- Sensor Networks
- Control Systems

---

# License

MIT License
