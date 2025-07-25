# 🤖 YuMi Pick and Place – RobotStudio Project

## 📌 Project Description

This project focuses on simulating a **two-arm ABB YuMi robot** performing a pick and place operation with quality control. The station workflow is based on the following sequence:

1. **First phase:** The robot picks up a product with one arm.<img width="1288" height="720" alt="Screenshot 2025-07-25 133326" src="https://github.com/user-attachments/assets/435d53e3-ac3a-40f4-bce9-50d70296049e" />

2. **Second phase:** The product is positioned for quality inspection, where the robot takes a photo using its second arm.
3. **Third phase:** The second arm picks up the product after inspection.
4. **Fourth phase:** The product is placed in the designated location.
5. **Fifth phase:** The robot picks up the next product and repeats the sequence.

The project was implemented in **ABB RobotStudio**, providing a fully simulated environment for programming and testing the YuMi robot’s dual-arm coordination and quality control process.

## ⚙️ Technologies and Tools

- **ABB RobotStudio** – main simulation and programming environment
- **Smart Components** – for modeling robot and peripheral devices
- **RAPID** – ABB’s robot programming language controlling the sequence
- **I/O Signals** – to manage communication between robot arms and peripherals

## 🧩 Features

- Dual-arm coordination and handover of products between arms
- Integrated quality control phase using the second arm for product inspection
- Automated pick, inspect, place cycle with repeatable sequences
- Modular project structure for easy updates and scalability
- Realistic simulation environment enabling thorough testing of complex robot tasks
