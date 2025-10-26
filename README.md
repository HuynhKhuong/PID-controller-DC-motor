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

This project implements a PID controller for precise DC motor control (In terms of Position and Velocity).

### Why I started this project

Purely just for studying and hobby! My major in University is System Control and Modeling. I dealt with Matlab and Simulink all the time. Of course all of projects are mathematical simulation of a particular system and I emploied several types of controller into such systems 
As the matter of fact, I haven't dealt with the variable of external factors (noise, environment impact) in the real model, which, to be honest, is embarassing. As consequences, The real model (in terms of hardware and software) I built during my capstone project isn't stable at all. Of course it is decent to qualify that I could pass the exam, but I do know there's spacious room for improvement. Therefore, This repository is for it! 
Besides, this is for target readers who are diving into the field of Automatic control, can refer as an example for your big assignments or your capstone project. It's nothing fancy, but it could give you insights about what you're studying.
Happy learning!

### What is PID Control?

Review my [capstone projects report](docs/BAOCAODOAN1_HuynhKhuong_1812689.pdf)
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
```

### Serial Commands

*TBD*

## PID Tuning
### Other Tuning Method
### Manual Tuning Method

1. **Start with P only**: 

2. **Add Integral**: 

3. **Add Derivative**:

### Recommended Starting Values

```
Kp = xx
Ki = xx
Kd = xx
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
- [Original capstone project from university](docs/BAOCAODOAN1_HuynhKhuong_1812689.pdf)
- Highly recommend to deep dive into [system modeling and control](https://drive.google.com/file/d/1Jd4t0ZNPOKRBkgVSiwPoOUvK1DkX8ZBU/view?usp=drive_link) 

---

