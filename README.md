# Synchronous FIFO Verification using SystemVerilog & UVM

> A reusable UVM-based verification environment for validating a Synchronous FIFO using SystemVerilog, featuring constrained-random verification, functional coverage, self-checking scoreboards, and assertion-based verification.

---

## Overview

This project implements a comprehensive UVM verification environment for a Synchronous FIFO (First-In, First-Out) memory. The verification environment is designed using industry-standard methodologies to verify FIFO functionality under various operating conditions, including normal operation, boundary conditions, and overflow/underflow scenarios.

The testbench is modular, reusable, and scalable, enabling efficient verification through constrained-random stimulus generation, automated result checking, functional coverage, and SystemVerilog Assertions (SVA).

---

## Project Objectives

* Verify FIFO read and write functionality
* Validate data integrity and ordering
* Verify FIFO status flags (Full, Empty, Almost Full, Almost Empty)
* Detect Overflow and Underflow conditions
* Develop a reusable UVM verification environment
* Achieve high functional coverage
* Implement assertion-based protocol checking using SVA

---

## Features

* Complete UVM Testbench Architecture
* Reusable Verification Components
* Constrained-Random Test Generation
* Self-Checking Scoreboard
* Reference Model
* Functional Coverage Collection
* SystemVerilog Assertions (SVA)
* Random Read/Write Transactions
* FIFO Flag Verification
* Boundary Condition Testing
* Automated Error Detection

---

## Technologies Used

| Technology           | Purpose                            |
| -------------------- | ---------------------------------- |
| SystemVerilog        | RTL & Verification                 |
| UVM                  | Universal Verification Methodology |
| SVA                  | Assertion-Based Verification       |
| Functional Coverage  | Coverage-Driven Verification       |
| QuestaSim / ModelSim | Simulation & Debugging             |

---

## UVM Testbench Architecture

```text
Top Testbench
│
├── Interface
│
├── Test
│
├── Environment
│   ├── FIFO Agent
│   │   ├── Sequencer
│   │   ├── Driver
│   │   └── Monitor
│   │
│   ├── Scoreboard
│   ├── Reference Model
│   ├── Coverage Collector
│   └── Assertions (SVA)
│
├── Sequences
│
└── FIFO DUT
```

---

## Repository Structure

```text
FIFO-UVM/
│
├── rtl/
├── interface/
├── transaction/
├── sequences/
├── sequencer/
├── driver/
├── monitor/
├── agent/
├── env/
├── scoreboard/
├── reference_model/
├── coverage/
├── assertions/
├── tests/
├── tb/
├── docs/
└── README.md
```

---

## Verification Components

* Interface
* Sequence Item (Transaction)
* Sequences
* Sequencer
* Driver
* Monitor
* Agent
* Environment
* Scoreboard
* Reference Model
* Functional Coverage
* SystemVerilog Assertions (SVA)
* Test Cases
* Top Testbench

---

## Test Scenarios

* FIFO Reset Verification
* Single Write Operation
* Single Read Operation
* Multiple Write Transactions
* Multiple Read Transactions
* Simultaneous Read and Write
* FIFO Full Condition
* FIFO Empty Condition
* FIFO Overflow Verification
* FIFO Underflow Verification
* Almost Full Flag Verification
* Almost Empty Flag Verification
* Random Read/Write Sequences
* Data Integrity Verification
* Boundary Condition Testing

---

## Verification Flow

```text
Sequence
      │
      ▼
Sequencer
      │
      ▼
Driver
      │
      ▼
FIFO Interface
      │
      ▼
FIFO DUT
      │
      ▼
Monitor
      │
      ├────────► Scoreboard
      ├────────► Reference Model
      ├────────► Coverage
      └────────► Assertions
```

---

## Simulation

Example simulation commands using QuestaSim/ModelSim:

```tcl
vlib work
vlog *.sv
vsim top_tb
run -all
```

---

## Skills Demonstrated

* SystemVerilog
* Universal Verification Methodology (UVM)
* FIFO Verification
* Functional Verification
* Constrained-Random Verification
* Assertion-Based Verification (SVA)
* Functional Coverage
* Self-Checking Testbench Development
* Reference Model Design
* Scoreboard Implementation
* Verification Planning
* Waveform Analysis and Debugging

---

## Future Enhancements

* Asynchronous FIFO Verification
* Parameterized FIFO Support
* UVM Register Abstraction Layer (RAL)
* Regression Automation
* Continuous Integration (CI) with GitHub Actions
* Coverage Closure Reports
* Performance and Stress Testing

---

## Author

**Gudala Chandini**

Electronics & Communication Engineering Graduate | VLSI Design Verification Enthusiast

**Areas of Interest**

* ASIC Design Verification
* SystemVerilog
* UVM
* FIFO & Memory Verification
* AMBA Protocols
* Functional Verification

---

⭐ If you find this repository helpful, consider giving it a star. Contributions, suggestions, and feedback are always welcome.


## Author

**Chandini Gudala**
