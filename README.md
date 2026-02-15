🚀 Behavioral DRAM Model — Verilog HDL

A simulation-based implementation of a Dynamic Random Access Memory (DRAM) architecture built using Verilog HDL, demonstrating real memory access behavior including row/column addressing, read/write cycles, and bidirectional data bus control.

📌 Project Overview

Modern digital systems rely heavily on high-density memory devices. This project recreates the functional behavior of a DRAM chip at RTL level to understand how processors and memory controllers communicate with dynamic memory.

Unlike simple RAM models, this design mimics real DRAM operation using:

Multiplexed addressing

RAS/CAS timing control

Byte-select write operations

Tri-state data bus behavior

The goal of this project is to bridge the gap between textbook memory theory and practical hardware simulation.

✨ Key Features

✅ 256K × 16 Behavioral DRAM model
✅ Row & Column multiplexed addressing
✅ RAS (Row Address Strobe) operation
✅ CAS (Column Address Strobe) operation
✅ Read and Write cycle implementation
✅ Upper-byte & Lower-byte selective writes
✅ Bidirectional tri-state DATA bus
✅ Refresh behavior representation
✅ Structured verification using testbench
✅ Clean RTL design methodology

🧠 What This Project Demonstrates

This project models how real DRAM works internally:

Row Address  → Latched using RAS
Column Addr  → Selected using CAS
WE Control   → Determines Read / Write
OE Control   → Enables output driving
DATA Bus     ↔ Bidirectional communication


It provides practical insight into:

Memory controller interaction

Dynamic memory timing concepts

Hardware-level data flow

Simulation-based verification

🏗️ Project Structure
Behavioral-DRAM/
│
├── DRAM.v
├── DRAM_tb.v
└── README.md

⚙️ Simulation Setup

Open Xilinx Vivado

Add files under Simulation Sources

Run Behavioral Simulation

Observe waveform timing for:

RAS/CAS sequencing

Write cycle

Read cycle

DATA bus transitions

📊 Expected Waveform Behavior

DATA bus remains High-Z when output disabled

Write cycle stores incoming data into memory

Read cycle outputs stored data onto DATA bus

Proper RAS → CAS timing sequence

🧰 Tools Used

Verilog HDL

Xilinx Vivado Simulator

RTL Behavioral Modeling

Digital Memory Design Concepts

⚠️ Important Note

This is a behavioral DRAM model intended for simulation and learning purposes only.

Due to large memory size, the design is not synthesizable on FPGA hardware and should be used strictly for verification and educational exploration.

🎯 Learning Outcomes

Through this project, I gained hands-on experience with:

DRAM architecture fundamentals

Address multiplexing techniques

Bidirectional bus design

Memory timing control

RTL verification workflow

Debugging using waveform analysis

🔮 Future Improvements

DRAM Controller design

Burst read/write support

Timing parameter modeling

FPGA BRAM-based synthesizable version

🤝 Contributions

Suggestions, improvements, and discussions are welcome!

⭐ If you find this project useful, consider giving it a star!
