# IR-Based Parking Management System
> Efficient vehicle tracking through digital counter technology

## System Overview
This project implements a comprehensive parking management solution using infrared (IR) sensors and digital counters. The system provides real-time monitoring of vehicle entry and exit, enabling accurate occupancy tracking for parking facilities of various sizes.

### Key Features
* **Bidirectional counting**: Accurate tracking of both entering and exiting vehicles
* **IR sensor detection**: Reliable vehicle presence detection
* **Digital display interface**: Clear occupancy indicators
* **Multiple counter implementations**: CD40110, 74LS192, and 74LS191 options
* **Threshold alerts**: Configurable capacity warnings

## Hardware Architecture

### Core Components
- IR LED emitter and photodiode pairs
- LM358 operational amplifier comparators
- Digital counter ICs (CD40110/74LS192/74LS191)
- 7-segment LED displays
- Power regulation circuitry


┌───────────┐    ┌───────────┐    ┌───────────┐
│ IR Sensors │───>│ Signal    │───>│ Counter   │
│ (Entry)    │    │ Processing│    │ Circuits  │
└───────────┘    └───────────┘    └─────┬─────┘
│
┌───────────┐    ┌───────────┐    ┌─────▼─────┐
│ IR Sensors │───>│ Signal    │───>│ Display   │
│ (Exit)     │    │ Processing│    │ System    │
└───────────┘    └───────────┘    └───────────┘

> **Implementation Tip**: Use Schmidt trigger buffers for mechanical button interfaces to eliminate bounce effects.

## Video Tutorial Series
For detailed implementation guides and troubleshooting, visit our YouTube channel:
[Digital Systems Engineering](https://www.youtube.com/playlist?list=PLrZbkNpNVSwy9fEkcHNX9e-MsvJz9Zem-)
