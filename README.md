# Smart Hair Dryer

## Overview

A smart hair dryer based on STM32 that automatically controls fan speed and heater output using distance and moisture sensing.

## Features

- PWM fan and heater control
- Distance-based detection
- Moisture-based control
- control status display with PC
- Mobile app integration (planned)

## Power Architecture

The system is powered by a 12V DC adapter.

Power conversion:
- 12V → 5V using LM2596 Buck Converter Module
- 5V → 3.3V using AMS1117-3.3 LDO

Power distribution:
- STM32F411RE : 5V
- VL53L0X : 3.3V
- MLX90614 : 3.3V
- PWM Fan, heater : 12V

## Hardware

- WeAct STM32F411
- VL53L0X Distance Sensor
- MLX90614 temperature Sensor
- PTC Heater Module
- PWM Fan, Heater

## Software

- STM32CubeIDE
- C Language
- Git
- GitHub

## System Architecture

1. Measure the distance between the dryer and the user's hair
2. Measure hair temperature level
3. Adjust fan speed automatically
4. Adjust heater output automatically
5. Display system status on PC
6. Send monitoring data to mobile application
