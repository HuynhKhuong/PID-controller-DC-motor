# PID Controller DC Motor

A PID (Proportional-Integral-Derivative) controller implementation for DC motor speed and position control. This project revisits and improves upon a university capstone project, demonstrating advanced motor control techniques.

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
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Overview

This project implements a PID controller for precise DC motor control. The PID algorithm continuously calculates an error value as the difference between a desired setpoint and a measured process variable, applying a correction based on proportional, integral, and derivative terms.

### What is PID Control?

- **Proportional (P)**: Produces an output proportional to the current error
- **Integral (I)**: Accounts for past errors and eliminates steady-state error
- **Derivative (D)**: Predicts future errors based on the rate of change

## Features

- Real-time PID control implementation
- Adjustable PID parameters (Kp, Ki, Kd)
- Motor speed and position control modes
- Real-time monitoring and data logging
- Serial communication interface
- Emergency stop functionality
- Overshoot and oscillation minimization

## Hardware Requirements

- Microcontroller (e.g., Arduino, ESP32, STM32)
- DC Motor with encoder
- Motor driver (e.g., L298N, TB6612FNG)
- Power supply (appropriate voltage for your motor)
- Connecting wires and breadboard
- Optional: Display module for real-time monitoring

## Software Requirements

- Arduino IDE / PlatformIO / Other development environment
- Required libraries:
  - [Library Name] - for motor control
  - [Library Name] - for encoder reading
  - [Library Name] - for communication
- Serial monitor or plotting tool for data visualization

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/HuynhKhuong/PID-controller-DC-motor.git
cd PID-controller-DC-motor
```

### 2. Install Dependencies

```bash
# Instructions for installing required libraries
# Example for Arduino:
# Open Arduino IDE -> Sketch -> Include Library -> Manage Libraries
# Search and install required libraries
```

### 3. Hardware Setup

1. Connect the motor driver to your microcontroller
2. Wire the DC motor to the motor driver outputs
3. Connect the encoder to digital input pins
4. Ensure proper power supply connections
5. Verify all ground connections

### 4. Upload the Code

1. Open the project in your IDE
2. Select the correct board and port
3. Adjust configuration parameters in `config.h` (if applicable)
4. Compile and upload to your microcontroller

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

```
[Add your circuit diagram here]
```

## Configuration

Edit the configuration parameters in the main file or `config.h`:

```cpp
// PID Parameters
#define KP 1.0
#define KI 0.1
#define KD 0.01

// Motor Pins
#define MOTOR_PIN1 9
#define MOTOR_PIN2 10
#define ENCODER_A 2
#define ENCODER_B 3

// Control Settings
#define SAMPLE_TIME 10  // milliseconds
#define MAX_SPEED 255
```

## Examples

### Example 1: Speed Control

```cpp
// Set motor to maintain 100 RPM
motor.setMode(SPEED_CONTROL);
motor.setSetpoint(100);
motor.start();
```

### Example 2: Position Control

```cpp
// Move motor to 360 degrees position
motor.setMode(POSITION_CONTROL);
motor.setSetpoint(360);
motor.start();
```

## Troubleshooting

| Problem | Possible Cause | Solution |
|---------|---------------|----------|
| Motor oscillates | Kp too high | Reduce Kp value |
| Slow response | Kp too low | Increase Kp value |
| Steady-state error | Ki too low | Increase Ki value |
| Overshoot | Kd too low or Ki too high | Adjust Kd and Ki |
| Motor doesn't move | Wiring or power issue | Check connections and power supply |

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please ensure your code follows the existing style and includes appropriate documentation.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Original capstone project from university
- PID control theory resources
- Open-source community contributions
- [Add any specific references or inspirations]

## Contact

Project Link: [https://github.com/HuynhKhuong/PID-controller-DC-motor](https://github.com/HuynhKhuong/PID-controller-DC-motor)

---

**Note**: This is a template README. Please update the sections with your specific implementation details, actual hardware specifications, and code examples.
