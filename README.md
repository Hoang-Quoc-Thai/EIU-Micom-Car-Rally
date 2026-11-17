
# 🏎️ EIU Micom Car Rally (MCR) Autonomous Racing Robot

![Language](https://img.shields.io/badge/Language-C%2FC%2B%2B-blue.svg)
![MCU](https://img.shields.io/badge/MCU-ATmega2560-00979D.svg)
![IDE](https://img.shields.io/badge/IDE-Atmel%20Studio-orange.svg)
![Competition](https://img.shields.io/badge/Competition-Micom%20Car%20Rally-orange.svg)

## 📌 Overview
This repository contains the embedded firmware, custom PCB designs, and 3D mechanical CAD files for the **Autonomous Line-Following Racing Robot** developed at **Eastern International University (EIU)** for the **Micom Car Rally (MCR)** competition. 

The robot is engineered to autonomously navigate high-speed tracks featuring sharp corners, right-angle turns, lane changes, and crank obstacles using real-time optical sensor fusion and closed-loop PID control.

---

## ⚙️ Key Features
* **High-Speed Line Tracking:** Multi-channel phototransistor sensor array with dynamic calibration for varying ambient light conditions.
* **Rule-Based & State-Machine Steering:** Discrete steering angle mapping and velocity profiling tailored for straightaways, 90-degree turns, lane-change markers, and crank sections.
* **Custom High-Current Power Stage:** Dedicated self-designed motor driver PCB utilizing **BTS7960** half-bridge ICs to handle high stall currents and rapid acceleration of dual **GA25** DC gear motors.
* **Precision Front-Wheel Steering:** High-torque **MG996R** metal-gear servo actuated via hardware PWM timers for responsive cornering.

---

## 🛠️ System Architecture & Hardware Stack

| Subsystem | Component / Specification |
| :--- | :--- |
| **Microcontroller** | Custom Control Board featuring **ATmega2560** (16 MHz, 8-bit AVR) |
| **Firmware Toolchain** | **Atmel Studio** (Embedded C / AVR-GCC) |
| **Steering Actuator** | **MG996R** High-Torque Metal-Gear Servo |
| **Drive Motors** | Dual **GA25** Brushed DC Gear Motors |
| **Motor Driver** | Custom Power PCB with **BTS7960** High-Current H-Bridge Drivers |
| **Chassis & Mechanical** | Custom 3D-Modeled Chassis & Steering Linkage (**SolidWorks**) |
---

## 📂 Repository Structure
```text
EIU-Micom-Car-Rally/
├── Firmware/               # Embedded C/C++ source code, PID tuning, and state machine
│   ├── Inc/                # Header files (sensor drivers, PID, PWM config)
│   └── Src/                # Main control loop and peripheral ISRs
├── Hardware_PCB/           # Altium / EasyEDA schematics, PCB layouts, and BOM
├── Mechanical_CAD/         # SolidWorks / Fusion 360 assemblies and STL files for 3D printing
└── Docs/                   # Wiring diagrams, track rulebooks, and test logs
```
---

## 🔮 Future Improvements

* Implement closed-loop **PID control** for smoother high-speed steering transitions and differential motor speed regulation using GA25 encoder feedback.
* Add dynamic speed profiling based on upcoming track curvature.

---

## 👨‍💻 Author

**Hoàng Quốc Thái**

*Mechatronics Engineering Student — Eastern International University (EIU)*

* **GitHub:** [@Hoang-Quoc-Thai](https://github.com/Hoang-Quoc-Thai)
* **LinkedIn:** [linkedin.com/in/thaihoangg](https://www.google.com/search?q=https://www.linkedin.com/in/thaihoangg/)
