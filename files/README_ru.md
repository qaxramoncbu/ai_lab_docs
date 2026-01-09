<div align="center">

# 🤖 Лаборатория ИИ и Робототехники
## Инвентаризация оборудования и руководство по использованию

![Category](https://img.shields.io/badge/Категория-Робототехника-blue)
![Category](https://img.shields.io/badge/Категория-Компьютерное%20зрение-purple)
![Category](https://img.shields.io/badge/Категория-Искусственный%20интеллект-green)
![Access](https://img.shields.io/badge/Доступ-Ограничен-red)
![Usage](https://img.shields.io/badge/Использование-Требуется%20программирование-orange)
![OS](https://img.shields.io/badge/ОС-Linux%20%7C%20Windows-blue)
![Code](https://img.shields.io/badge/Код-Python-yellow)
![Framework](https://img.shields.io/badge/Фреймворк-ROS-green)
![Status](https://img.shields.io/badge/Статус-Работает-brightgreen)
![Version](https://img.shields.io/badge/Версия-1.0-lightgrey)

*Подробная документация по оборудованию лаборатории и правилам эксплуатации*

</div>

---

<div align="center">

## 🏢 Обзор лаборатории
![Category](https://img.shields.io/badge/Category-Robotics-blue)
![Laboratory](https://img.shields.io/badge/Laboratory-Lab-purple?logo=atom)
![Overview](https://img.shields.io/badge/Overview-Project-blue?logo=abstract)

*Лаборатория искусственного интеллекта и робототехники предоставляет современную исследовательскую инфраструктуру для:*
</div>

- **🤖 Робототехники и автономных систем** — планирование движения, управление, взаимодействие человек–робот  
- **👁️ Компьютерного зрения и восприятия** — 3D-реконструкция, обнаружение объектов, анализ глубины  
- **🧠 Искусственного интеллекта и машинного обучения** — обучение моделей и инференс  
- **🌐 Пограничных вычислений и IoT** — обработка данных в реальном времени  

---


<div align="center">

## 🖥️ Центральный AI-сервер (Инфраструктурный обзор)

[![Infrastructure](https://img.shields.io/badge/Infrastructure-Central%20AI%20Server-darkblue?logo=serverfault)](https://serverfault.com/)
[![Architecture](https://img.shields.io/badge/System-Architecture-blue?logo=diagramsdotnet)](https://www.drawio.com/)
[![Backend](https://img.shields.io/badge/Backend-Server--Side-gray?logo=linux)](https://www.kernel.org/)
</div>

<table>
<tr>
<td width="65%" valign="top">

> ⚠️ **Уведомление по инфраструктуре**  
> Прямой доступ к серверному оборудованию разрешён только администраторам системы.

### Назначение
AI-сервер — это **централизованная вычислительная платформа**, используемая для:
- Обучения моделей ИИ
- Масштабного инференса
- Обработки данных
- Серверных сервисов для робототехнических и vision-систем

### Взаимодействие с пользователем
Пользователи работают с сервером **только удалённо**:
- Доступ по SSH
- Удалённый рабочий стол или веб-интерфейсы
- Запуск заданий и вычислительных задач

### Управляемые компоненты
Следующие компоненты обслуживаются администраторами и **не требуют действий пользователя**:
- Серверный корпус и стойка
- CPU и GPU
- Оперативная память и хранилища
- Питание и системы охлаждения

📌 По вопросам доступа обращайтесь к администратору лаборатории.

</td>
<td width="35%" align="right">
<img src="../images/ai_server.png" alt="AI сервер в стойке" width="100%"/>
</td>
</tr>
</table>

---

<div align="center">

## 🖥️ Рабочие станции (x10) — ThinkStation P3 Tower Gen 2

[![Workstation](https://img.shields.io/badge/Workstations-ThinkStation%20P3%20Tower%20Gen%202-black?logo=lenovo)](https://www.lenovo.com/us/en/p/workstations/thinkstation-p-series/lenovo-thinkstation-p3-tower-gen-2-intel-workstation/30hs000nus)
[![Specs PDF](https://img.shields.io/badge/Specs-PDF-blue?logo=adobereader)](https://psref.lenovo.com/syspool/Sys/PDF/ThinkStation/ThinkStation_P3_Tower_Gen_2/ThinkStation_P3_Tower_Gen_2_Spec.pdf)
</div>

<table>
<tr>
<td width="65%" valign="top">

### Назначение
Рабочие станции являются **пользовательскими машинами разработки**, предназначенными для:
- Разработки программного обеспечения
- Экспериментов с ИИ и машинным обучением
- Обработки и визуализации данных
- Подключения к центральному AI-серверу

Каждая станция оснащена выделенным GPU.

---

### Кто может использовать
- Студенты  
- Исследователи  
- Разработчики  
- Сотрудники лаборатории с утверждёнными проектами  

</td>
<td width="35%" align="right">
<img src="../images/power_station.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/>
</td>
</tr>
</table>

<table>
<tr>
<td width="65%" valign="top">

### Начало работы
1. Включите рабочую станцию  
2. Войдите в **Windows 11 Pro**  
3. Запустите инструменты разработки (VS Code, Python, Docker и др.)  
4. Выполняйте локальные задачи или подключайтесь к серверу  

---

### Возможности пользователя
- Написание, запуск и отладка кода  
- Запуск GPU-ускоренных приложений  
- Обучение и тестирование моделей ИИ  
- Визуализация данных  
- Доступ к сетевым ресурсам  

</td>
<td width="35%" align="right">
<img src="../images/power.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/>
</td>
</tr>
</table>

<table>
<tr>
<td width="65%" valign="top">

### Проверка доступности GPU
```powershell
powershell
nvidia-smi

import torch
print(torch.cuda.is_available())
```

### Примечания
- Немедленно сообщайте о любых аппаратных или программных неисправностях
- Всегда соблюдайте правила эксплуатации лаборатории и требования техники безопасности

</td> 
<td width="35%" align="right">
<img src="../images/gpu_check.png" alt="ThinkStation P3 Tower Gen 2" width="100%"/> 
</td> </tr> </table>

<div align="center">

## 👁️ Стереокамера — Intel RealSense D455

![Category](https://img.shields.io/badge/Category-Robotics-blue)
[![GitHub](https://img.shields.io/badge/GitHub-IntelRealSense%2Flibrealsense-black?logo=github)](https://github.com/IntelRealSense/librealsense)
[![Docs](https://img.shields.io/badge/Docs-Intel%20RealSense-blue?logo=readthedocs)](https://www.realsenseai.com/products/real-sense-depth-camera-d455f/)


</div>

<table>
<tr>
<td width="65%" valign="top">

### Назначение
Intel RealSense D455 — это **стереокамера с измерением глубины**, используемая для:
- Обхода препятствий
- 3D-сканирования и реконструкции
- Компьютерного зрения с учётом глубины
- Систем восприятия в робототехнике

</td> 
<td width="35%" align="right">
<img src="../images/stereo_camera.png" alt="Intel RealSense D455" width="100%"/> 
</td> </tr> </table>
    

<table>
<tr>
<td width="65%" valign="top">

### Порядок использования
1. Подключите камеру по USB  
2. Установите Intel RealSense SDK  
3. Запустите ваше приложение или скрипт  
4. Получайте RGB- и depth-потоки через API  

</td>
<td width="35%" align="right">
<img src="../images/camera.png" alt="Intel RealSense D455" width="100%"/> 
</td> </tr> </table>


### Пример базового кода (RGB-поток)
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

## 🤖 Человекоподобный робот — Unitree G1

[![Humanoid Robot](https://img.shields.io/badge/Humanoid%20Robot-Unitree%20G1-blue?logo=robotframework)](https://www.unitree.com/g1/)
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics)
[![unitree_sdk2](https://img.shields.io/badge/SDK-unitree_sdk2-blue?logo=github)](https://github.com/unitreerobotics/unitree_sdk2)
[![unitree_ros](https://img.shields.io/badge/ROS-unitree_ros-blue?logo=ros)](https://github.com/unitreerobotics/unitree_ros)
[![unitree_sdk2_python](https://img.shields.io/badge/Python-SDK%20Python-blue?logo=python)](https://github.com/unitreerobotics/unitree_sdk2_python)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Назначение
**Unitree G1** — это **человекоподобный исследовательский робот**, используемый для:
- Исследований мобильности и передвижения
- Управления балансом и движением
- Взаимодействия человек–робот
- Проведения передовых экспериментов в робототехнике

---

### Уведомление по безопасности ⚠️
- Эксплуатируйте робота только в специально отведённых зонах
- Соблюдайте безопасную дистанцию во время движения
- Никогда не блокируйте суставы и исполнительные механизмы
- Кнопка аварийной остановки должна быть всегда доступна

---

### Взаимодействие пользователя с роботом
Пользователи управляют роботом с помощью:
- Официального программного обеспечения
- SDK и API
- Предустановленных сценариев движения

---

### Порядок начала работы
1. Установите робота на устойчивую поверхность  
2. Включите питание робота  
3. Подключитесь к управляющей сети  
4. Запустите управляющее ПО или SDK  
5. Выполните проверку системы перед началом движения  

</td>
<td width="35%" align="right">
<img src="../images/robot.png" alt="Человекоподобный робот Unitree G1" width="100%"/>
</td> </tr> </table>

### Пример базового управления
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

## 🐕 Четвероногий робот — Unitree Go2

[![Quadruped Robot](https://img.shields.io/badge/Quadruped%20Robot-Unitree%20Go2-blue?logo=robotframework)](https://www.unitree-robot.com/products/unitree-go2.html) &nbsp;
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics) &nbsp;
[![Go2 ROS 2](https://img.shields.io/badge/ROS2-Go2%20Support-brightgreen?logo=ros)](https://github.com/Unitree-Go2-Robot/go2_robot)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Назначение
**Unitree Go2** — это **четвероногая роботизированная платформа**, предназначенная для:
- Исследований и обучения в области робототехники
- Экспериментов с автономной навигацией
- Тестирования ИИ-алгоритмов восприятия и передвижения
- Взаимодействия человек–робот

---

### Уведомление по безопасности ⚠️
- Используйте робота только на ровных поверхностях без препятствий
- Держите руки подальше от движущихся ног
- Используйте аварийную остановку при необходимости
- Не эксплуатируйте робота рядом с лестницами и краями платформ

---

### Взаимодействие пользователя с роботом
Пользователи управляют роботом с помощью:
- Официального управляющего приложения
- Интерфейса SDK / API
- Предустановленных режимов движения

---

### Порядок начала работы
1. Установите робота на устойчивую поверхность  
2. Включите питание  
3. Подключитесь через управляющее программное обеспечение  
4. При необходимости выполните калибровку  
5. Выберите режим движения или автономный режим  

</td>
<td width="35%" align="right">
<img src="../images/dog.png" alt="Четвероногий робот Unitree Go2" width="100%"/> 
</td> </tr> </table> 

### Пример базового движения
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

## 🦾 Роботизированный манипулятор

[![Quadruped Robot](https://img.shields.io/badge/Quadruped%20Robot-Unitree%20Go2-blue?logo=robotframework)](https://www.unitree.com/en/go2)
[![Official GitHub](https://img.shields.io/badge/GitHub-Unitree%20Robotics-black?logo=github)](https://github.com/unitreerobotics)
[![Go2 ROS 2](https://img.shields.io/badge/ROS2-Go2%20Support-brightgreen?logo=ros)](https://github.com/YasiruDEX/unitree-go2-ros2)

</div>

<table>
<tr>
<td width="65%" valign="top">

### Назначение
**Роботизированный манипулятор** предназначен для:
- Научно-исследовательских и опытно-конструкторских работ
- Тестирования алгоритмов управления движением
- Задач захвата и манипулирования объектами
- Интеграции с системами компьютерного зрения и ИИ
- Автоматизации повторяющихся операций

---

### Основные функции
- Точное позиционирование в пространстве
- Захват, перемещение и укладка объектов
- Программируемые траектории движения
- Ручной и автоматический режимы работы

---

### Меры безопасности ⚠️
- Не размещайте руки в рабочей зоне во время работы манипулятора
- Используйте аварийную остановку при необходимости
- Надёжно закрепите манипулятор на рабочей поверхности
- Проверяйте допустимую нагрузку перед началом работы

---

### Взаимодействие пользователя
Управление манипулятором осуществляется через:
- Программный интерфейс (SDK / API)
- Ручное управление (режим обучения / jog)
- Предустановленные сценарии движения

---

### Начало работы
1. Надёжно закрепите манипулятор на устойчивой поверхности  
2. Подключите питание и интерфейсы управления  
3. Запустите управляющее программное обеспечение  
4. Выполните калибровку осей  
5. Выберите режим работы (ручной или автоматический)  

</td>
<td width="35%" align="right">
<img src="../images/robotic_manipulator.png" alt="Роботизированный манипулятор" width="100%"/> 
</td> </tr> </table> 

### Пример базового управления
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

## 🤖 Промышленный робот — FANUC LR Mate 200iC/5L (контроллер R-30iA)

[![Industrial Robot](https://img.shields.io/badge/Robot-FANUC%20LR%20Mate%20200iC%2F5L-red?logo=fanuc)](https://www.fanucamerica.com/products/robots/series/lr-mate)
[![Official GitHub](https://img.shields.io/badge/GitHub-FANUC%20ROS%202%20Driver-black?logo=github)](https://github.com/FANUC-CORPORATION/fanuc_driver)
[![ROS2 Support](https://img.shields.io/badge/ROS2-FANUC%20ROS2%20Docs-brightgreen?logo=ros)](https://fanuc-corporation.github.io/fanuc_driver_doc/main/)

</div>


<table>
<tr>
<td width="65%" valign="top">

### Модель
- **Робот:** FANUC LR Mate 200iC/5L  
- **Контроллер:** FANUC R-30iA

---

### Назначение
**FANUC LR Mate 200iC/5L** — это компактный промышленный робот, предназначенный для:
- Исследований в области автоматизации
- Промышленного обучения и образования
- Операций pick-and-place
- Сборочных работ и перемещения материалов
- Роботизированных задач с использованием систем машинного зрения

---

### Ключевые возможности
- Шестиосевой шарнирно-сочленённый робот-манипулятор
- Высокая точность и повторяемость
- Версия с увеличенным радиусом действия (5L)
- Совместимость с системами машинного зрения и внешними датчиками
- Поддержка офлайн- и онлайн-программирования

---

### Взаимодействие с пользователем
Управление роботом осуществляется с помощью:
- Пульта обучения FANUC (Teach Pendant)
- Контроллера FANUC R-30iA
- Робот-программ, написанных на языках **TP** или **KAREL**
- Опциональной интеграции с ПЛК и системами технического зрения

---

### Базовый рабочий процесс
1. Включите контроллер R-30iA  
2. Снимите аварийную остановку  
3. Выберите режим работы (Teach / Auto)  
4. Переместите робот в нужные позиции (jog-режим)  
5. Запишите точки с помощью Teach Pendant  
6. Запустите или протестируйте программу робота  

</td>
<td width="35%" align="right">
<img src="../images/fanuc_img.png" alt="Промышленный робот FANUC LR Mate 200iC/5L" width="100%"/> 
</td> </tr> </table> 

### Пример — Простая логика Pick & Place (концептуально)
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

## 🦾 Набор роботизированного манипулятора (механическая рука с контроллером)
[![Official GitHub](https://img.shields.io/badge/GitHub‑open_manipulator-black?logo=github)](https://github.com/ROBOTIS-GIT/open_manipulator)  

</div>


<table>
<tr>
<td width="65%" valign="top">

### Тип
- **Категория:** Учебный / исследовательский роботизированный манипулятор  
- **Конфигурация:** Модульная механическая рука с контроллером управления  

---

### Назначение
Данный **набор роботизированного манипулятора** предназначен для:
- Обучения и подготовки в области робототехники
- Изучения управления движением и кинематики
- Прототипирования решений автоматизации
- Тестирования алгоритмов захвата и манипулирования объектами

---

### Ключевые возможности
- Многозвенная шарнирная механическая рука
- Управление на базе контроллера
- Поддержка сервоприводов или шаговых двигателей
- Поддержка сменных исполнительных механизмов  
  (захват, вакуумная присоска, инструменты)
- Возможность расширения с помощью датчиков  
  (концевые выключатели, камеры, датчики силы)

---

### Взаимодействие с пользователем
Пользователи взаимодействуют с манипулятором через:
- Специализированную плату контроллера
- Подключение к ПК (USB / Serial)
- Программирование на Python, C/C++ или Arduino-подобном коде
- Ручное и программное управление суставами

---

### Базовый порядок работы
1. Подключите манипулятор к контроллеру  
2. Включите питание системы  
3. Инициализируйте начальные положения суставов  
4. Управляйте суставами вручную или через программное обеспечение  
5. Установите и настройте исполнительный механизм  
6. Выполните заданные последовательности движений  

</td>
<td width="35%" align="right">
<img src="../images/img_1.png" alt="Набор роботизированного манипулятора" width="100%"/> 
</td> </tr> </table> 

### Пример — Базовое управление суставами (концептуально)
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

## 🏁 Конец документации

![Статус](https://img.shields.io/badge/Статус-Работает-brightgreen)
![Доступ](https://img.shields.io/badge/Доступ-Ограничен-red)
![Безопасность](https://img.shields.io/badge/Безопасность-Требуется%20обучение-orange)
![Документация](https://img.shields.io/badge/Документация-Завершена-blue)
![Поддержка](https://img.shields.io/badge/Поддержка-Активна-green)
![Конец](https://img.shields.io/badge/README-Конец%20файла-black)
![Версия](https://img.shields.io/badge/Версия-1.0-lightgrey)
![Обновлено](https://img.shields.io/badge/Последнее%20обновление-2026-blue)

---

</div>
