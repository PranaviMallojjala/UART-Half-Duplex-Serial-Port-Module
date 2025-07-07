# UART Half-Duplex Serial Port Module Design
Front-End VLSI Project (ASIC) – Verilog HDL Implementation

**Overview**
This repository demonstrates the RTL design and functional verification of a Universal Asynchronous Receiver/Transmitter (UART) module, implemented in Verilog HDL, for use in front-end ASIC workflows. UART is a widely used asynchronous serial communication protocol critical for data exchange between microcontrollers, embedded systems, SoCs, and other digital components.

The design focuses on implementing a half-duplex UART communication system capable of transmitting and receiving 8-bit data at a baud rate of 115200 bps. The project emphasizes speed, power efficiency, and FSM-based control logic. Parity handling is intentionally excluded to maintain focus on core communication logic and simplify the simulation environment.

**Key Features**
Baud rate of 115200 bps for high-speed data transfer

Standard 1 start bit, 8 data bits, 1 stop bit format

No parity bit for simplified protocol implementation

Half-duplex asynchronous communication model

RTL design in Verilog HDL following a modular and hierarchical structure

FSM-based control logic for both transmission and reception modules

Synthesizable and simulation-ready codebase

Verified through testbenches and waveform simulations using ModelSim and Vivado

Performance is evaluated based on power, thermal stability, and data integrity

**Technical Concepts Covered**
UART Protocol Design: Covers the structure and functionality of asynchronous serial communication without external clock synchronization

Bitstream Analysis: Introduction to Serial Data Packet Sniffing Techniques

Finite State Machine (FSM): Design and implementation of FSM for managing TX/RX flow control

Digital System Design (DSD): Emphasis on synthesizable RTL, modular coding, and timing optimization

Simulation and Analysis: Focus on

Power-aware communication behavior

Thermal stability during continuous transmission

High-speed and glitch-free data transfer validation

**File Structure**
graphql
Copy
Edit
├── uart_tx.v           # UART Transmitter Module
├── uart_rx.v           # UART Receiver Module
├── uart_fsm.v          # FSM Controller for UART
├── uart_tb.v           # Testbench for Simulation
├── simulation_results/ # Waveform outputs and reports
└── README.md           # Documentation

**Tools and Technologies**
Hardware Description Language: Verilog HDL

Simulation Tools: ModelSim, Xilinx Vivado

Target Platform: ASIC (Front-End RTL design)

Design Methodology: RTL modeling, simulation, and testbench-based verification

**Results and Performance**
Successfully implemented and verified UART module at 115200 bps

FSM-controlled TX and RX units exhibited stable, deterministic behavior

Efficient toggling control reduced unnecessary switching activity, contributing to power optimization

Design remained thermally stable and operational across simulation scenarios

Ready for integration into SoC design or FPGA platforms

**Future Improvements**
Integration of parity bit and error detection mechanisms

Development of a configurable baud rate generator

Extension to full-duplex communication protocol

Migration to SystemVerilog and UVM-based automated verification

**Conclusion**
This project showcases core skills in digital logic design, asynchronous communication, and Verilog-based RTL development, providing a strong foundation for roles in RTL design, ASIC front-end development, and verification engineering.
