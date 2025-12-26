# Logic Gates Based Line Following Robot (LFR)

## 📌 Project Overview
This project presents the **design and implementation of an autonomous Line Following Robot (LFR)** developed **entirely using fundamental digital logic gates** without employing any microcontroller. The robot detects and follows a predefined path using a **five-sensor Infrared (IR) array**, while all decision-making and motor control operations are performed through **pure combinational logic** constructed from **AND, OR, and NOT gates**.

The project demonstrates the **practical application of Boolean algebra, Karnaugh map (K-map) minimization, and digital logic design** in real-world robotic systems. It was completed as part of the **Digital Electronics Laboratory (EEE-314)** course at **Bangladesh Army International University of Science and Technology (BAIUST)**.

---

## 🎯 Objectives
- Design a line following robot using **only fundamental logic gates**
- Eliminate the use of **microcontrollers and software-based control**
- Apply **Boolean algebra and Karnaugh map techniques** for logic minimization
- Understand the **hardware-level implementation** of robotic control systems
- Demonstrate the educational value of **pure digital electronics in robotics**

---

## 🧠 Working Principle
The robot uses **five IR sensors** arranged horizontally to detect the position of the line. Each sensor outputs a digital signal (HIGH or LOW) depending on whether it detects the line.

### Sensor Inputs
- **L1** – Leftmost sensor  
- **L0** – Left sensor  
- **C0** – Center sensor  
- **R0** – Right sensor  
- **R1** – Rightmost sensor  

### Motor Control Outputs
- **ML0, ML1** → Left motor control  
- **MR0, MR1** → Right motor control  

Each motor is controlled using a **2-bit control scheme** that determines forward, reverse, or stop operations.

---

## 🔁 Control Strategy
- **Move Straight:** Both motors ON  
- **Turn Left:** Right motor ON, Left motor OFF  
- **Turn Right:** Left motor ON, Right motor OFF  
- **Stop:** Both motors OFF  

The logic outputs are derived from a **truth table**, optimized using **Karnaugh maps**, and implemented using standard TTL logic ICs.

---

## ⚙️ Hardware Components
- Infrared (IR) Sensors (5×)
- Logic Gate ICs: 7408 (AND), 7404 (NOT), 7432 (OR)
- L293D Motor Driver IC
- DC Geared Motors (2×)
- Buck Converter Module
- 7.4V Battery
- Chassis, Wheels, Breadboard, Jumper Wires

---

## 🧮 Digital Logic Design
- Truth table created using five sensor inputs and four motor outputs
- Karnaugh map (K-map) minimization applied
- Implemented using:
  - 14 AND gates
  - 6 OR gates
  - 4 NOT gates
- Built entirely with TTL logic ICs

---

## 🧪 Implementation
- Components mounted on a foamboard chassis
- Two-layer design:
  - Lower layer: Battery, buck converter, IR sensors
  - Upper layer: Logic circuit on breadboard
- Optimized for a line width of **4.5–5 cm**

---

## 📊 Results and Observations
- Handles straight paths, curves, zigzags, and intersections
- Successfully manages 90°, 45°, and 130° turns
- Reliable under controlled lighting conditions

**Limitations:**
- Line width below 4.5 cm is unreliable
- Sensitive to sensor alignment and noise

---
## 🖼️ Robot Images

### Top View of the Robot
![Top View](Images/Top View.png)

### Final Assembled Robot
![Final Robot](Images/Final_Robot.jpg)

---

## ✅ Advantages
- No microcontroller required
- Transparent and deterministic logic
- Educational and cost-effective

---

## ❌ Limitations
- Higher hardware complexity
- Limited flexibility compared to programmable systems

---

## 🚀 Applications
- Digital electronics laboratories
- Educational robotics demonstrations
- Hardware-based autonomous navigation

---

## 💰 Cost Analysis
**Total estimated cost:** **1280 BDT**  
(Additional cost incurred for track construction)

---

## 🎓 Academic Information
- **Course:** Digital Electronics Laboratory (EEE-314)
- **Department:** Electrical and Electronic Engineering
- **University:** Bangladesh Army International University of Science and Technology (BAIUST)
- **Submission Date:** December 21, 2025

---

## 👨‍🏫 Supervisor
**Md. Ashraful Islam**  
Assistant Professor, Department of EEE, BAIUST

---

## 👥 Project Team
- Jawad Nahin (ID: 1218017)
- Arzuman Ara (ID: 1218020)
- Khandker Mahazabin (ID: 1218028)
- Adnan Hossain Bhuiyan (ID: 1218031)
- M. Monsur Ahmed Evan (ID: 131014)

---

## 📚 References
- M. Morris Mano, *Digital Design*
- L293D Motor Driver Datasheet
- https://github.com/Batushn/Logic-Gates-Line-Follower

---

## 📌 License
This project is licensed under the **MIT License**.
