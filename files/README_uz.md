<div align="center">

# 🤖 Sun’iy Intellekt va Robototexnika Laboratoriyasi
## Uskunalar ro‘yxati va foydalanish qo‘llanmasi

![Category](https://img.shields.io/badge/Category-Robototexnika-blue)
![Category](https://img.shields.io/badge/Category-Kompyuter%20Ko‘rishi-purple)
![Category](https://img.shields.io/badge/Category-AI-green)
![Access](https://img.shields.io/badge/Access-Cheklangan-red)
![Usage](https://img.shields.io/badge/Usage-Dasturlash%20Talab%20Qilinadi-orange)
![OS](https://img.shields.io/badge/OS-Linux%20%7C%20Windows-blue)
![Code](https://img.shields.io/badge/Code-Python-yellow)
![Framework](https://img.shields.io/badge/Framework-ROS-green)
![Status](https://img.shields.io/badge/Status-Faol-brightgreen)
![Version](https://img.shields.io/badge/Version-1.0-lightgrey)

*Laboratoriya uskunalari va ulardan foydalanish bo‘yicha to‘liq hujjat*

</div>

---

<div align="center">

## 🏢 Laboratoriya haqida
![Category](https://img.shields.io/badge/Category-Robotics-blue)
![Laboratory](https://img.shields.io/badge/Laboratory-Lab-purple?logo=atom)
![Overview](https://img.shields.io/badge/Overview-Project-blue?logo=abstract)

*Sun’iy intellekt va robototexnika laboratoriyasi quyidagi yo‘nalishlarda
tadqiqot va ishlanmalar olib borish uchun mo‘ljallangan:*
</div>

- **🤖 Robototexnika va avtonom tizimlar** — harakatni rejalashtirish, boshqaruv
- **👁️ Kompyuter ko‘rishi** — 3D skanerlash, chuqurlikni aniqlash, obyektlarni tanish
- **🧠 Sun’iy intellekt** — model o‘qitish, inferens, mashinaviy o‘rganish
- **🌐 Edge hisoblash** — real vaqt rejimidagi hisoblash tizimlari

---

<div align="center">

## 🖥️ Markaziy AI Server (Infratuzilma)

[![Infrastructure](https://img.shields.io/badge/Infrastructure-Central%20AI%20Server-darkblue?logo=serverfault)](https://serverfault.com/)
[![Architecture](https://img.shields.io/badge/System-Architecture-blue?logo=diagramsdotnet)](https://www.drawio.com/)
[![Backend](https://img.shields.io/badge/Backend-Server--Side-gray?logo=linux)](https://www.kernel.org/)

</div>


<table>
<tr>
<td width="65%" valign="top">

> ⚠️ **Muhim eslatma**  
> Server apparatiga to‘g‘ridan-to‘g‘ri kirish faqat administratorlar uchun ruxsat etilgan.

### Maqsad
Markaziy AI server quyidagi vazifalar uchun ishlatiladi:
- Sun’iy intellekt modellari o‘qitish
- Katta hajmdagi hisoblashlar
- Ma’lumotlarni qayta ishlash
- Robotlar va ko‘rish tizimlari uchun backend xizmatlar

### Foydalanuvchi bilan o‘zaro aloqa
Foydalanuvchilar serverga **faqat masofadan** ulanadi:
- SSH
- Masofaviy ish stoli
- Veb interfeyslar

### Administrator tomonidan boshqariladi
- CPU va GPU
- Operativ xotira
- Disk tizimlari
- Quvvat va sovitish

</td>
<td width="35%" align="right">
<img src="../images/ai_server.png" alt="AI Server" width="100%"/>
</td>
</tr>
</table>

---

<div align="center">

## 🖥️ Ishchi stansiyalar (x10) — ThinkStation P3 Tower Gen 2

[![Workstation](https://img.shields.io/badge/Workstations-ThinkStation%20P3%20Tower%20Gen%202-black?logo=lenovo)](https://www.lenovo.com/us/en/p/workstations/thinkstation-p-series/lenovo-thinkstation-p3-tower-gen-2-intel-workstation/30hs000nus)
[![Specs PDF](https://img.shields.io/badge/Specs-PDF-blue?logo=adobereader)](https://psref.lenovo.com/syspool/Sys/PDF/ThinkStation/ThinkStation_P3_Tower_Gen_2/ThinkStation_P3_Tower_Gen_2_Spec.pdf)
</div>

<table>
<tr>
<td width="65%" valign="top">

### Maqsad
Bu ishchi stansiyalar foydalanuvchilar uchun mo‘ljallangan:
- Dastur ishlab chiqish
- AI tajribalar
- Ma’lumotlarni tahlil qilish
- Markaziy serverga ulanish

### Kimlar foydalanishi mumkin
- Talabalar
- Tadqiqotchilar
- Dasturchilar
- Laboratoriya xodimlari

</td>
<td width="35%" align="right">
<img src="../images/power_station.png" alt="Workstation" width="100%"/>
</td>
</tr>
</table>

<table>
<tr>
<td width="65%" valign="top">

### Ishni boshlash
1. Kompyuterni yoqing
2. Windows 11 tizimiga kiring
3. Kerakli dasturlarni oching
4. Lokal yoki masofaviy hisoblashni boshlang

</td>
<td width="35%" align="right">
<img src="../images/power.png" alt="Power" width="100%"/>
</td>
</tr>
</table>

<table>
<tr>
<td width="65%" valign="top">

### GPU mavjudligini tekshirish
```powershell
nvidia-smi

import torch
print(torch.cuda.is_available())
```
</td> <td width="35%" align="right"> <img src="../images/gpu_check.png" alt="GPU Check" width="100%"/> </td> </tr> </table>

<div align="center">

## 👁️ Stereo kamera — Intel RealSense D455

![Category](https://img.shields.io/badge/Category-Robotics-blue)
[![GitHub](https://img.shields.io/badge/GitHub-IntelRealSense%2Flibrealsense-black?logo=github)](https://github.com/IntelRealSense/librealsense)
[![Docs](https://img.shields.io/badge/Docs-Intel%20RealSense-blue?logo=readthedocs)](https://www.realsenseai.com/products/real-sense-depth-camera-d455f/)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Maqsad
Intel RealSense D455 — **chuqurlikni aniqlovchi stereo kamera** bo‘lib, quyidagi vazifalar uchun ishlatiladi:
- To‘siqlardan qochish
- 3D skanerlash va rekonstruksiya
- Chuqurlikka asoslangan kompyuter ko‘rishi
- Robot idrok (perception) tizimlari

</td> 
<td width="35%" align="right">
<img src="../images/stereo_camera.png" alt="Intel RealSense D455" width="100%"/> 
</td> </tr> </table>
    

<table>
<tr>
<td width="65%" valign="top">

### Qanday foydalaniladi
1. Kamerani USB orqali ulang
2. Intel RealSense SDK ni o‘rnating
3. Dasturingizni yoki skriptingizni ishga tushiring
4. API orqali RGB va chuqurlik (depth) oqimlariga murojaat qiling

</td>
<td width="35%" align="right">
<img src="../images/camera.png" alt="Intel RealSense D455 Camera" width="100%"/> 
</td> </tr> </table>

### Namuna
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

## 🤖 Insonsimon robot — Unitree G1

[![Humanoid Robot](https://img.shields.io/badge/Humanoid%20Robot-Unitree%20G1-blue?logo=robotframework)](https://www.unitree.com/g1/)
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics)
[![unitree_sdk2](https://img.shields.io/badge/SDK-unitree_sdk2-blue?logo=github)](https://github.com/unitreerobotics/unitree_sdk2)
[![unitree_ros](https://img.shields.io/badge/ROS-unitree_ros-blue?logo=ros)](https://github.com/unitreerobotics/unitree_ros)
[![unitree_sdk2_python](https://img.shields.io/badge/Python-SDK%20Python-blue?logo=python)](https://github.com/unitreerobotics/unitree_sdk2_python)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Maqsad
**Unitree G1** — bu **insonsimon tadqiqot roboti** bo‘lib, quyidagi yo‘nalishlarda qo‘llaniladi:
- Harakatlanish va lokomotsiya tadqiqotlari
- Muvozanat va harakatni boshqarish
- Inson–robot o‘zaro aloqasi
- Ilg‘or robototexnika tajribalari

---

### Xavfsizlik bo‘yicha ogohlantirish ⚠️
- Faqat maxsus belgilangan hududlarda foydalaning
- Robot harakatlanayotganda xavfsiz masofani saqlang
- Bo‘g‘inlar yoki aktuatorlarni to‘sib qo‘ymang
- Favqulodda to‘xtatish (Emergency Stop) tugmasi har doim ochiq va mavjud bo‘lishi shart

---

### Foydalanuvchilar robot bilan qanday ishlaydi
Foydalanuvchilar robotni quyidagi vositalar orqali boshqaradi:
- Rasmiy boshqaruv dasturi
- SDK va API interfeyslari
- Oldindan tayyorlangan harakat skriptlari

---

### Robotdan foydalanishni boshlash tartibi
1. Robotni tekis va barqaror yuzaga joylashtiring
2. Robotni yoqing
3. Boshqaruv tarmog‘iga ulang
4. Boshqaruv dasturini yoki SDK ni ishga tushiring
5. Harakatni boshlashdan oldin tizim tekshiruvlarini bajaring

</td>
<td width="35%" align="right">
<img src="../images/robot.png" alt="Unitree G1 Insonsimon Roboti" width="100%"/>
</td> </tr> </table>

---

### Namuna 
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

## 🐕 To‘rt oyoqli robot — Unitree Go2

[![Quadruped Robot](https://img.shields.io/badge/Quadruped%20Robot-Unitree%20Go2-blue?logo=robotframework)](https://www.unitree-robot.com/products/unitree-go2.html) &nbsp;
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics) &nbsp;
[![Go2 ROS 2](https://img.shields.io/badge/ROS2-Go2%20Support-brightgreen?logo=ros)](https://github.com/Unitree-Go2-Robot/go2_robot)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Maqsad
**Unitree Go2** — bu **to‘rt oyoqli robot platformasi** bo‘lib, quyidagi yo‘nalishlar uchun mo‘ljallangan:
- Robototexnika bo‘yicha tadqiqotlar va ta’lim
- Avtonom navigatsiya tajribalari
- Sun’iy intellekt asosida idrok va harakatni sinovdan o‘tkazish
- Inson–robot o‘zaro aloqasi

---

### Xavfsizlik bo‘yicha ogohlantirish ⚠️
- Faqat tekis va to‘siqlarsiz yuzalarda ishlating
- Harakatlanayotgan oyoqlarga qo‘llarni yaqinlashtirmang
- Zarurat bo‘lsa favqulodda to‘xtatish (Emergency Stop) dan foydalaning
- Zinapoyalar yoki baland chekkalar yaqinida ishlatmang

---

### Foydalanuvchilar robot bilan qanday ishlaydi
Foydalanuvchilar robotni quyidagi usullar orqali boshqaradi:
- Rasmiy boshqaruv ilovasi
- SDK / API interfeysi
- Oldindan belgilangan harakat rejimlari

---

### Robotdan foydalanishni boshlash tartibi
1. Robotni barqaror va tekis yuzaga joylashtiring
2. Robotni yoqing
3. Boshqaruv dasturi orqali ulanib oling
4. Agar kerak bo‘lsa, kalibrlashni bajaring
5. Harakat rejimini yoki avtonom rejimni tanlang

</td>
<td width="35%" align="right">
<img src="../images/dog.png" alt="Unitree Go2 To‘rt Oyoqli Roboti" width="100%"/> 
</td> </tr> </table> 

---

### Namuna
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

## 🦾 Robotlashtirilgan manipulyator

[![Quadruped Robot](https://img.shields.io/badge/Quadruped%20Robot-Unitree%20Go2-blue?logo=robotframework)](https://www.unitree.com/en/go2)
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics)
[![Go2 ROS 2](https://img.shields.io/badge/ROS2-Go2%20Support-brightgreen?logo=ros)](https://github.com/YasiruDEX/unitree-go2-ros2)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Maqsad
**Robotlashtirilgan manipulyator** quyidagi vazifalar uchun mo‘ljallangan:
- Ilmiy tadqiqotlar va ishlab chiqish ishlari
- Harakatni boshqarish algoritmlarini sinovdan o‘tkazish
- Obyektlarni ushlash, ko‘chirish va joylashtirish
- Kompyuter ko‘rish va sun’iy intellekt tizimlari bilan integratsiya
- Takrorlanuvchi jarayonlarni avtomatlashtirish

---

### Asosiy funksiyalar
- Yuqori aniqlikdagi fazoviy joylashuv
- Obyektlarni ushlash, ko‘chirish va joyiga qo‘yish
- Dasturlashtiriladigan harakat trayektoriyalari
- Qo‘lda va avtomatik ishlash rejimlari

---

### Xavfsizlik choralari ⚠️
- Ishlayotgan vaqtda qo‘llarni ish hududiga kiritmang
- Zarurat bo‘lsa favqulodda to‘xtatish tugmasidan foydalaning
- Manipulyatorni ish stoliga yoki platformaga mustahkam mahkamlang
- Ishlashdan oldin yuk ko‘tarish chegarasini tekshiring

---

### Foydalanuvchi bilan o‘zaro aloqa
Manipulyator quyidagi usullar orqali boshqariladi:
- Dasturiy interfeys (SDK / API)
- Qo‘lda boshqarish (teach / jog rejimi)
- Oldindan yozilgan harakat skriptlari

---

### Ishni boshlash tartibi
1. Manipulyatorni barqaror yuzaga mahkamlang
2. Quvvat va boshqaruv interfeyslarini ulang
3. Boshqaruv dasturini ishga tushiring
4. O‘qlarni (axis) kalibrlashni bajaring
5. Ishlash rejimini tanlang (qo‘lda yoki avtomatik)

</td>
<td width="35%" align="right">
<img src="../images/robotic_manipulator.png" alt="Robotlashtirilgan manipulyator" width="100%"/> 
</td> </tr> </table> 

### Namuna
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
 
## 🤖 Sanoat roboti — FANUC LR Mate 200iC/5L (R-30iA kontrolleri)

[![Industrial Robot](https://img.shields.io/badge/Robot-FANUC%20LR%20Mate%20200iC%2F5L-red?logo=fanuc)](https://www.fanucamerica.com/products/robots/series/lr-mate)
[![Official GitHub](https://img.shields.io/badge/GitHub-FANUC%20ROS%202%20Driver-black?logo=github)](https://github.com/FANUC-CORPORATION/fanuc_driver)
[![ROS2 Support](https://img.shields.io/badge/ROS2-FANUC%20ROS2%20Docs-brightgreen?logo=ros)](https://fanuc-corporation.github.io/fanuc_driver_doc/main/)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Model
- **Robot:** FANUC LR Mate 200iC/5L  
- **Kontroller:** FANUC R-30iA

---

### Maqsad
**FANUC LR Mate 200iC/5L** — ixcham sanoat roboti bo‘lib, quyidagi vazifalar uchun mo‘ljallangan:
- Avtomatlashtirish bo‘yicha tadqiqotlar
- Sanoat ta’limi va treninglar
- Pick-and-place (olish va joylashtirish) operatsiyalari
- Yig‘ish (assembly) va materiallarni ko‘chirish
- Ko‘rish tizimi asosidagi robotlashtirilgan vazifalar

---

### Asosiy imkoniyatlar
- 6 o‘qli bo‘g‘inli robot qo‘li
- Yuqori aniqlik va takrorlanuvchanlik
- Kengaytirilgan yetib borish masofasi (5L versiyasi)
- Ko‘rish tizimlari va tashqi sensorlar bilan moslik
- Onlayn va oflayn dasturlashni qo‘llab-quvvatlaydi

---

### Foydalanuvchi bilan o‘zaro aloqa
Robot quyidagi vositalar orqali boshqariladi:
- FANUC Teach Pendant
- FANUC R-30iA kontrolleri
- **TP** yoki **KAREL** tillarida yozilgan robot dasturlari
- PLC va ko‘rish tizimlari bilan ixtiyoriy integratsiya

---

### Asosiy foydalanish jarayoni
1. R-30iA kontrollerini yoqing
2. Favqulodda to‘xtatish (Emergency Stop) ni bo‘shating
3. Ishlash rejimini tanlang (Teach / Auto)
4. Robotni kerakli pozitsiyalarga qo‘lda olib boring (jog)
5. Teach Pendant yordamida nuqtalarni yozib oling
6. Robot dasturini ishga tushiring yoki sinovdan o‘tkazing

</td>
<td width="35%" align="right">
<img src="../images/fanuc_img.png" alt="FANUC LR Mate 200iC/5L sanoat roboti" width="100%"/> 
</td> </tr> </table> 

### Misol — Oddiy Pick & Place mantiqi (kontseptual)
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

## 🦾 Robotlashtirilgan Manipulyator To‘plami (Kontroller asosidagi mexanik qo‘l)
[![Official GitHub](https://img.shields.io/badge/GitHub‑open_manipulator-black?logo=github)](https://github.com/ROBOTIS-GIT/open_manipulator)  

</div>


<table>
<tr>
<td width="65%" valign="top">

### Turi
- **Kategoriya:** Ta’limiy / Tadqiqot uchun robotlashtirilgan manipulyator
- **Konfiguratsiya:** Kontrollerga ega modulli mexanik qo‘l

---

### Maqsad
Ushbu **robotlashtirilgan manipulyator to‘plami** quyidagi yo‘nalishlar uchun mo‘ljallangan:
- Robototexnika bo‘yicha ta’lim va treninglar
- Harakatni boshqarish va kinematikani o‘rganish
- Avtomatlashtirish yechimlarini prototiplash
- Ushlash (grasping) va manipulyatsiya algoritmlarini sinovdan o‘tkazish

---

### Asosiy imkoniyatlar
- Ko‘p bo‘g‘inli artikulyatsiyalangan mexanik qo‘l
- Kontroller asosida boshqarish
- Servo yoki stepper motorlarni qo‘llab-quvvatlash
- End-effektorlarni ulash imkoniyati (gripper, vakuumli so‘rg‘ich, asboblar)
- Sensorlar bilan kengaytirish imkoniyati  
  (chegara kalitlari, kameralar, kuch sensorlari)

---

### Foydalanuvchi bilan o‘zaro aloqa
Foydalanuvchilar manipulyator bilan quyidagi usullar orqali ishlaydi:
- Maxsus kontroller plata
- Kompyuterga ulanish (USB / Serial)
- Python, C/C++ yoki Arduino-uslubidagi kodlar orqali dasturlash
- Bo‘g‘inlarni qo‘lda va dasturiy boshqarish

---

### Asosiy foydalanish jarayoni
1. Manipulyatorni kontrollerga ulang
2. Tizimni yoqing
3. Bo‘g‘inlarning boshlang‘ich holatini sozlang
4. Bo‘g‘inlarni qo‘lda yoki dastur orqali boshqaring
5. End-effektorni ulang va sozlang
6. Harakat ketma-ketliklarini bajaring

</td>
<td width="35%" align="right">
<img src="../images/img_1.png" alt="Robotlashtirilgan manipulyator to‘plami" width="100%"/> 
</td> </tr> </table> 

### Misol — Bo‘g‘inlarni oddiy boshqarish (kontseptual)
```
SET joint1 = 45°
SET joint2 = 30°
SET joint3 = 15°
OPEN gripper
MOVE to target position
CLOSE gripper
```

---

<div align="center">

## 🏁 Hujjatlarning oxiri

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