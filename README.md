# TIA_PORTAL_
# 🏭 Biscuit Production Line – Factory I/O + TIA Portal + HMI

This project simulates a smart biscuit production system using **Factory I/O**, **Siemens S7-1500 PLC**, and an **HMI interface** developed with **TIA Portal**. It enables real-time control, monitoring, and performance tracking of three biscuit types: *Biscuit Sec*, *Biscuit Chocolat*, and *Biscuit Vanille*.

---

## 🔧 System Description

### 💻 Tools Used

- **Factory I/O** – 3D simulation of the biscuit production line
- **TIA Portal** – PLC and HMI development (Siemens S7-1500)
- **HMI Panel** – For system interaction and display
- **PLCSIM Advanced** – Simulation of the PLC controller

---

## ⚙️ System Functionality

- Count and track the number of each biscuit type produced
- Allow operator to select biscuit orders from the HMI
- Start/Stop system via push buttons
- Emergency stop for safety
- Real-time indicators of production performance

---

## 📊 Performance Indicators

| **Indicator**        | **Description**                                             | **Calculation**                          |
|----------------------|-------------------------------------------------------------|-------------------------------------------|
| `Quantité produite`  | Total number of biscuits produced (all types combined)      | Sum of BS + BC + BV                       |
| `Temps`              | Total production time                                       | Clock timer or system timer               |
| `Débit`              | Production rate in biscuits/minute                          | `Quantité produite / Temps`               |
| `num de gamme`       | Production batch or order number, manually entered or set   | Updated by operator via HMI               |

Displayed live on the HMI using numerical displays.

---

## 🖥️ HMI Overview

### Main View (Default)

| **Element**           | **Function**                        |
|------------------------|-------------------------------------|
| Emergency Stop Button  | Stops all processes immediately     |
| Start Button           | Starts the production cycle         |
| Indicator Lights       | Show system status (running/stopped)|
| Biscuit Selectors      | Choose type: Sec, Chocolat, Vanille |
| Order Selectors        | Set order mode for each type        |
| Displays               | Show: Count, Time, Débit, Gamme     |

### View Hierarchy

