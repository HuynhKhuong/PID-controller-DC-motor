# PID Controller DC Motor

A PID (Proportional-Integral-Derivative) controller implementation for DC motor speed and position control. This project revisits and improves upon my university capstone project.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Software Requirements](#software-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [PID Tuning](#pid-tuning)
- [Circuit Diagram](#circuit-diagram)
- [Configuration](#configuration)
- [Examples](#examples)
- [Troubleshooting](#troubleshooting)
- [Acknowledgments](#acknowledgments)

## Overview

This project implements a PID controller for precise DC motor control (In terms of Position and Velocity). The PID algorithm continuously calculates an error value as the difference between a desired setpoint and a measured process variable, applying a correction based on proportional, integral, and derivative terms.

### What is PID Control?

Review my [capstone projects report](docs\BAOCAODOAN1_HuynhKhuong_1812689.pdf)
This document has well elaborated the foundational knowledge about PID controller! 

## Features

- Real-time PID control implementation
- Adjustable PID parameters (Kp, Ki, Kd)
- Motor speed and position control modes
- Real-time monitoring and data logging
- Emergency stop functionality (*Place Holder*)
- Overshoot and oscillation minimization (*Place Holder*)

## Hardware Requirements

- *Place holder*
- *Place holder*

## Software Requirements

- *Place holder* 
- *Place holder* 

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/HuynhKhuong/PID-controller-DC-motor.git
cd PID-controller-DC-motor
```

### 2. Install Dependencies

```bash
# Instructions for installing required libraries
```

### 3. Hardware Setup

1. *Place holder*
2. *Place holder*
3. *Place holder*
4. *Place holder*
5. *Place holder*

### 4. Upload the Code

1. *Place holder*
2. *Place holder*
3. *Place holder*
4. *Place holder*

## Usage

### Basic Operation

```cpp
// Example code snippet
PIDController motor(Kp, Ki, Kd);
motor.setSetpoint(targetSpeed);
motor.compute();
motor.updateMotor();
```

### Serial Commands

- `SET_SPEED <value>` - Set target speed (RPM)
- `SET_PID <Kp> <Ki> <Kd>` - Update PID parameters
- `START` - Start motor control
- `STOP` - Stop motor control
- `STATUS` - Display current status

## PID Tuning

### Manual Tuning Method

1. **Start with P only**: Set Ki and Kd to 0
   - Increase Kp until the system oscillates
   - Reduce Kp to 50-60% of this value

2. **Add Integral**: 
   - Gradually increase Ki to eliminate steady-state error
   - Watch for increased overshoot

3. **Add Derivative**:
   - Increase Kd to reduce overshoot and oscillation
   - Find the optimal balance

### Recommended Starting Values

```
Kp = 1.0
Ki = 0.1
Kd = 0.01
```

Adjust based on your specific motor and load characteristics.

## Circuit Diagram

*TBD*

## Configuration

Edit the configuration parameters in the main file or `config.h`:

```cpp
// PID Parameters
// Motor Pins
// Control Settings
```

## Examples

### Example 1: Speed Control

```cpp
// Set motor to maintain 100 RPM
```

### Example 2: Position Control

```cpp
// Move motor to 360 degrees position
```

## Troubleshooting

| Problem | Possible Cause | Solution |
|---------|---------------|----------|
| *Place Holder* | *Place Holder* | *Place Holder* |
| *Place Holder* | *Place Holder* | *Place Holder* |
| *Place Holder* | *Place Holder* | *Place Holder* |
| *Place Holder* | *Place Holder* | *Place Holder* |
| *Place Holder* | *Place Holder* | *Place Holder* |

## Acknowledgments
- [Original capstone project from university](docs\BAOCAODOAN1_HuynhKhuong_1812689.pdf)

---

