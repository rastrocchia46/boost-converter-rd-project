# High-Frequency Boost Converter R&D Project

This repository documents the design, PCB layout, prototyping and testing of a high-frequency switch-mode Boost converter developed as part of an R&D academic project.

The converter is designed as a step-up DC-DC power converter, with the main objective of converting a 12 V input voltage into a regulated 24 V output voltage. The project includes topology selection, component sizing, controller implementation, magnetic component design, PCB layout and prototype validation.

---

## Project Overview

The goal of this project is to design and build a functional Boost converter prototype and evaluate its electrical, thermal and efficiency performance.

Main project activities include:

- Definition of electrical specifications
- Component selection and sizing
- Design of the control stage based on a current-mode PWM controller
- Custom inductor design and magnetic component evaluation
- Electrical schematic design
- PCB layout design
- Prototype manufacturing and assembly
- Functional testing and validation
- Thermal and efficiency analysis

---

## Main Specifications

| Parameter | Value / Description |
|---|---|
| Input voltage | 12 V DC |
| Output voltage | 24 V DC |
| Output current | 2.5 A |
| Output power | 60 W |
| Switching frequency | 62 kHz |
| Switching period | 16.13 µs |
| Duty cycle | 50% |
| On-time | 8.065 µs |
| Inductor current ripple | 2 A |
| Output voltage ripple target | < 100 mV |
| Magnetic component | Custom inductor |

---

## Repository Structure

```text
boost-converter-rd-project/
│
├── README.md
│
├── docs/
│   └── Project documentation and schematic files
│
├── images/
│   └── PCB layout and 3D render images
│
├── hardware/
│   └── Hardware design files
│
├── simulations/
│   └── Simulation files and results
│
├── bom/
│   └── Bill of materials
│
└── reports/
    └── Technical reports and project documentation
