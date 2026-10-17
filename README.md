# 🌊 AbyssalROV 3D — Red Sea Oceanographic Digital Twin & Subsea Robotics Lab

![AbyssalROV Status](https://img.shields.io/badge/Subsea_Robotics-6--DoF_Vector_Thrust-00e5ff?style=for-the-badge&logo=subversion)
![Physics Engine](https://img.shields.io/badge/Three.js-WebGL_3D-facc15?style=for-the-badge&logo=three.js)
![Oceanographic](https://img.shields.io/badge/Acoustic_Sonar-Multibeam_PPI-00ffaa?style=for-the-badge)
![Deployment](https://img.shields.io/badge/Live_Demo-GitHub_Pages-blue?style=for-the-badge&logo=github)

> **Architected & Engineered by:** [Tareq Aboushi](https://github.com/Tareq0001)  
> **Interactive Live Simulation:** [https://tareq0001.github.io/AbyssalROV-RedSea-Subsea-Twin/](https://tareq0001.github.io/AbyssalROV-RedSea-Subsea-Twin/)

---

## 🎯 Executive Vision: The Red Sea Abyssal Frontier

The Red Sea rift trench is one of the planet's most biologically and geothermally extreme marine ecosystems, plunging to depths exceeding **2,800 meters**. Featuring ultra-dense **hot brine pools (e.g. Kebrit Deep & Atlantis II Deep)**, pristine deep-water coral reefs, and active hydrothermal mineral vents, it represents the cornerstone of Saudi Vision 2030 marine research (**Red Sea Global, NEOM Sindalah, and the Farasan Marine Biosphere**).

**AbyssalROV 3D** is an institutional-grade, physics-grounded **Digital Twin and Subsea Flight Simulator** for a work-class Remotely Operated Vehicle (ROV). Designed for deep-sea robotic exploration, archaeological survey, and hydrothermal sampling.

---

## 🔬 Core Engineering & Physics Subsystems

### 1. 6-DoF Hydrodynamic Thrust Allocation Matrix
The vehicle features an **8-thruster omnidirectional vector configuration** (4 horizontal thrusters vectored at 45° angles and 4 vertical heave thrusters):
- **Surge ($X$) & Sway ($Z$):** Vector decomposition yields instant translation without rotation.
- **Heave ($Y$):** Direct ballast and vertical thruster equilibrium balancing negative syntactic foam buoyancy.
- **Fluid Drag & Hydrodynamic Damping:** Nonlinear fluid resistance modeled via the Morison equation tensor:
  $$\vec{F}_{\text{drag}} = -\frac{1}{2} \rho C_d A \|\vec{v}\| \vec{v}$$
- **Hydrostatic Pressure Simulation:** Real-time barometric computation:
  $$P_{\text{depth}} = 1.013 + \frac{\rho g h}{10^5} \quad [\text{bar}]$$

### 2. Multibeam Bathymetric Sonar (PPI 360° Acoustic Radar)
- 450 kHz acoustic phased array simulation.
- Real-time polar Plan Position Indicator (PPI) canvas renderer.
- Acoustic echo detection for hydrothermal chimneys, coral walls, and sunken Ottoman amphoras.

### 3. 5-DoF Hydraulic Manipulator Robotic Arm & Tooling
- 5-axis articulated robotic arm mounted on the starboard skid.
- Joint controls: Base Yaw, Shoulder Pitch, Elbow Pitch, and Proportional Gripper Jaw.
- **Automated Core Sampling Routine:** Downward deployment, seabed sediment penetration, core tube retrieval, and automated stowing in the payload basket.
- **Dual Green Parallel Calibration Lasers (10 cm):** Optical scale projection for measuring marine specimens on the seabed.

### 4. Synthesized Deep-Sea Web Audio API Engine
- **Hull Structural Resonance:** Low-frequency 55 Hz continuous submersible hum.
- **Acoustic Sonar Ping:** 1.85 kHz swept chime with acoustic delay reverberation.
- **Propeller Cavitation Noise:** Dynamic bandpass filtered sawtooth wave responsive to thrust power.
- **Emergency Ballast Jettison:** Acoustic warning klaxon and pressurized nitrogen burst.

---

## 🎮 Pilot Controls & Keybindings

| Key | Control Axis | Subsea Function |
| :---: | :---: | :--- |
| <kbd>W</kbd> / <kbd>S</kbd> | **Surge** | Forward / Reverse Horizontal Propulsion |
| <kbd>A</kbd> / <kbd>D</kbd> | **Sway** | Port / Starboard Lateral Strafe |
| <kbd>R</kbd> / <kbd>F</kbd> | **Heave** | Ascend / Descend Vertical Depth Control |
| <kbd>Q</kbd> / <kbd>E</kbd> | **Yaw** | Turn Heading Left / Right |
| <kbd>C</kbd> | **Camera View** | Cycle Cockpit FPV / External Chase / Oceanographic Map |
| <kbd>L</kbd> | **Lighting** | Toggle High-Lumen Dual LED Spotlights |
| <kbd>Space</kbd> | **Emergency** | Jettison Ballast Weight for Rapid Emergency Ascent |

*Full touch virtual joysticks enabled for iPad, iPhone, and Android touchscreens.*

---

## 🌐 Complete Bilingual Support (العربية / English)
Zero-delay runtime localization toggling all primary telemetry tapes, compass bearings, mission objectives, and acoustic controls between Arabic and English.

---

## 📜 License
MIT License — Open-source educational and research subsea digital twin. Designed and built by **Tareq Aboushi**.
