# Smart Home

## Introduction

**Smart Home** is a sensor-driven automation system designed to provide intelligent control over home environments. Using an AUTOSAR-inspired layered model, this embedded solution enhances daily living by integrating safety, comfort, and energy optimization. The system monitors various environmental parameters through a network of sensors and automates devices based on real-time conditions.

## How to Use

To get started with the Smart Home system:

1. Clone the repository to your local environment.
2. Navigate to the project directory using your terminal or IDE.
3. Run the primary application file to initiate the system interface.

## System Security

Access to the system is protected by a password-based entry mechanism. Users are granted a maximum of three login attempts. After three incorrect tries, the system locks down to prevent unauthorized access.

## Environmental Automation Features

### Temperature Regulation

The system evaluates temperature levels and adjusts the air conditioning unit accordingly:

- **< 20°C** → AC remains off.
- **20–24°C** → Activates low-speed cooling.
- **25–34°C** → Switches to medium-speed mode.
- **≥ 35°C** → Operates at full speed for maximum cooling.

### Light Sensitivity Control

Utilizing LDR readings, the lighting system adjusts based on room brightness:

- **≥ 50% light detected** → Lamps are turned off to conserve power.
- **< 50% light detected** → Lamps are activated for visibility.

## Integrated Sensors & Reactions

### Motion Detection (PIR)

Monitors movement in outdoor or hallway areas. If motion is detected, an external light is automatically triggered for safety or security purposes.

### Flame Monitoring

A dedicated sensor detects the presence of flames. On detection, the system issues an internal warning, alerting residents of a possible fire threat.

### Gas Leak Detection

The system continuously checks for the presence of harmful or flammable gases. If dangerous levels are detected, a gas alarm is activated immediately.

## Simulated Environment

<img width="700" height="587" alt="simulation" src="https://github.com/user-attachments/assets/247a4927-98a3-47da-92a7-d2327c837aea" />

The above simulation was created using **Proteus**, providing a virtual representation of the system's sensor interactions and automation logic. This helps validate the setup and logic before deploying it on real hardware.

## Feature Summary

- **Digital Lock Integration** – Adds secure, password-based access to the system.
- **Automatic AC Control** – Dynamically adjusts air conditioning based on ambient temperature.
- **Smart Lighting** – Reacts to changes in light levels to control lamp state.
- **Emergency Alerts** – Fires and gas leaks trigger instant warnings for immediate attention.

---

**Smart Home** demonstrates the capabilities of combining sensor inputs, real-time logic, and automation to create a safer and smarter living space. Ideal for embedded systems learners and IoT enthusiasts looking to explore real-world applications.
