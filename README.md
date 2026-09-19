# HVAC Plant Operation & Performance Analysis

## 📌 Project Overview

This project presents a practical study and engineering analysis of the **centralized chilled-water HVAC system at IIT Indore**.

The study focused on understanding the complete operation of the HVAC plant, from the **refrigeration cycle and chilled-water generation** to **cooling tower heat rejection and conditioned-air delivery through Air Handling Units (AHUs)**.

The system serves major campus buildings including the **Library, Admin Building, and Lecture Hall Complex (LHC)**. The study covered the major components, fluid circuits, operating temperatures, heat-exchanger behaviour, and important AHU parameters.

---

## 🎯 Objectives

* Understand the complete working of a centralized chilled-water HVAC system.
* Study the refrigeration cycle inside the chiller.
* Analyse the condenser-water and cooling-tower loop.
* Understand primary and secondary chilled-water circulation.
* Study AHU operation and air-side heat transfer.
* Perform LMTD calculations for evaporator and condenser heat exchangers.
* Analyse important operating parameters such as temperature, pressure, water velocity, airflow, and static pressure.
* Compare centralized chilled-water systems with other HVAC configurations.

---

## 🏭 System Studied

The HVAC plant uses a **centralized chilled-water cooling system**.

### Major Buildings Served

| Building       | Cooling Capacity |
| -------------- | ---------------: |
| Library        |           400 TR |
| Admin Building |           450 TR |
| LHC            |           810 TR |

The system uses **R-410A and R-134A refrigerants** in the studied refrigeration systems. R-410A was identified as a higher-efficiency, lower-GWP alternative, while R-134A is a widely used HFC refrigerant.

---

# 🔄 1. Refrigeration Cycle

The refrigeration cycle consists of four major processes:

**Compressor → Condenser → Expansion Valve → Evaporator**

### Compressor

The refrigerant enters the compressor as a low-pressure vapour and is compressed to a **high-pressure, high-temperature superheated vapour**.

### Condenser

The high-temperature refrigerant rejects heat to the condenser-water circuit.

The refrigerant undergoes condensation from vapour toward the liquid state.

### Expansion Valve

The high-pressure liquid refrigerant passes through the expansion valve, producing a pressure drop and a corresponding reduction in temperature.

### Evaporator

The cold refrigerant absorbs heat from the chilled-water circuit inside the evaporator.

The chilled-water supply temperature is approximately **7°C**, while return water is approximately **12°C**.

---

# 🌡️ 2. Evaporator LMTD Calculation

For the evaporator:

* ΔT₁ = 12 − 5 = **7°C**
* ΔT₂ = 7 − 5 = **2°C**

The logarithmic mean temperature difference is:

$$
LMTD = \frac{\Delta T_1-\Delta T_2}
{\ln(\Delta T_1/\Delta T_2)}
$$

Therefore,

$$
LMTD =
\frac{7-2}{\ln(7/2)}
\approx 4°C
$$

This gives an approximate evaporator LMTD of **4°C**.

---

# 🔥 3. Condenser LMTD

For the condenser:

$$
LMTD =
\frac{10-5}{\ln(10/5)}
$$

$$
LMTD \approx 7.2°C
$$

The condenser LMTD was therefore approximately **7.2°C**.

---

# 💧 4. Condenser Water & Cooling Tower Loop

The condenser-water loop transfers heat rejected by the chiller to the cooling tower.

### Main Components

* Condenser
* Condenser pumps
* Cooling tower
* Fans
* Fill/mesh media
* Makeup-water tank
* Condenser piping

The cooling tower operates through **direct air-water contact**.

Warm condenser water enters the cooling tower, where air is drawn across the water by the fan. Heat is transferred from the water to the air.

The studied operating range was approximately:

**Cooling Tower Inlet:** 30–35°C
**Cooling Tower Outlet:** 25–30°C

---

# 💦 5. Chilled-Water System

The chilled-water system consists of two major loops:

### Primary Loop

The primary loop circulates water between the chiller and the primary circuit.

* Chiller-side flow
* Approximately constant flow
* Chilled-water supply from evaporator: **~7°C**

### Secondary Loop

The secondary loop distributes chilled water to the buildings according to cooling demand.

* Supply temperature: **~7°C**
* Return temperature: **~12°C**
* Variable flow depending on cooling load

A **decoupler/common pipe** connects the supply and return sides of the primary and secondary circuits.

### Flow Path

```text
Chiller Evaporator
        ↓
Primary Pump
        ↓
Decoupler
        ↓
Secondary Pump
        ↓
Building AHUs
        ↓
Return Water
        ↓
Decoupler
        ↓
Chiller Evaporator
```

---

# 🌬️ 6. Air-Side Cycle

The AHU transfers cooling from chilled water to the building air.

### Process

```text
Return Air
    ↓
Cooling Coil
    ↓
AHU Fan
    ↓
Duct Network
    ↓
Conditioned Space
```

Warm return air from the conditioned space enters the AHU.

The air passes over the chilled-water cooling coil, where heat is transferred from the air to the chilled water.

The AHU fan then pushes the conditioned air through the duct network.

The studied air-side parameters included:

* Chilled-water supply: **~7°C**
* Air discharge: **~12°C**
* Return-air temperature
* Airflow velocity
* Static pressure

---

# ⚙️ 7. AHU Analysis

The AHU study covered the following sections:

### Blower Section

The system specifications studied included:

* Maximum blower outlet velocity: **610 m/min**
* Minimum static pressure: **40 mm water gauge**
* Vibration isolation using rubber/neoprene pads or spring mountings

A reduction in static pressure below the required level can cause fan stalling and a significant reduction in airflow.

### Coil Section

The studied coil specifications included:

* Seamless solid-drawn copper tubes
* Copper U-bends
* Brazed tube connections
* Water velocity: **0.6–1.8 m/s**
* Maximum working pressure: approximately **10 bar**

### Filter Section

The maximum filter face velocity was approximately:

**155 m/min**

The pre-filters were designed to capture particles down to approximately **10 μm**.

---

# 📊 8. Key Parameters

| Parameter                      | Studied Value |
| ------------------------------ | ------------: |
| Chilled-water supply           |          ~7°C |
| Chilled-water return           |         ~12°C |
| Cooling tower inlet            |      ~30–35°C |
| Cooling tower outlet           |      ~25–30°C |
| Evaporator LMTD                |          ~4°C |
| Condenser LMTD                 |        ~7.2°C |
| AHU coil water velocity        |   0.6–1.8 m/s |
| AHU minimum static pressure    |      40 mm WG |
| Maximum blower outlet velocity |     610 m/min |
| Filter maximum face velocity   |     155 m/min |

---

# 🧮 9. Engineering Analysis

The project involved understanding and applying heat-transfer and HVAC engineering concepts including:

* Refrigeration cycle
* Heat exchanger operation
* Log Mean Temperature Difference (LMTD)
* Chilled-water circulation
* Condenser-water heat rejection
* Cooling tower operation
* Air-side heat transfer
* AHU operation
* Pressure and flow requirements
* Cooling-load-dependent secondary flow

The study connected the theoretical refrigeration and heat-transfer concepts with the operation of an actual centralized HVAC plant.

---

# 🔧 10. Major Components Studied

* Chillers
* Compressors
* Condensers
* Evaporators
* Expansion valves
* Cooling towers
* Condenser pumps
* Primary chilled-water pumps
* Secondary chilled-water pumps
* Decoupler
* AHUs
* Cooling coils
* Fans/blowers
* Filters
* Ducting
* Sensors and control elements

---

# 📈 11. Engineering Takeaways

### Refrigeration

Understood how the refrigerant circulates through the compressor, condenser, expansion valve, and evaporator to produce chilled water.

### Heat Transfer

Used LMTD to analyse the temperature driving force in the evaporator and condenser.

### Fluid Circuits

Understood the difference between the constant-flow primary loop and variable-flow secondary loop.

### Cooling Tower

Studied how heat rejected by the condenser is transferred to atmospheric air through direct air-water contact.

### AHU

Understood how chilled water removes heat from return air through the cooling coil before the fan distributes conditioned air through the building.

---

# 🏢 HVAC System Flow

```text
                    REFRIGERATION LOOP
                          
              ┌──────────────────────┐
              │      COMPRESSOR      │
              └──────────┬───────────┘
                         ↓
              ┌──────────────────────┐
              │      CONDENSER       │
              └──────────┬───────────┘
                         ↓
              ┌──────────────────────┐
              │   EXPANSION VALVE    │
              └──────────┬───────────┘
                         ↓
              ┌──────────────────────┐
              │      EVAPORATOR      │
              └──────────┬───────────┘
                         │
                         ↓
                 CHILLED WATER
                         │
                         ↓
                       AHU
                         │
                         ↓
                 CONDITIONED AIR
                         │
                         ↓
                    BUILDINGS
```

---

# 🛠️ Tools & Concepts

### Engineering Concepts

* Thermodynamics
* Refrigeration & Air Conditioning
* Heat Transfer
* Fluid Mechanics
* HVAC Systems
* Heat Exchangers
* Cooling Towers

### Analysis

* LMTD calculation
* Temperature analysis
* Flow-system analysis
* HVAC component analysis

---

# 📚 Project Scope

This project was primarily a **practical HVAC plant study and engineering analysis**. It focused on understanding the operation and interaction of the major HVAC components and applying thermodynamics, heat-transfer, and fluid-flow concepts to the observed system.

No CFD or detailed numerical HVAC simulation is claimed as part of this project.

---

## 👨‍🔧 Project Information

**Project:** HVAC Plant Operation & Performance Analysis
**Location:** IIT Indore Campus
**System:** Centralized Chilled-Water HVAC System
**Buildings Studied:** Library, Admin Building, LHC
**Domain:** HVAC / Thermal Engineering / Heat Transfer / Refrigeration
