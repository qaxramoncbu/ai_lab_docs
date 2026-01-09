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


<div align="center">

## 🏢 Laboratory Overview
![Category](https://img.shields.io/badge/Category-Robotics-blue)
![Laboratory](https://img.shields.io/badge/Laboratory-Lab-purple?logo=atom)
![Overview](https://img.shields.io/badge/Overview-Project-blue?logo=abstract)

*The AI & Robotics Laboratory provides cutting-edge research infrastructure for:*

</div>

- **🤖 Robotics & Autonomous Systems** – Motion planning, control, and human-robot interaction
- **👁️ Computer Vision & Perception** – 3D reconstruction, object detection, and depth sensing
- **🧠 Artificial Intelligence & Machine Learning** – Model training, inference, and neural networks
- **🌐 Edge Computing & IoT** – Real-time processing and distributed systems

<div align="center">

## 🖥️ Central AI Server (Infrastructure Overview)

[![Infrastructure](https://img.shields.io/badge/Infrastructure-Central%20AI%20Server-darkblue?logo=serverfault)](https://serverfault.com/)
[![Architecture](https://img.shields.io/badge/System-Architecture-blue?logo=diagramsdotnet)](https://www.drawio.com/)
[![Backend](https://img.shields.io/badge/Backend-Server--Side-gray?logo=linux)](https://www.kernel.org/)

</div>

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


<div align="center">

## 🖥️ Workstations (x10) — ThinkStation P3 Tower Gen 2

[![Workstation](https://img.shields.io/badge/Workstations-ThinkStation%20P3%20Tower%20Gen%202-black?logo=lenovo)](https://www.lenovo.com/us/en/p/workstations/thinkstation-p-series/lenovo-thinkstation-p3-tower-gen-2-intel-workstation/30hs000nus)
[![Specs PDF](https://img.shields.io/badge/Specs-PDF-blue?logo=adobereader)](https://psref.lenovo.com/syspool/Sys/PDF/ThinkStation/ThinkStation_P3_Tower_Gen_2/ThinkStation_P3_Tower_Gen_2_Spec.pdf)
</div>


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

<div align="center">

## 👁️ Stereo Camera — Intel RealSense D455

![Category](https://img.shields.io/badge/Category-Robotics-blue)
[![GitHub](https://img.shields.io/badge/GitHub-IntelRealSense%2Flibrealsense-black?logo=github)](https://github.com/IntelRealSense/librealsense)
[![Docs](https://img.shields.io/badge/Docs-Intel%20RealSense-blue?logo=readthedocs)](https://www.realsenseai.com/products/real-sense-depth-camera-d455f/)

</div>


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

- More information could be found via

</td>
<td width="35%" align="right">
<img src="../images/camera.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>



### Basic code example (RGB stream)

```python
import pyrealsense2 as rs

pipeline = rs.pipeline() # Create a pipeline
pipeline.start() # Start streaming

try:
    while True:
        frames = pipeline.wait_for_frames()
        depth_frame = frames.get_depth_frame()
        if not depth_frame:
            continue

        width, height = depth_frame.get_width(), depth_frame.get_height()
        dist = depth_frame.get_distance(width // 2, height // 2)
        print(f"The camera is facing an object {dist:.3f} meters away", end="\r")

finally:
    pipeline.stop() # Stop streaming
```

---

<div align="center">

## 🤖 Humanoid Robot — Unitree G1

[![Humanoid Robot](https://img.shields.io/badge/Humanoid%20Robot-Unitree%20G1-blue?logo=robotframework)](https://www.unitree.com/g1/)
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics)
[![unitree_sdk2](https://img.shields.io/badge/SDK-unitree_sdk2-blue?logo=github)](https://github.com/unitreerobotics/unitree_sdk2)
[![unitree_ros](https://img.shields.io/badge/ROS-unitree_ros-blue?logo=ros)](https://github.com/unitreerobotics/unitree_ros)
[![unitree_sdk2_python](https://img.shields.io/badge/Python-SDK%20Python-blue?logo=python)](https://github.com/unitreerobotics/unitree_sdk2_python)

</div>

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

### Basic setup example

```python
from setuptools import setup, find_packages

setup(name='unitree_sdk2py',
      version='1.0.1',
      author='UnitreeRobotics',
      author_email='unitree@unitree.com',
      long_description=open('README.md').read(),
      long_description_content_type="text/markdown",
      license="BSD-3-Clause",
      packages=find_packages(include=['unitree_sdk2py','unitree_sdk2py.*']),
      description='Unitree robot sdk version 2 for python',
      project_urls={
            "Source Code": "https://github.com/unitreerobotics/unitree_sdk2_python",
      },
      python_requires='>=3.8',
      install_requires=[
            "cyclonedds==0.10.2",
            "numpy",
            "opencv-python",
      ],
      )
```

---

<div align="center">

## 🐕 Quadruped Robot — Unitree Go2

[![Quadruped Robot](https://img.shields.io/badge/Quadruped%20Robot-Unitree%20Go2-blue?logo=robotframework)](https://www.unitree-robot.com/products/unitree-go2.html) &nbsp;
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics) &nbsp;
[![Go2 ROS 2](https://img.shields.io/badge/ROS2-Go2%20Support-brightgreen?logo=ros)](https://github.com/Unitree-Go2-Robot/go2_robot)

</div>


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


### Basic motor control example

```cpp
uint8[2] head
uint8 level_flag
uint8 frame_reserve
uint32[2] sn
uint32[2] version
uint16 bandwidth
MotorCmd[20] motor_cmd //motor command
BmsCmd bms_cmd
uint8[40] wireless_remote
uint8[12] led
uint8[2] fan
uint8 gpio
uint32 reserve
uint32 crc
```

---

<div align="center">

## 🐕 Quadruped Robot — Unitree Go2

[![Quadruped Robot](https://img.shields.io/badge/Quadruped%20Robot-Unitree%20Go2-blue?logo=robotframework)](https://www.unitree.com/en/go2)
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics)
[![Go2 ROS 2](https://img.shields.io/badge/ROS2-Go2%20Support-brightgreen?logo=ros)](https://github.com/YasiruDEX/unitree-go2-ros2)

</div>


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

### Basic avoiding obstacles example
```python 
import time
import os

from unitree_sdk2py.core.channel import ChannelFactoryInitialize
from unitree_sdk2py.go2.obstacles_avoid.obstacles_avoid_client import ObstaclesAvoidClient

if __name__ == "__main__":
    ChannelFactoryInitialize(0, "enp3s0")

    client = ObstaclesAvoidClient()
    client.SetTimeout(3.0)
    client.Init()

    while True:
        print("##################GetServerApiVersion###################")
        code, serverAPiVersion = client.GetServerApiVersion()
        if code != 0:
            print("get server api error. code:", code)
        else:
            print("get server api version:", serverAPiVersion)

        if serverAPiVersion != client.GetApiVersion():
            print("api version not equal.")

        time.sleep(3)

        print("##################SwitchGet###################")
        code, enable = client.SwitchGet()
        if code != 0:
            print("switch get error. code:", code)
        else:
            print("switch get success. enable:", enable)
            
        time.sleep(3)
        
        print("##################SwitchSet (on)###################")
        code = client.SwitchSet(True)
        if code != 0:
            print("switch set error. code:", code)
        else:
            print("switch set success.")
            
        time.sleep(3)

        print("##################SwitchGet###################")
        code, enable1 = client.SwitchGet()
        if code != 0:
            print("switch get error. code:", code)
        else:
            print("switch get success. enable:", enable1)
            
        time.sleep(3)

        print("##################SwitchSet (off)###################")
        code = client.SwitchSet(False)
        if code != 0:
            print("switch set error. code:", code)
        else:
            print("switch set success.")
            
        time.sleep(3)

        print("##################SwitchGet###################")
        code, enable1 = client.SwitchGet()
        if code != 0:
            print("switch get error. code:", code)
        else:
            print("switch get success. enable:", enable1)
            
        time.sleep(3)


        print("##################SwitchSet (enable)###################")

        code = client.SwitchSet(enable)
        if code != 0:
            print("switch set error. code:", code)
        else:
            print("switch set success. enable:", enable)
            
        time.sleep(3)

        print("##################SwitchGet###################")
        code, enable = client.SwitchGet()
        if code != 0:
            print("switch get error. code:", code)
        else:
            print("switch get success. enable:", enable)
            
        time.sleep(3)
```

---

<div align="center">

## 🤖 Industrial Robot — FANUC LR Mate 200iC/5L (R-30iA Controller)

[![Industrial Robot](https://img.shields.io/badge/Robot-FANUC%20LR%20Mate%20200iC%2F5L-red?logo=fanuc)](https://www.fanucamerica.com/products/robots/series/lr-mate)
[![Official GitHub](https://img.shields.io/badge/GitHub-FANUC%20ROS%202%20Driver-black?logo=github)](https://github.com/FANUC-CORPORATION/fanuc_driver)
[![ROS2 Support](https://img.shields.io/badge/ROS2-FANUC%20ROS2%20Docs-brightgreen?logo=ros)](https://fanuc-corporation.github.io/fanuc_driver_doc/main/)

</div>


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
```python
#!/usr/bin/env python3

# Copyright 2025 FANUC CORPORATION
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

import rclpy
from rclpy.node import Node
from std_msgs.msg import Float64MultiArray
import math
import time


class SineWavePublisher(Node):
    """
    A ROS2 node that publishes sine wave commands to the forward_command_controller.

    This node generates sine wave trajectories for a single joint at a time and publishes
    them to the forward_position_controller's commands topic.
    """

    def __init__(self):
        super().__init__("sine_wave_publisher")

        # Hardcoded parameters
        self.amplitude = math.radians(10)  # 10 degrees in radians
        self.frequency = 0.1  # Hz
        self.publish_rate = 500.0  # Hz (matches controller manager update rate)

        # Create publisher with larger queue size
        self.publisher = self.create_publisher(
            Float64MultiArray, "/forward_position_controller/commands", 100
        )

        # Create timer for publishing
        timer_period = 1.0 / self.publish_rate
        self.timer = self.create_timer(timer_period, self.publish_command)

        # Initialize time
        self.start_time = time.time()

        self.get_logger().info("Sine wave publisher started:")
        self.get_logger().info("  Joints: All 6 joints (J1-J6)")
        self.get_logger().info(f"  Amplitude: {self.amplitude} radians")
        self.get_logger().info(f"  Frequency: {self.frequency} Hz")
        self.get_logger().info(f"  Publish rate: {self.publish_rate} Hz")
        self.get_logger().info("  Publishing to: /forward_position_controller/commands")

    def publish_command(self):
        """Publish trajectory-style sine wave command for all joints."""
        # Calculate current time
        current_time = time.time() - self.start_time

        # Calculate phase (similar to send_trajectory.py)
        period = 1.0 / self.frequency  # Convert frequency to period
        phase = (2.0 * math.pi / period) * current_time

        # Calculate trajectory-style sine wave: amplitude * (1.0 - cos(phase))
        # This creates a smooth rise from 0 to 2*amplitude and back to 0
        trajectory_value = self.amplitude * (1.0 - math.cos(phase))

        # Create message with 6 joint positions (all joints get the same trajectory value)
        msg = Float64MultiArray()
        msg.data = [trajectory_value] * 6  # Apply trajectory wave to all joints

        # Publish message
        self.publisher.publish(msg)

        # Log current value (only every 50th message to avoid spam)
        if int(current_time * self.publish_rate) % 50 == 0:
            self.get_logger().info(f"All joints: {trajectory_value:.3f} rad")


def main(args=None):
    rclpy.init(args=args)

    try:
        node = SineWavePublisher()
        rclpy.spin(node)
    except KeyboardInterrupt:
        pass
    except Exception as e:
        print(f"Error: {e}")
    finally:
        rclpy.shutdown()


if __name__ == "__main__":
    main()
```

---

<div align="center">

## 🦾 Robotic Manipulator Kit (Controller‑Based Mechanical Arm)
[![Official GitHub](https://img.shields.io/badge/GitHub‑open_manipulator-black?logo=github)](https://github.com/ROBOTIS-GIT/open_manipulator)  

</div>


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
