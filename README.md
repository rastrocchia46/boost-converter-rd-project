# High-Frequency Boost Converter R&D Project

This repository documents the design, PCB layout, prototyping and testing of a high-frequency switch-mode Boost converter developed as part of an R&D academic project.

The converter is designed as a step-up DC-DC power converter, with the main objective of converting a 12 V input voltage into a regulated 24 V output voltage. The project includes topology selection, component sizing, controller implementation, magnetic component design, PCB layout and prototype validation.

---

## Project Overview

The goal of this project is to design and build a functional Boost converter prototype and evaluate its electrical, thermal and efficiency performance.

Main project activities include:

- Review of common switch-mode power converter topologies
- Selection of the Boost converter topology
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

| Parameter | Target / Description |
|---|---|
| Converter topology | Boost converter |
| Input voltage | 12 V DC |
| Output voltage | 24 V DC |
| Control method | Current-mode PWM control |
| PWM controller | UC3843 |
| Power switch | N-channel MOSFET |
| Magnetic component | Custom inductor |
| PCB type | Custom PCB prototype |
| Main analysis | Electrical performance, thermal behaviour and efficiency |

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
