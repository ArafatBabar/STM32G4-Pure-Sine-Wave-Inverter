# STM32G4-Pure-Sine-Wave-Inverter
![alt text](inverter.png)

A 1kW Two-Stage Pure Sine Wave Inverter based on the STM32G474 microcontroller.

The project converts a three-phase AC source into a regulated 400V DC link and then generates a low-distortion 230V RMS 50Hz pure sine wave output using SPWM-controlled full-bridge inverter topology.

## Specifications

| Parameter | Value |
|------------|------------|
| Output Power | 1kW Peak |
| Continuous Power | 800W |
| Output Voltage | 230V RMS |
| Output Frequency | 50Hz |
| DC Bus Voltage | 400V |
| Switching Frequency | 20kHz |
| Controller | STM32G474QETx |
| Modulation | Unipolar SPWM |
| Output Filter | LC Low Pass |
| Target THD | <3% |

## System Architecture

3 Phase AC
      │
      ▼
Rectifier
      │
      ▼
400V DC Link
      │
      ▼
Full Bridge Inverter
      │
      ▼
LC Filter
      │
      ▼
230V RMS 50Hz Output

## Features

- STM32G474-based control system
- 20kHz SPWM generation
- Isolated gate drivers
- Current sensing
- Voltage sensing
- LC output filtering
- High-voltage DC link architecture
- Modular PCB design
- Future-ready closed-loop control architecture

## Hardware Overview

### Power Stage
- Full bridge MOSFET inverter
- 400V DC bus
- LC output filter

### Controller Board
- STM32G474QETx
- ADC-based sensing
- PWM generation

### Gate Driver Board
- UCC21520 isolated gate driver

### Auxiliary Power Supply
- High-voltage DC/DC converter
- Isolated supplies

## Development Timeline

1. Topology selection
2. Simulation in PSIM
3. Schematic design
4. PCB design
5. Fabrication
6. Assembly
7. Firmware development
8. Hardware validation
9. Final testing

## Team

Project Team:

- Arafat Babar
- Vedant Acharya
- Krisha Pandya
- Ketan Pitroda
- Dev Bhavsar
- Yash Patel
- Raj Gediya
- Pritha Patel

Guides:

- Prof. Ketan Bhavsar
- Prof. Ankit Chauhan