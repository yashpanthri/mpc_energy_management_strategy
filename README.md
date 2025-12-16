# mpc_energy_management_strategy
This project contains a non linear hybrid vehicle model which includes MPC and rule based Energy Management Strategies.

# Energy Optimization of a P2 Parallel PHEV using MPC

This repository contains a MATLAB/Simulink implementation of an energy
management strategy for a **P2 parallel plug-in hybrid electric vehicle (PHEV)**.
The project compares a baseline **50–50 rule-based controller** with an
**updated Linear Time-Invariant Model Predictive Control (MPC)** strategy.

The final results, discussion, conclusions, and future work are documented
in the included project report.

---

## Project Overview

- Backward-looking longitudinal vehicle model
- ADVISOR-based engine and motor efficiency maps
- Power-based battery SOC model
- Comparison of:
  - 50–50 rule-based energy management
  - MPC-based energy management (final updated formulation)

Drive cycle used: **UDDS (Urban Dynamometer Driving Schedule)**  
Simulation time step: **1 s**

---

## Repository Contents (As-Is)

This repository intentionally preserves the original folder structure to
avoid MATLAB/Simulink path issues.

Key files:
- `Vehicle_model_mpc_updated.slx` – **Final model used for results**
- `Vehicle_model_old_mpc.slx` – Older MPC formulation (legacy)
- `Vehicle_model_without_controller.slx` – Plant-only model
- `FC_SI63_emis.m` – Engine model (ADVISOR based)
- `MC_PM49.m` – Motor model (ADVISOR based)
- `AENG 562_Project Report.pdf` – Final report (results + conclusions)
- `pics/` – Result figures used below

---

## How to Run the Project

### 1) Open MATLAB
Open MATLAB **with the repository root as the current folder**.

### 2) Add Project to Path
Run:
```matlab
uddscycle_and_parameters_simulated_motor_map
Vehicle_model_mpc_updated.slx 
