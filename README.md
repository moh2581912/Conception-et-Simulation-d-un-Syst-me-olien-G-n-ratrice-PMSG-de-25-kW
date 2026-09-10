# 🌬️ 25 kW Wind Energy Conversion System

<p align="center">
  <img src="system_architecture.png" alt="25 kW Wind Energy Conversion System" width="900"/>
</p>

<h3 align="center">
  Modeling, Control and Simulation of a Grid-Connected PMSG-Based Wind Energy Conversion System
</h3>

<p align="center">
  <img src="https://img.shields.io/badge/MATLAB-R202x-orange?logo=mathworks" />
  <img src="https://img.shields.io/badge/Simulink-Modeling-blue?logo=mathworks" />
  <img src="https://img.shields.io/badge/Power%20Electronics-AC%2FDC%20%7C%20DC%2FAC-green" />
  <img src="https://img.shields.io/badge/Renewable%20Energy-Wind-brightgreen" />
  <img src="https://img.shields.io/badge/Power-25%20kW-red" />
</p>

---

## 📌 Overview

This project presents the **modeling, control, and simulation of a 25 kW grid-connected Wind Energy Conversion System (WECS)** based on a **Permanent Magnet Synchronous Generator (PMSG)**.

The complete conversion chain is developed in **MATLAB/Simulink**, from wind energy extraction to electrical power injection into the grid.

The system integrates:

- 🌬️ 25 kW wind turbine
- ⚡ Permanent Magnet Synchronous Generator (PMSG)
- 🔄 AC/DC machine-side converter
- 🔋 DC-link
- 🔄 DC/AC grid-side converter
- 🎯 MPPT control
- 🎛️ Machine-side control
- ⚡ Grid-side control
- 📊 RMS and THD analysis
- 🔌 Active and reactive power control

---

## ⚙️ System Architecture

```text
                    WIND ENERGY
                         │
                         ▼
                ┌─────────────────┐
                │  Wind Turbine   │
                │      25 kW      │
                └────────┬────────┘
                         │
                    Mechanical
                      Power
                         │
                         ▼
                ┌─────────────────┐
                │      PMSG       │
                │ Permanent Magnet│
                │    Generator    │
                └────────┬────────┘
                         │ 3-Phase AC
                         ▼
                ┌─────────────────┐
                │     AC → DC     │
                │ Machine-Side    │
                │   Converter     │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │     DC-LINK     │
                │      Vdc        │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │     DC → AC     │
                │   Grid-Side     │
                │   Converter     │
                └────────┬────────┘
                         │ 3-Phase AC
                         ▼
                ┌─────────────────┐
                │      GRID       │
                └─────────────────┘
