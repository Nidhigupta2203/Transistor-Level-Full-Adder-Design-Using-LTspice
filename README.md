# Transistor-Level CMOS Full Adder Design Using LTspice

A 10-transistor CMOS full adder designed and simulated using LTspice with 180 nm CMOS transistor models.

## Overview

This project explores a transistor-level implementation of a 1-bit CMOS full adder. The circuit uses XOR-based sum generation and compact carry-generation logic to perform binary addition.

The project focuses on functional verification, transient response, propagation delay, and power-performance trade-offs in CMOS circuit design.

## Objectives

- Design a 10-transistor CMOS full adder.
- Implement XOR-based sum generation and carry logic.
- Simulate circuit behavior using LTspice.
- Analyze propagation delay and output waveforms.
- Study transistor-level design trade-offs and pass-transistor voltage degradation.

## Design Specifications

| Parameter | Description |
|---|---|
| Circuit | 1-bit CMOS Full Adder |
| Transistor Count | 10 |
| Technology Node | 180 nm |
| Simulation Tool | LTspice |
| Supply Voltage | 1.8 V |
| Inputs | A, B, Cin |
| Outputs | Sum, Cout |

## Full Adder Logic

The circuit accepts three 1-bit inputs: A, B, and Cin.

The outputs are defined as:

- **Sum** = A XOR B XOR Cin
- **Carry** = (A AND B) OR (Cin AND (A XOR B))

## Truth Table

| A | B | Cin | Sum | Cout |
|---|---|---|---|---|
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 |
| 0 | 1 | 0 | 1 | 0 |
| 0 | 1 | 1 | 0 | 1 |
| 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 1 | 0 | 1 |
| 1 | 1 | 0 | 0 | 1 |
| 1 | 1 | 1 | 1 | 1 |

## Tools and Technology

- LTspice for circuit design and transient simulation
- 180 nm CMOS NMOS and PMOS transistor models
- Transistor-level circuit analysis

## Repository Structure

```
Transistor-Level-Full-Adder-Design-Using-LTspice/
├── README.md
├── circuit/
│   └── CMOS_Full_Adder.asc
├── schematics/
│   └── CMOS_Full_Adder_Schematic.pdf
├── simulation/
│   ├── Output_Waveforms.pdf
│   ├── Delay_Analysis.pdf
│   └── Power_Analysis.pdf
└── images/
    ├── circuit_schematic.jpg
    └── power_analysis.jpg
```

## Simulation and Results
Transient analysis was performed in LTspice to examine the input signals and the resulting Sum and Carry outputs.
- Functional verification: Output waveforms can be checked against the full-adder truth table.
- Propagation delay: The supplied delay report shows a transition interval of approximately 184.8 ps for one measured Sum transition. This is not necessarily the worst-case delay.
- Power analysis: The supply-power waveform was examined during switching. A reliable average-power value requires checking the current sign convention and measurement interval.
  
## Key Design Considerations
- Transistor count and circuit compactness
- XOR-based Sum generation
- Carry-generation logic
- Output voltage degradation in pass-transistor logic
- Propagation delay and power trade-offs

## Future Improvements
- Measure and document worst-case propagation delay.
- Validate all input combinations and output voltage levels.
- Calculate average power using a consistent measurement method.
- Compare alternative transistor sizing configurations.
- Evaluate circuit performance across different operating conditions.

## Author
Nidhi Gupta

## Acknowledgment
This project was developed collaboratively. The repository organizes the circuit documentation and simulation analysis for portfolio presentation
