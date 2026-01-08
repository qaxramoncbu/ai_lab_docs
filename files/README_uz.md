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

## 🏢 Laboratoriya haqida

Sun’iy intellekt va robototexnika laboratoriyasi quyidagi yo‘nalishlarda
tadqiqot va ishlanmalar olib borish uchun mo‘ljallangan:

- **🤖 Robototexnika va avtonom tizimlar** — harakatni rejalashtirish, boshqaruv
- **👁️ Kompyuter ko‘rishi** — 3D skanerlash, chuqurlikni aniqlash, obyektlarni tanish
- **🧠 Sun’iy intellekt** — model o‘qitish, inferens, mashinaviy o‘rganish
- **🌐 Edge hisoblash** — real vaqt rejimidagi hisoblash tizimlari

---

## 🖥️ Markaziy AI Server (Infratuzilma)

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

## 🖥️ Ishchi stansiyalar (x10) — ThinkStation P3 Tower Gen 2

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



## 👁️ Stereo kamera — Intel RealSense D455

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

## 🤖 Insonsimon robot — Unitree G1

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
robot.stand()
robot.walk_forward(steps=3)
robot.turn(angle=30)
```

---

## 🐕 To‘rt oyoqli robot — Unitree Go2

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
```python
robot.stand()
robot.walk_forward(distance=2.0)
robot.turn(angle=45)
robot.stop()
```

## 🦾 Robotlashtirilgan manipulyator

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
arm.move_to(x=0.3, y=0.2, z=0.15)
arm.open_gripper()
arm.move_to(x=0.3, y=0.2, z=0.05)
arm.close_gripper()
arm.move_to_home()
```

## 🤖 Sanoat roboti — FANUC LR Mate 200iC/5L (R-30iA kontrolleri)

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
```text
MOVE TO HOME
MOVE TO PICK POSITION
CLOSE GRIPPER
MOVE TO PLACE POSITION
OPEN GRIPPER
RETURN TO HOME
```

## 🦾 Robotlashtirilgan Manipulyator To‘plami (Kontroller asosidagi mexanik qo‘l)

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