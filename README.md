# Roctara – A Wall Climbing Inspection Robot

Roctara is the second-generation version of our earlier Wall Climbing Robot (WCR) project, 
rebuilt from the ground up with a more compact, modular design, an improved suction 
mechanism, and a more advanced control methodology. This repository documents both the 
original prototype and its evolution into Roctara.

---

## 🧭 Project Evolution

### Version 1 – Wall Climbing Robot (WCR)
The first prototype validated the core concept of vertical climbing using a 
**propeller-based suction mechanism** paired with basic embedded motor control.

**What it achieved:**
- ✅ Vertical surface climbing (prototype stage)
- ✅ Embedded motor driver and microcontroller control
- ⚠️ Adhesion mechanism functional but unstable over long climbs

**Limitations that led to the redesign:**
- Propeller-based suction produced inconsistent adhesion force, especially over longer climbs
- Weight distribution affected balance on vertical walls
- Power consumption was higher than expected during sustained climbing
- Chassis design was bulky, not modular, and hard to iterate on
- Control responsiveness dropped off at steep angles
- No wireless control — manual/wired only

These limitations were the main motivation for a redesign: the team wanted a platform that 
was **more compact, more modular, produced stronger and more consistent suction, and used a 
more advanced control methodology.**

### Version 2 – Roctara
Roctara addresses each of these limitations directly:

- **EDF-based suction** (replacing the propeller-based mechanism) for stronger, more 
  consistent adhesion
- **Modular design architecture** — components can be swapped/upgraded independently, 
  making iteration and maintenance far easier than the monolithic V1 chassis
- **RF transmitter-receiver based control** for reliable wireless operation
- **High-torque N20 gear motors** for improved movement precision and control at steep 
  angles
- **ROS integration** — early-stage implementation and simulation (Gazebo) toward 
  autonomous navigation

---

## 🚀 Features (Planned & Implemented)

| Feature | V1 (WCR) | V2 (Roctara) |
|---|---|---|
| Suction mechanism | Propeller-based | ✅ EDF-based |
| Chassis design | Fixed/bulky | ✅ Modular & compact |
| Control | Wired/manual | ✅ RF transmitter-receiver |
| Motors | Standard DC | ✅ High-torque N20 gear motors |
| Autonomy | Not implemented | 🛠️ ROS integration (in progress) |
| Simulation | None | ✅ Gazebo simulation |

---

## 📂 Repository Structure
- `code/` → Source code (microcontroller/embedded C/Arduino)
- `docs/` → Documentation, diagrams, and design notes
- `media/` → Images, GIFs, and videos of both prototypes
- `simulation/` → ROS/Gazebo simulation files
- [`ROADMAP.md`](ROADMAP.md) → Planned improvements and development roadmap

---

## 📸 Project Media
*(V1 and V2 images/videos go here)*

---

## 🛠️ Tech Stack
- **Hardware (V2):** N20 high-torque gear motors, EDF suction unit, RF transmitter-receiver 
  module, modular chassis
- **Hardware (V1):** Propeller-based suction, standard motor drivers
- **Software:** Embedded C / Arduino IDE, ROS (in progress)
- **Tools:** CAD for chassis design, Gazebo simulation

---

## 📌 Applications
- Inspection of vertical structures (walls, tanks, bridges)
- Surveillance in urban or industrial environments
- Disaster rescue in collapsed or unsafe structures

---

## ⚠️ Project Status
Roctara (V2) is **under active development**. Current work is focused on refining the ROS 
integration, validating suction performance across surface types, and finalizing the 
modular chassis assembly.

Detailed roadmap: 👉 [`ROADMAP.md`](ROADMAP.md)
