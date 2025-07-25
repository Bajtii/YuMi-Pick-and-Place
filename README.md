# 🤖 YuMi Pick and Place – RobotStudio Project

## 📌 Project Description

This project focuses on simulating a **two-arm ABB YuMi robot** performing a pick and place operation with quality control. The station workflow is based on the following sequence:

1. **First phase:** The robot picks up a product with one arm.<img width="1288" height="720" alt="Screenshot 2025-07-25 133326" src="https://github.com/user-attachments/assets/435d53e3-ac3a-40f4-bce9-50d70296049e" />

2. **Second phase:** The product is positioned for quality inspection, where the robot takes a photo using its second arm.<img width="1332" height="705" alt="Screenshot 2025-07-25 133931" src="https://github.com/user-attachments/assets/fc045065-e4d0-4c5f-a4e9-3f9fd588030e" />

3. **Third phase:** The second arm picks up the product after inspection.<img width="1335" height="722" alt="Screenshot 2025-07-25 133412 (1)" src="https://github.com/user-attachments/assets/7637e738-1524-4b57-9174-2156b706bee3" /><img width="1331" height="731" alt="Screenshot 2025-07-25 133612 (1)" src="https://github.com/user-attachments/assets/f19a944c-2a7c-43b0-864b-62052d7e56cd" />


4. **Fourth phase:** The product is placed in the designated location.
5. **Fifth phase:** The robot picks up the next product and repeats the sequence.<img width="1332" height="705" alt="Screenshot 2025-07-25 133931 (1)" src="https://github.com/user-attachments/assets/ad02e3f9-af27-4ae7-90db-e9a11dd871cf" />



The project was implemented in **ABB RobotStudio**, providing a fully simulated environment for programming and testing the YuMi robot’s dual-arm coordination and quality control process.

An important part of the implementation is the **gripper control logic** — the opening and closing (release and grasp) of the robot's grippers is precisely controlled. This logic uses **persistent boolean variables (PERS BOOL)** to wait for the completion of specific gripper signals on each arm, ensuring proper synchronization before transitioning to the next step in the sequence.

## ⚙️ Technologies and Tools

- **ABB RobotStudio** – main simulation and programming environment
- **Smart Components** – for modeling robot and peripheral devices
- **RAPID** – ABB’s robot programming language controlling the sequence
- **I/O Signals** – to manage communication between robot arms and peripherals
- **PERS BOOL variables** – used for robust synchronization of gripper actions and signal completion

## 🧩 Features

- Dual-arm coordination and handover of products between arms
- Integrated quality control phase using the second arm for product inspection
- Automated pick, inspect, place cycle with repeatable sequences
- Gripper open/close (release/grasp) logic implemented with PERS BOOL synchronization
- Modular project structure for easy updates and scalability
- Realistic simulation environment enabling thorough testing of complex robot tasks
