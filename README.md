# Round Robin Arbiter Using Verilog

## Overview

This project implements a **Round Robin Arbiter** in Verilog, designed to manage fair access to shared resources in digital systems. The arbiter ensures that multiple competing entities (such as processors, memory modules, or I/O devices) are granted access in a cyclic, fair, and starvation-free manner. The project includes design, simulation, and performance analysis, and was developed as part of the B.Tech requirements at Rajiv Gandhi University of Knowledge and Technologies, RK Valley, Kadapa[1].

---

## Table of Contents

- [Introduction](#introduction)
- [Objectives](#objectives)
- [Scope](#scope)
- [Working Principle](#working-principle)
- [Arbitration Steps](#arbitration-steps)
- [Software Used](#software-used)
- [Project Structure](#project-structure)
- [Contributors](#contributors)
- [Acknowledgements](#acknowledgements)

---

## Introduction

Efficient management of shared resources is essential for optimal digital system performance. The **Round Robin Arbiter** is a hardware mechanism that allocates resources among multiple entities in a cyclic order, ensuring fairness and eliminating starvation. It is widely used in multi-processor systems, multi-core CPUs, memory controllers, and I/O management[1].

---

## Objectives

- Design and implement a Round Robin Arbiter for fair resource allocation.
- Simulate and verify the arbiter's functionality under various scenarios.
- Analyze the advantages and limitations of the round robin scheme.
- Demonstrate fairness and avoidance of starvation in resource allocation[1].

---

## Scope

- **Design:** Hardware-based arbiter using sequential logic, granting access in rotating order.
- **Simulation & Testing:** Test with simultaneous, single, and no-request scenarios using simulation tools.
- **System Integration:** Integrate into a basic bus system for demonstration.
- **Performance Analysis:** Assess fairness, response time, and efficiency[1].

---

## Working Principle

1. **Request Inputs:** Multiple entities send requests via dedicated lines.
2. **Grant Outputs:** Arbiter grants access to one entity at a time via grant lines.
3. **Round Robin Cycle:** Grants access in a cyclic order to maintain fairness.
4. **Reset/Refresh:** After each grant, the arbiter waits for new requests and resets the cycle as needed[1].

---

## Arbitration Steps

1. **Request:** Each input sends a request to the arbiter.
2. **Grant:** Arbiter grants access based on the next entity in the round-robin schedule.
3. **Accept:** Granted entity accepts, pointer updates for the next cycle.

The round robin protocol guarantees fairness, prevents starvation, and allows for predictable worst-case wait times (proportional to the number of requestors minus one)[1].

---

## Software Used

- **Xilinx Vivado:** Advanced FPGA design and analysis suite used for:
  - RTL design with Verilog/VHDL
  - IP integration and block design
  - High-level synthesis (HLS)
  - Simulation and debugging
  - Synthesis and implementation for Xilinx FPGAs[1]

---

## Project Structure

- `src/` — Verilog source code for the arbiter
- `sim/` — Testbenches and simulation waveforms
- `docs/` — Project documentation and report

---

## Contributors

- **B. Hemanjali** (R200209)
- **K. Harshitha** (R200376)
- **J. Sravya** (R200366)
- **Guide:** Mr. A. Ramesh, Assistant Professor, RGUKT RK Valley[1]

---

## Acknowledgements

We thank our guide Mr. A. Ramesh for his valuable guidance, Mr. Y. Arun Kumar (Head of Department), the management, our parents, and friends for their support throughout this project[1].

---

## License

This project was submitted in partial fulfillment of the requirements for the B.Tech degree at RGUKT, RK Valley. All rights reserved by the authors and institution[1].

---

*For detailed design, source code, and simulation results, refer to the full project report.*
