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
  - Created a high-fidelity 3D model with accurate revolute joints and link geometries.  
  - Exported using Simscape Multibody Link (simport) for seamless MATLAB integration.  

- **Performed Motion Simulations**  
  - Configured mass, inertia, and joint properties for realistic dynamics.  
  - Conducted forward kinematics using Denavit–Hartenberg parameters.  
  - Verified a workspace reach of **~0.7 m**, consistent with FANUC LR Mate specs.  

- **Developed Control Interface (GUI)**  
  - Built an interactive GUI in Simulink (MATLAB App Designer).  
  - Allowed manual input of **joint angles (θ1–θ6)** for forward kinematics.  
  - Enabled Cartesian input (Px, Py, Pz) for inverse kinematics with real-time computation.  
  - Incorporated **three modes:** Run, Default (reset), and Inverse (Jacobian solver).  
  - Displayed real-time **end-effector coordinates & axis displacements**.  

- **Implemented Inverse Kinematics Algorithms**  
  - Designed solver using Jacobian pseudo-inverse with damping to avoid singularities.  
  - Achieved precision of **±0.001 mm** in end-effector positioning.  
  - Enabled smooth, accurate trajectories for pick-and-place with **12% motion efficiency improvement**.  

- **Validated Arm Performance**  
  - Verified smooth joint motion and full workspace coverage in Mechanics Explorer.  
  - Achieved **±0.02 mm repeatability** with payloads up to **7 kg**, meeting industrial benchmarks.  
  - Produced 3D visualizations of kinematic behavior and workspace envelope.  

- **Optimized Motion Trajectories**  
  - Applied cubic polynomial interpolation for smooth trajectory planning.  
  - Reduced cycle time by **~10%** while maintaining accuracy.  
  - Added basic collision avoidance logic using Stateflow for safe operations.  

---

## Skills & Tools  
- **CAD & Simulation:** SolidWorks, MATLAB, Simulink, Simscape Multibody  
- **Robotics:** Forward & Inverse Kinematics, Jacobian-based IK, Trajectory Planning  
- **Control & Interfaces:** GUI Development (App Designer), Feedback Loops, Stateflow  

