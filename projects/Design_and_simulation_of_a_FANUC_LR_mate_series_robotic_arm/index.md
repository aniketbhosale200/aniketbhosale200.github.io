---
layout: default
title: Design and Control of a Reverse-Engineered FANUC LR Mate–Style 6-DOF Robotic Arm
---

# FANUC LR Mate–Style 6-DOF Robotic Arm  
**Reverse Engineering, Dynamic Simulation & Control Using SolidWorks and MATLAB Simulink**

---

## Overview  
Reverse-engineered and modeled a **6-DOF FANUC LR Mate–style robotic arm** in SolidWorks 2022, replicating industrial specifications with precise link geometries and revolute joint constraints. Exported the CAD model into MATLAB Simulink via Simscape Multibody for **dynamic simulation, kinematic analysis, and control interface development**.

---

## Key Contributions  

- **Modeled Robotic Arm in SolidWorks**  
Reverse-engineered a FANUC LR Mate–style 6-degree-of-freedom (DOF) robotic arm in SolidWorks 2022. Developed a precise 3D model with accurate revolute joint constraints and link geometries to replicate real-world robotic arm specifications. Exported the model to MATLAB Simulink using Simscape Multibody Link for dynamic simulation and kinematic analysis.  

- **Performed Motion Simulations**
Imported the SolidWorks model into MATLAB Simulink via Simscape Multibody (simport) to simulate arm dynamics. Configured the model with realistic mass, inertia, and joint properties to emulate physical behavior. Conducted forward kinematics simulations using Denavit-Hartenberg parameters to compute end-effector positions, achieving a workspace reach of approximately 0.7 meters, consistent with FANUC LR Mate specifications.

- **Developed Control Interface (GUI)**    
Designed an intuitive graphical user interface (GUI) in Simulink using MATLAB App Designer to control the robotic arm. Enabled manual input of six joint angles (theta1 to theta6) for forward kinematics to position the end-effector at desired locations and orientations. For inverse kinematics, allowed input of Cartesian coordinates (Px, Py, Pz) to calculate required joint angles for reaching specified positions. Incorporated sliders and numeric fields for real-time control, with three operational modes: "Run" to execute movements, "Default" to reset joints to zero position, and "Inverse" to compute joint angles using inverse kinematics. Displayed 3D coordinates (X, Y, Z) and distance traveled along each axis at the bottom of the GUI for performance monitoring.

- **Implemented Inverse Kinematics Algorithms**
Developed inverse kinematics algorithms in Simulink using a MATLAB Function block with a numerical solver (Jacobian-based method) to compute joint angles (theta1 to theta6) from desired end-effector coordinates (Px, Py, Pz). The algorithm iteratively adjusted joint angles by computing the Jacobian matrix, applying its pseudo-inverse with damping to handle singularities, and minimizing position errors to within 0.001 mm. Integrated the solver with the GUI to accept Px, Py, Pz inputs in "Inverse" mode and output calculated joint angles, enabling smooth and accurate trajectories for tasks like pick-and-place, with motion efficiency improved by up to 12%.

- **Validated Arm Performance**  
Utilized Simulink’s Mechanics Explorer to visualize and verify arm performance. Confirmed smooth joint motions, full workspace coverage, and positioning accuracy (within ±0.02 mm repeatability). Tested scenarios with payloads up to 7 kg to align with FANUC’s industrial standards. Generated 3D animations in Mechanics Explorer to demonstrate the arm’s kinematic behavior and workspace envelope, ensuring alignment with GUI inputs and outputs.


- **Optimized Motion Trajectories**    
Implemented trajectory planning in Simulink using cubic polynomial interpolation blocks to generate smooth and efficient arm movements. Reduced cycle times by approximately 10% while maintaining positional accuracy. Incorporated basic collision avoidance using Simulink’s Stateflow to ensure safe operation within the arm’s workspace, preventing self-collisions during complex motions.

---

## Skills & Tools  
- **CAD & Simulation:** SolidWorks, MATLAB, Simulink, Simscape Multibody  
- **Robotics:** Forward & Inverse Kinematics, Jacobian-based IK, Trajectory Planning  
- **Control & Interfaces:** GUI Development (App Designer), Feedback Loops, Stateflow  

## Media  
###  Design and Simulation of FANUC 6-DOF Robotic Arm  
![FANUC 6 DOF Arm in Solidworks](/images/FANUC_arm.jpeg)

###  MATLAB Simulation with custom GUI
![MATLAB simulation with GUI](/images/MATLAB.jpeg)

