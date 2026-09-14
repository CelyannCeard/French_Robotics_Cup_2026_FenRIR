<h1 align="center">🐺 FenRIR - French Robotics Cup 2026</h1>

<p align="center">
  <i>Autonomous robot built for the "Winter is Coming" theme, designed to gather hazelnuts alongside our "Ratatosk" PAMIs.🐿️</i>
</p>

## 🎯 Overview
FenRIR is the primary autonomous robot of our clan, designed to navigate the game table, collect hazelnut crates (giant Jenga blocks), and deposit them in the pantry and nests. Operating alongside 4 smaller "Ratatosk" PAMIs (including one Ninja PAMI), FenRIR relies on an ESP32 microcontroller, a 12V Parkside battery power system, and LiDAR for obstacle detection. 

<p align="center">
<img width="376" height="531" alt="image" src="https://github.com/user-attachments/assets/eb1d1699-436f-4fce-b600-164deeedb502" />
</p>
<p align="center">
[Poster_FenRIR.pdf](https://github.com/user-attachments/files/32194994/Poster_FenRIR.pdf)
</p>

## 🛠️ My Contributions
While the software logic was handled by my teammates, I led the mechanical design, hardware integration, and overall project management for our 8-member team:
*   **System Architecture & Component Selection:** Acted as the primary technical decision-maker, defining the mechanical solutions and selecting the core hardware for the robot's mechanisms (linear guides, NEMA stepper motors, high-torque servos, vacuum pumps, solenoid valves, and suction cups).
*   **CAD & Mechanics:** Designed and 3D-printed custom parts in PLA, ABS, and TPU. The flexible TPU mounts were specifically engineered to dampen the vibrations of the two 12V vacuum pumps. 
*   **Aesthetics & Assembly:** Managed the physical DIY assembly, painting, and overall visual design of the robot.
*   **Electronics Integration:** Wired the limit switches for the Z-axis, custom connectors, RGB LED strips (powering the glowing eyes that indicate the selected team color), and a mini DFPlayer module connected to a speaker for thematic wolf sound effects.
*   **Team Leadership & Logistics:** As Association President, I coordinated tasks, set strict milestones to keep the development of both the main robot and the PAMIs on track, and handled all competition logistics (registration, van rental, and accommodation).

## ⚙️ Technical Architecture
*   **Locomotion:** Driven by NEMA 23 stepper motors and industrial drivers. Navigation is achieved point-to-point via precise open-loop odometry, utilizing exact wheel dimensions, track width, and known starting coordinates.
*   **Z-Axis Elevator:** A NEMA 17 stepper motor paired with a lead screw and linear guide rails lifts the entire gripping assembly.
*   **Smart Grippers:** Four distinct prehensors mounted on the elevator. Each features a 15kg servo motor, a suction cup powered by the vacuum pumps and solenoid valves, and a dedicated color sensor to identify and flip the crates to match our team's color.
*   **Auxiliary Mechanisms:** Side claws actuated by small servos deployed to manipulate the game table's temperature slider.

---
*Project managed and built by the Polytech Lyon RIR (Robotique des Ingénieurs de Roanne) Association.*
