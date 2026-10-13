# Transistor-Level CMOS Full Adder Design and Analysis

A 10-transistor CMOS full adder designed and evaluated using LTspice and 180 nm CMOS transistor models.

## Project Overview

This group project explores a compact transistor-level implementation of a 1-bit CMOS full adder. The design uses XOR-based sum generation and compact carry-generation logic to implement binary addition.

The project focuses on circuit functionality, transient behavior, transistor sizing, and the trade-offs associated with pass-transistor logic.

## Design Objectives

- Implement a 1-bit full adder using a 10-transistor architecture.
- Study XOR-based sum generation and carry-generation logic.
- Simulate circuit behavior using LTspice.
- Examine propagation delay and power consumption.
- Analyze output voltage behavior in pass-transistor logic.

## Circuit Functionality

The full adder accepts three inputs:

- A: First input bit
- B: Second input bit
- Cin: Carry input

It produces two outputs:

- Sum = A XOR B XOR Cin
- Cout = AB + Cin(A XOR B)

## Technology and Tools

- Circuit design: Transistor-level CMOS
- Simulation: LTspice
- Technology node: 180 nm
- Devices: NMOS and PMOS transistor models

## Simulation Methodology

1. Build or open the transistor-level schematic in LTspice.
2. Apply input signals to cover all eight input combinations.
3. Run transient analysis.
4. Compare Sum and Carry outputs with the expected truth table.
5. Inspect propagation delay and power measurements.
6. Examine output voltage levels and switching behavior.

## Analysis

The project investigates the relationship between transistor count, circuit compactness, propagation delay, and output voltage degradation.

Measured delay, power consumption, supply voltage, and transistor dimensions should be documented using the actual simulation setup and results.

## Repository Structure
```

- `circuit/`: Editable LTspice schematic
- `documentation/`: Circuit documentation
- `simulation/`: Actual waveform and analysis reports
- `images/`: Circuit and simulation screenshots
```

## Verification Status

Include only simulation results that have been reproduced or checked against the original project files. Document any model dependencies required to run the schematic.

## Project Collaboration

This project was developed collaboratively. The repository presents the circuit design and analysis in an independently organized project portfolio.

## Author

Nidhi Gupta
