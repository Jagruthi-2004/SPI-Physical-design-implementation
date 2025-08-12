# SPI-Physical-design-implementation

## Overview
This project implements the **Serial Peripheral Interface (SPI) protocol** in Verilog and takes it through the **complete VLSI Physical Design (PD) flow** using **Qflow**.  
The implementation includes synthesis, placement, routing, and timing closure, resulting in a GDSII layout ready for fabrication.

## Features
- RTL design of SPI protocol in Verilog.
- Fully synthesizable design targeting ASIC implementation.
- Physical design using **Qflow**:
  - Synthesis with Yosys.
  - Placement and routing with GrayWolf & QRouter.
  - Layout verification with Magic VLSI.
- Timing analysis for meeting design constraints.

## Tools & Technologies
- **HDL**: Verilog
- **PD Tools**: Qflow, Yosys, GrayWolf, QRouter, Magic VLSI
- **Simulation**: Questa Sim
- **Verification**: Testbenches in Verilog

## How It Works
SPI is a synchronous serial communication protocol used for short-distance communication between a master and one or more slaves.  
This implementation supports:
- Full-duplex communication.
- Configurable clock polarity (CPOL) and phase (CPHA).
- Parameterizable data width.

## Project Flow
1. **RTL Design**  
   Write SPI master and slave modules in Verilog.

2. **RTL Simulation**  
   Run functional verification with testbenches and view waveforms in Questa Sim.

3. **Synthesis**  
   Use Yosys to generate the gate-level netlist.

4. **Placement & Routing**  
   Perform floorplanning, placement, and routing with GrayWolf & QRouter.

5. **Layout Verification**  
   Check DRC and LVS using Magic VLSI.

## Results
- Functional RTL verified via simulation.
- Gate-level netlist generated with successful synthesis.
- Fully routed GDSII layout ready for fabrication.

## Repository Structure
