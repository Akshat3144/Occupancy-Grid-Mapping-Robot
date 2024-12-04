# Probabilistic Robot Mapping System

## Project Overview

This project implements a probabilistic mapping system for an ESP32-based robotic platform using a VL53L0X distance sensor. The system allows for interactive mapping of an environment using log-odds probability mapping and provides real-time visualization of the robot's position and surroundings.

## Hardware Components

- ESP32 Microcontroller
- VL53L0X Distance Sensor
- DC Motors (with motor driver)
- Wireless Networking Capabilities

## Software Components

### ESP32 Firmware
- Implements Wi-Fi access point functionality
- Provides motor control interfaces
- Handles sensor readings and command processing

### Python Mapping Client
- Interactive mapping application
- Real-time grid visualization
- Probabilistic environment mapping
- Keyboard-based robot control

## Key Features

- Probabilistic log-odds mapping algorithm
- Interactive grid-based environment representation
- Real-time sensor data processing
- Customizable mapping parameters
- Visualized robot movement and sensor readings

## Prerequisites

### Hardware
- ESP32 Development Board
- VL53L0X Distance Sensor
- Motor Driver
- DC Motors

### Software
- Python 3.7+
- Libraries:
  - `matplotlib`
  - `numpy`
  - `socket`
  - `keyboard`
  - `keyboard`

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/robot-mapper.git
   cd robot-mapper
   ```

2. Install required Python dependencies:
   ```bash
   pip install matplotlib numpy keyboard
   ```

3. Flash the ESP32 firmware using Arduino IDE or PlatformIO

## Usage

### ESP32 Setup
1. Configure Wi-Fi credentials in the ESP32 firmware
2. Upload firmware to the ESP32 board
3. Ensure ESP32 creates a Wi-Fi access point

### Running the Mapping Application
1. Connect to the ESP32's Wi-Fi network
2. Run the Python script:
   ```bash
   python robot_mapper.py
   ```

3. Follow the on-screen prompts to:
   - Set up mapping parameters
   - Control robot movement
   - Visualize environment mapping

### Keyboard Controls
- Arrow Keys: Move the robot
- 'R': Get sensor reading
- 'ESC': Stop robot and exit

## Mapping Parameters

The application allows customization of:
- Grid size
- Cell size
- Sensor positioning
- Initial probability
- Measurement tolerance

## Probabilistic Mapping

The system uses log-odds transformation to:
- Handle sensor uncertainty
- Update cell probabilities
- Represent environment state

## Visualization

- Real-time grid visualization
- Color-coded probability representation
- Robot position marker
