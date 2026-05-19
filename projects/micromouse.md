# Micromouse Maze-Solving Robot

An autonomous, high-speed Micromouse robot engineered to navigate and solve complex mazes. This project integrates precise hardware design with robust control loops to achieve stable, high-performance maze exploration and speed runs.

## 🚀 Key Features
* **PID Feedback Control:** Utilizes a tuned Proportional-Integral-Derivative (PID) controller for precise straight-line tracking, smooth cornering, and dynamic direction decisions.
* **IR Sensor Array:** Multi-channel Infrared (IR) sensor integration for real-time distance estimation, obstacle detection, and wall-following capabilities.
* **Optimized Mechatronics:** High-efficiency DC motors driven by specialized motor drivers, balanced carefully for fast acceleration and sharp turning accuracy.

---

## 📸 System Overview

<table align="center">
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/d0765e36-d077-4e66-ad58-854c64b2ccf2" alt="Micromouse Top View" style="width:100%; border-radius:8px;"/>
      <br />
      <b>Isometric Profile</b>
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/8fd8e731-626e-41d6-a4a4-14b999517240" alt="Micromouse Sensor Alignment" style="width:100%; border-radius:8px;"/>
      <br />
      <b>Sensor Integration</b>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/b10732b8-10f3-4ae9-911d-5967bd08576b" alt="Micromouse Hardware Detail" style="width:100%; border-radius:8px;"/>
      <br />
      <b>Chassis and Motor Assembly</b>
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/d75aa6e2-b375-4dcd-abc4-96b50cbbfea4" alt="Micromouse Bench Testing" style="width:100%; border-radius:8px;"/>
      <br />
      <b>Hardware Configuration</b>
    </td>
  </tr>
</table>

---

## 🛠️ Tech Stack & Components

* **Control Theory:** PID / PI Loop tuning for dynamic steering error correction.
* **Perception:** Analog/Digital IR Transceivers for non-contact distance sensing.
* **Firmware/Software:** Written in C++/Python for hardware control, simulation calibration, and path planning.
* **Debugging & Validation:** Bench tested using hardware tools (Oscilloscopes, Analog Discovery 2) to eliminate signal noise and sensor latency.

## 💡 How It Works
1. **Sensing:** The IR sensors continuously poll distances from left, right, and front walls.
2. **Error Calculation:** The control system computes the delta between the left and right sensor values to detect alignment drift.
3. **PID Correction:** The PID controller processes the error value instantly, modifying the left and right motor PWM signals to center the mouse in the cell.
4. **Navigation:** Maze-solving algorithms handle turn decisions at intersections while the low-level mechatronics maintain physical stability.
