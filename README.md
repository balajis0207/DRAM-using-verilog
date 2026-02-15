Behavioral DRAM Model using Verilog HDL

This project implements a Behavioral Dynamic Random Access Memory (DRAM) model using Verilog HDL. The design emulates the functional behavior of a real DRAM device, including row and column addressing, read/write operations, and bidirectional data bus control.

The model is intended for simulation and educational purposes, enabling verification of memory controller logic and understanding of DRAM timing concepts.

Features

256K × 16 DRAM behavioral model

Multiplexed address input (Row Address + Column Address)

RAS (Row Address Strobe) and CAS (Column Address Strobe) operation

Read and write cycle implementation

Upper-byte and lower-byte write enable support

Tri-state bidirectional DATA bus

Refresh behavior modeling

Simulation-ready RTL design

Project Structure
DRAM/
│
├── DRAM.v        # Behavioral DRAM model
├── DRAM_tb.v     # Testbench for verification
└── README.md

Simulation

The design is verified using Xilinx Vivado behavioral simulation.

Simulation validates:

Row address latching

Column address access

Write cycle operation

Read data retrieval

DATA bus tri-state behavior

Key Concepts Covered

DRAM architecture fundamentals

Memory addressing techniques

RTL behavioral modeling

Bidirectional bus design

Digital memory timing

Hardware verification using testbenches

Tools Used

Verilog HDL

Xilinx Vivado Simulator

Applications

Memory controller verification

Digital system simulation

Processor memory interface studies

FPGA and ASIC learning projects

Note

This DRAM model is behavioral and intended for simulation purposes only. It is not meant for FPGA synthesis due to large memory size constraints.
