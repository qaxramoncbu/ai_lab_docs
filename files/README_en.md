<div align="center">

# 🤖 AI & Robotics Laboratory
## Equipment Inventory & Usage Guide

![Category](https://img.shields.io/badge/Category-Robotics-blue)
![Category](https://img.shields.io/badge/Category-Computer%20Vision-purple)
![Category](https://img.shields.io/badge/Category-AI-green)
![Access](https://img.shields.io/badge/Access-Restricted-red)
![Usage](https://img.shields.io/badge/Usage-Programming%20Required-orange)
![OS](https://img.shields.io/badge/OS-Linux%20%7C%20Windows-blue)
![Code](https://img.shields.io/badge/Code-Python-yellow)
![Framework](https://img.shields.io/badge/Framework-ROS-green)
![Status](https://img.shields.io/badge/Status-Operational-brightgreen)
![Version](https://img.shields.io/badge/Version-1.0-lightgrey)

*Comprehensive documentation for laboratory equipment and operational procedures*

</div>

---



## 🏢 Laboratory Overview

The AI & Robotics Laboratory provides cutting-edge research infrastructure for:

- **🤖 Robotics & Autonomous Systems** – Motion planning, control, and human-robot interaction
- **👁️ Computer Vision & Perception** – 3D reconstruction, object detection, and depth sensing
- **🧠 Artificial Intelligence & Machine Learning** – Model training, inference, and neural networks
- **🌐 Edge Computing & IoT** – Real-time processing and distributed systems


## 🖥️ Central AI Server (Infrastructure Overview)

<table>
<tr>
<td width="65%" valign="top">

> ⚠️ **Infrastructure notice**  
> Direct interaction with server hardware is restricted to system administrators.

### Purpose
The AI Server is a **centralized compute platform** used for:
- AI model training
- Large-scale inference
- Data processing
- Backend services for robotics and vision systems

### User Interaction
Users interact with the server **remotely only**:
- SSH access
- Remote desktop or web interfaces
- Job execution and workload submission

### Managed Components
The following components are **administrator-managed** and require **no user action**:
- Server chassis and rack
- CPUs and GPUs
- RAM and storage
- Power (PDU) and cooling systems

📌 For access requests or issues, contact the lab administrator.

</td>
<td width="35%" align="right">

<img src="../images/ai_server.png" alt="AI Server Installed in Rack" width="100%"/>

</td>
</tr>
</table>

## 🖥️ Workstations (x10) — ThinkStation P3 Tower Gen 2


<table>
<tr>
<td width="65%" valign="top">

### Purpose
These workstations are **user-facing development machines** intended for:
- Software development  
- AI and machine learning experiments  
- Data processing and visualization  
- Connecting to the central AI server  

Each workstation is an independent system equipped with a dedicated GPU.

---

### Who can use them
- Students  
- Researchers  
- Developers  
- Lab staff working on approved projects  

</td> 
<td width="35%" align="right">
<img src="../images/power_station.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>

<table>
<tr>
<td width="65%" valign="top">

### How to start using a workstation
1. Power on the workstation  
2. Log in to **Windows 11 Pro**  
3. Open required development tools (VS Code, Python, Docker, etc.)  
4. Run local workloads or connect to shared compute resources  

---

### What users can do
- Write, run, and debug code  
- Run GPU-accelerated applications  
- Train and test small-to-medium AI models  
- Visualize datasets and results  
- Access network and server resources  

</td> 
<td width="35%" align="right">
<img src="../images/power.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>



<table>
<tr>
<td width="65%" valign="top">

### Check GPU availability
```powershell
nvidia-smi

import torch
print(torch.cuda.is_available())
```

### Notes
- Report any hardware or software issues immediately
- Follow lab usage and safety rules at all times

</td> 
<td width="35%" align="right">
<img src="../images/gpu_check.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>

## 👁️ Stereo Camera — Intel RealSense D455

<table>
<tr>
<td width="65%" valign="top">

### Purpose
The Intel RealSense D455 is a **depth-sensing stereo camera** used for:
- Obstacle avoidance
- 3D scanning and reconstruction
- Depth-aware computer vision
- Robotics perception systems

</td> 
<td width="35%" align="right">
<img src="../images/stereo_camera.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>
    

<table>
<tr>
<td width="65%" valign="top">

### How to use
1. Connect the camera via USB
2. Install Intel RealSense SDK
3. Launch your application or script
4. Access RGB and depth streams via API

</td>
<td width="35%" align="right">
<img src="../images/camera.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>


### Basic code example (RGB stream)

```python
import pyrealsense2 as rs
import numpy as np
import cv2

pipeline = rs.pipeline()
pipeline.start()

while True:
    frames = pipeline.wait_for_frames()
    color_frame = frames.get_color_frame()
    if not color_frame:
        continue

    image = np.asanyarray(color_frame.get_data())
    cv2.imshow("RealSense RGB", image)

    if cv2.waitKey(1) == 27:
        break

pipeline.stop()
cv2.destroyAllWindows()
```

---

## 🤖 Humanoid Robot — Unitree G1

<table>
<tr>
<td width="65%" valign="top">

### Purpose
The **Unitree G1** is a **humanoid research robot** used for:
- Mobility and locomotion research
- Balance and motion control
- Human–robot interaction
- Advanced robotics experiments

---

### Safety notice ⚠️
- Operate only in designated areas
- Keep a safe distance during motion
- Never obstruct joints or actuators
- Emergency stop must be accessible at all times

---

### How users interact with the robot
Users control the robot through:
- Official control software
- SDK and APIs
- Predefined motion scripts

---

### How to start using the robot
1. Place the robot on a stable surface
2. Power on the robot
3. Connect to the control network
4. Launch control software or SDK
5. Perform system checks before motion

</td>
<td width="35%" align="right">
<img src="../images/robot.png" alt="Unitree G1 Humanoid Robot" width="100%"/>
</td> </tr> </table>

### Basic control example

```python
robot.stand()
robot.walk_forward(steps=3)
robot.turn(angle=30)
```

---

## 🐕 Quadruped Robot — Unitree Go2

<table>
<tr>
<td width="65%" valign="top">

### Purpose
The **Unitree Go2** is a **quadruped robotic platform** designed for:
- Robotics research and education
- Autonomous navigation experiments
- AI perception and locomotion testing
- Human–robot interaction

---

### Safety notice ⚠️
- Operate on flat, obstacle-free surfaces
- Keep hands clear of moving legs
- Use emergency stop when required
- Do not operate near stairs or edges

---

### How users interact with the robot
Users control the robot via:
- Official control application
- SDK / API interface
- Predefined motion modes

---

### How to start using the robot
1. Place the robot on a stable surface
2. Power on the robot
3. Connect via control software
4. Perform calibration if required
5. Select motion or autonomous mode

</td>
<td width="35%" align="right">
<img src="../images/dog.png" alt="Unitree Go2 Quadruped Robot" width="100%"/> 
</td> </tr> </table> 


### Basic motion example

```python
robot.stand()
robot.walk_forward(distance=2.0)
robot.turn(angle=45)
robot.stop()
```

---

## 🦾 Robotic Manipulator

<table>
<tr>
<td width="65%" valign="top">

### Purpose
The **robotic manipulator** is intended for:
- Research and development
- Motion control algorithm testing
- Object manipulation tasks
- Integration with computer vision and AI systems
- Automation of repetitive operations

---

### Key Functions
- Precise spatial positioning
- Grasping, moving, and placing objects
- Programmable motion trajectories
- Manual and automatic operation modes

---

### Safety Precautions ⚠️
- Do not place hands inside the working area during operation
- Use the emergency stop when required
- Securely mount the manipulator to the work surface
- Verify payload limits before operation

---

### User Interaction
The manipulator can be controlled via:
- Software interface (SDK / API)
- Manual control (teach / jog mode)
- Predefined motion scripts

---

### Getting Started
1. Secure the manipulator on a stable surface
2. Connect power and control interfaces
3. Launch the control software
4. Perform axis calibration
5. Select the operation mode (manual or automatic)

</td>
<td width="35%" align="right">
<img src="../images/robotic_manipulator.png" alt="Unitree Go2 Quadruped Robot" width="100%"/> 
</td> </tr> </table> 

### Basic Control Example
```python
arm.move_to(x=0.3, y=0.2, z=0.15)
arm.open_gripper()
arm.move_to(x=0.3, y=0.2, z=0.05)
arm.close_gripper()
arm.move_to_home()
```

---

## 🤖 Industrial Robot — FANUC LR Mate 200iC/5L (R-30iA Controller)

<table>
<tr>
<td width="65%" valign="top">

### Model
- **Robot:** FANUC LR Mate 200iC/5L  
- **Controller:** FANUC R-30iA

---

### Purpose
The **FANUC LR Mate 200iC/5L** is a compact industrial robot designed for:
- Automation research
- Industrial training and education
- Pick-and-place operations
- Assembly and material handling
- Vision-guided robotic tasks

---

### Key Capabilities
- 6-axis articulated robot arm
- High precision and repeatability
- Long reach version (5L)
- Compatible with vision systems and external sensors
- Supports offline and online programming

---

### User Interaction
The robot is operated using:
- FANUC Teach Pendant
- FANUC R-30iA controller
- Robot programs written in **TP** or **KAREL**
- Optional integration with PLCs and vision systems

---

### Basic Usage Workflow
1. Power on the R-30iA controller
2. Release emergency stop
3. Select operation mode (Teach / Auto)
4. Jog robot to desired positions
5. Record points using the Teach Pendant
6. Run or test the robot program

</td>
<td width="35%" align="right">
<img src="../images/fanuc_img.png" alt="Unitree Go2 Quadruped Robot" width="100%"/> 
</td> </tr> </table> 

### Example — Simple Pick & Place Logic (Conceptual)
```text
MOVE TO HOME
MOVE TO PICK POSITION
CLOSE GRIPPER
MOVE TO PLACE POSITION
OPEN GRIPPER
RETURN TO HOME
```

---

## 🦾 Robotic Manipulator Kit (Controller-Based Mechanical Arm)

<table>
<tr>
<td width="65%" valign="top">

### Type
- **Category:** Educational / Research Robotic Manipulator
- **Configuration:** Modular mechanical arm with controller

---

### Purpose
This **robotic manipulator kit** is designed for:
- Robotics education and training
- Learning motion control and kinematics
- Prototyping automation solutions
- Testing grasping and manipulation algorithms

---

### Key Capabilities
- Multi-joint articulated mechanical arm
- Controller-based operation
- Supports servo or stepper motors
- End-effector support (gripper, suction cup, tools)
- Expandable with sensors (limit switches, cameras, force sensors)

---

### User Interaction
Users interact with the manipulator via:
- Dedicated controller board
- PC connection (USB / Serial)
- Programming using Python, C/C++, or Arduino-style code
- Manual and programmatic joint control

---

### Basic Usage Workflow
1. Connect the manipulator to the controller
2. Power on the system
3. Initialize joint positions
4. Control joints manually or via software
5. Attach and configure end-effector
6. Execute motion sequences

</td>
<td width="35%" align="right">
<img src="../images/img_1.png" alt="Unitree Go2 Quadruped Robot" width="100%"/> 
</td> </tr> </table> 

### Example — Basic Joint Control (Conceptual)

```text
SET joint1 = 45°
SET joint2 = 30°
SET joint3 = 15°
OPEN gripper
MOVE to target position
CLOSE gripper
```

---

<div align="center">

## 🏁 End of Documentation

![Status](https://img.shields.io/badge/Status-Operational-brightgreen)
![Access](https://img.shields.io/badge/Access-Restricted-red)
![Safety](https://img.shields.io/badge/Safety-Training%20Required-orange)
![Docs](https://img.shields.io/badge/Documentation-Complete-blue)
![Maintained](https://img.shields.io/badge/Maintained-Yes-green)
![End](https://img.shields.io/badge/README-End%20of%20File-black)
![Version](https://img.shields.io/badge/Version-1.0-lightgrey)
![Updated](https://img.shields.io/badge/Last%20Updated-2026-blue)

---

</div>
