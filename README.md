# ESP32 Smart Temperature Monitoring System

## Overview
A simple embedded system using ESP32 and DHT11 to measure temperature and humidity. The readings are displayed on the Serial Monitor and an alert is generated when the temperature crosses a set limit.

## Components
- ESP32 Development Board
- DHT11 Temperature & Humidity Sensor
- Buzzer
- Jumper wires
- Breadboard
- USB cable

## Connections
| DHT11 | ESP32 |
|---|---|
| VCC | 3.3V |
| DATA | GPIO 4 |
| GND | GND |

Buzzer:
- Positive -> GPIO 5
- Negative -> GND

## Arduino Library
Install the `DHT sensor library` by Adafruit and its dependency `Adafruit Unified Sensor` from Arduino IDE Library Manager.

## Working
1. ESP32 reads temperature and humidity from DHT11.
2. Values are printed to the Serial Monitor.
3. If temperature is above 35°C, the buzzer is activated.
4. Otherwise, the buzzer remains OFF.

## How to Run
1. Open `src/main.ino` in Arduino IDE.
2. Select your ESP32 board.
3. Install the required DHT library.
4. Connect the hardware.
5. Upload the code.
6. Open Serial Monitor at 115200 baud.

## Future Improvements
- Add OLED display.
- Send readings to a mobile/web dashboard.
- Store readings in the cloud.
- Add MQTT/IoT connectivity.

## Project Type
ECE | Embedded Systems | IoT
