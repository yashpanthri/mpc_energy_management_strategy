# mpc_energy_management_strategy
This project contains a non linear hybrid vehicle model which includes MPC and rule based Energy Management Strategies.

# Energy Optimization of a P2 Parallel PHEV using MPC

This repository contains a MATLAB/Simulink implementation of an energy
management strategy for a **P2 parallel plug-in hybrid electric vehicle (PHEV)**.
The project compares a baseline **50–50 rule-based controller** with an
**updated Linear Time-Invariant Model Predictive Control (MPC)** strategy.

The final results, discussion, conclusions, and future work are documented
in the included report.
<img width="1851" height="839" alt="image" src="https://github.com/user-attachments/assets/1ac79aa1-0d50-4194-a490-e221a6146675" />

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

## Repository Contents 
Key files:
- `Vehicle_model_mpc_updated.slx` – Final MPC model used for results
- `Vehicle_model_old_mpc.slx` – Older MPC formulation
- `Vehicle_model_without_controller.slx` – Plant model with 50-50 controller
- `FC_SI63_emis.m` – Engine model (ADVISOR based)
- `MC_PM49.m` – Motor model (ADVISOR based)
- `report.pdf` – Concise report
- `plots` – Result plots included under this folder

---

## How to Run the Project

### 1) Open MATLAB
Open MATLAB **with the repository root as the current folder**.

### 2) Add Project to Path
Run:
```matlab
uddscycle_and_parameters_simulated_motor_map
Vehicle_model_mpc_updated.slx 
```
Details of mathematical modelling can be found in:
```
report.pdf
old_control_math.pdf
```
Drive Cycle is from UDDS:
```
uddscol.txt
```
