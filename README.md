# Arduino Heartbeat Monitor using Pulse Sensor

This project measures heart rate (BPM - Beats Per Minute) using an Arduino Uno and a Pulse Sensor. The BPM is calculated in real time and displayed on a 16x2 LCD using an I2C module.

## Components Used

- Arduino Uno
- Pulse Sensor
- 16x2 LCD Display with I2C Module
- Jumper Wires
- Breadboard (optional)

## Circuit Connections

### Pulse Sensor

| Sensor Pin | Arduino Pin |
|------------|-------------|
| VCC        | 5V          |
| GND        | GND         |
| Signal     | A0          |

### LCD I2C

| LCD Pin | Arduino Pin |
|--------|-------------|
| VCC    | 5V          |
| GND    | GND         |
| SDA    | A4          |
| SCL    | A5          |

## Working Principle

The pulse sensor works on the principle of **Photoplethysmography (PPG)**.  
It detects changes in blood volume in the fingertip using light. When the heart pumps blood, the reflected light intensity changes. The sensor converts these changes into electrical signals.

The Arduino reads these analog signals and calculates the time between heartbeats. Using this time difference, the Beats Per Minute (BPM) is calculated and displayed on the LCD.

## Features

- Real-time heart rate monitoring
- BPM calculation using Arduino
- LCD display output
- Noise filtering using threshold detection
- BPM averaging for stable readings

## Output

The LCD displays the heart rate as:

BPM: XX

where XX is the measured beats per minute.

## Author

Sarthak Arya# arduino-heartbeat-monitor
