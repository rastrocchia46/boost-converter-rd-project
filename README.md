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

## Converter Architecture

The power stage includes: input protection section, input capacitor bank, custom-designed inductor, power MOSFET, Schottky rectifier diode and an output capacitor bank.

The control stage is based on the UC3843 current-mode PWM controller. The controller drives the MOSFET gate and regulates the output voltage through a feedback network. The current sensing network provides the controller with information about the switch current, enabling current-mode operation and cycle-by-cycle current control.

---


## Schematic

The electrical schematic of the Boost converter is available in the documentation folder:

[Open schematic PDF](docs/Schematic%20Boost%20Converter.pdf)

---

## PCB Layout

The PCB was designed as a custom prototype board for practical validation of the converter. Particular attention was given to the placement of the main power components, current paths, input/output capacitor positioning and test-point accessibility. The main power path was routed with wide copper areas to reduce resistive losses and improve current handling. The inductor, MOSFET, Schottky diode and output capacitors were placed to keep the high-current switching loop as compact as possible.

### Front PCB Layout

![Front PCB Layout](images/Front%20-%20Boost%20Converter.png)

### Rear PCB Layout

![Rear PCB Layout](images/Rear%20-%20Boost%20Converter.png)

### 3D PCB View

![3D PCB Layout](images/3D%20layout%20-%20Boost%20Converter.png)

---

## Custom Inductor

A key part of the project is the design and construction of a custom magnetic component for the Boost converter. The inductor was designed according to the required current ripple, switching frequency and output power of the converter.

The inductor design process includes:

- Calculation of the required inductance
- Selection of the magnetic core
- Evaluation of saturation limits
- Definition of the number of turns
- Consideration of copper losses
- Practical winding and assembly of the magnetic component

The custom inductor will also be evaluated during prototype testing, with attention to thermal behaviour and its influence on converter efficiency.

---

## Authors

**Raffaele Strocchia**  
**Salvatore Turboli**
**Domenico Fiorinelli**
MSc Electronic Engineering students  
Double Degree Program  
University of Naples Federico II / Lodz University of Technology

---

This repository is part of an academic R&D project and is intended to document the engineering workflow followed during the development of the converter.

Further updates will be added after PCB manufacturing, assembly and prototype testing.
