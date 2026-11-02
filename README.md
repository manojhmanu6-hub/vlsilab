# VLSI Laboratory Projects Collection

<p align="center">
  <a href="https://github.com/manojhmanu6-hub/vlsilab-projects">
    <img src="https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge&logo=github" alt="GitHub Repository">
  </a>
  <img src="https://img.shields.io/badge/Domain-VLSI%20Design-blue?style=for-the-badge" alt="VLSI Design">
  <img src="https://img.shields.io/badge/Language-Verilog%2FVHDL-orange?style=for-the-badge" alt="Verilog/VHDL">
  <img src="https://img.shields.io/badge/Tools-Xilinx%20Vivado%2FModelSim-green?style=for-the-badge" alt="EDA Tools">
</p>

## 📌 Project Overview

The **VLSI Laboratory Projects Collection** contains a comprehensive set of digital design and hardware description language (HDL) implementations developed for academic and practical experimentation in Very Large Scale Integration (VLSI) design.

This repository features modular Verilog/VHDL designs ranging from combinational arithmetic circuits and sequential blocks to complex finite state machines and communication protocols, simulated and verified using standard EDA tools.

## 🎯 Projects Included

1. **ALU (Arithmetic Logic Unit):** A multi-function arithmetic and logic unit supporting core mathematical and logical operations.
2. **4-Bit Adder:** Implementation of ripple-carry and look-ahead adders for high-speed binary addition.
3. **Traffic Light Controller:** A finite state machine (FSM) based controller managing signal transitions for automated traffic junctions.
4. **UART (Universal Asynchronous Receiver-Transmitter):** Serial communication protocol implementation featuring baud rate generation, frame formatting, and serial-to-parallel conversion.

## ✨ Key Features

- **Modular RTL Design:** Written in clean, synthesizable Verilog/VHDL following industry coding standards.
- **Testbench Verification:** Includes complete testbenches for waveform analysis and functional verification.
- **Configurable Parameters:** Parameterized bit-widths and clock dividers for easy scalability.
- **Simulation Ready:** Compatible with ModelSim, Xilinx Vivado, and QuestaSim.

## 🛠️ Components & Architecture

| Project | Core Architecture / Description | Key Submodules |
|---|---|---|
| **ALU** | Combinational & Logic Unit | Multiplexers, Adders, Shifters, Logic Gates |
| **4-Bit Adder** | Binary Adder Circuit | Full Adders, Half Adders, Carry Propagation |
| **Traffic Light Controller** | Moore/Mealy State Machine | State Transition Logic, Timer Unit |
| **UART** | Serial Communication | Transmitter, Receiver, Baud Rate Generator |

## 💻 Software & Tool Requirements

- Xilinx Vivado / ISE Design Suite
- ModelSim / QuestaSim
- Verilog / VHDL Simulator
- Git for version control

## 🔌 Pin Configuration / Interfaces

Standard digital I/O lines depending on the target FPGA or simulation testbench:
- **Clock & Reset:** Global clock input (`clk`) and synchronous/asynchronous reset (`rst`).
- **Data Buses:** Configurable input/output data buses matching project specifications (e.g., 4-bit, 8-bit).
- **Control Signals:** Mode selectors, enable flags, and trigger inputs.

## ⚙️ Working Principle

### 1. Design Entry (RTL)
Each project is structured using behavioral and structural hardware description models to define hardware logic.

### 2. Testbench Simulation
Testbenches apply stimulus vectors to inputs and monitor output responses over simulation time steps to verify correctness.

### 3. Synthesis & Implementation (Optional)
Designs can be synthesized onto target FPGA evaluation boards to validate physical timing and resource utilization.

## 🔄 General Workflow

```text
          START DESIGN
                |
                v
        Write RTL Code (.v / .vhd)
                |
                v
        Create Testbench Wrapper
                |
                v
        Run Behavioral Simulation
                |
          Waveform Correct?
              /       \
            No         Yes
            |           |
        Debug Code   Synthesis / FPGA Implementation
