# 📚 LEARNINGLOG

## Project: Turn-Based Battle Game (Python CLI)

---

## 1. Project Overview

Turn-Based Battle Game เป็นเกมต่อสู้แบบ Text-based ที่พัฒนาด้วยภาษา Python โดยผู้เล่นสามารถเลือก Action ในแต่ละ Turn ได้แก่ Attack, Punch of Luck, Heal และ Defend เพื่อแข่งขันกับ Enemy ที่มีระบบตัดสินใจแบบ Simple AI

เป้าหมายของโปรเจกต์คือการนำความรู้พื้นฐาน Python มาประยุกต์ใช้กับการสร้างโปรแกรมที่มี Interaction กับผู้ใช้ โดยเน้นเรื่อง:

- Data Structure
- Control Flow
- Loop
- Input Validation
- Problem Solving

---

# 📝 Development Learning Process

---

# 1. Creating Basic Battle System

## Objective

สร้างระบบการต่อสู้พื้นฐานระหว่าง Player และ Enemy

## Implementation

สิ่งที่พัฒนา:

- Player HP system
- Enemy HP system
- Turn-based game loop
- Basic attack system
- Random damage system

ตัวอย่าง:

```python
while player_hp > 0 and enemy_hp > 0:
```

## Problem Encountered

ไม่เข้าใจวิธีควบคุมการทำงานของเกม เช่น

- เกมควรหยุดเมื่อไหร่
- จะตรวจสอบว่าใครชนะอย่างไร

## Solution

ใช้ while loop ร่วมกับ condition เพื่อตรวจสอบ HP ของทั้งสองฝ่าย

## Learning

- เข้าใจการใช้ loop ในการควบคุม process ที่ทำซ้ำ
- เข้าใจการใช้ condition เพื่อควบคุม flow ของโปรแกรม

---

# 2. Designing Skill System

## Objective

เพิ่ม Action ให้ผู้เล่นสามารถเลือกคำสั่งได้หลายแบบ

Skill ที่เพิ่ม:

- Attack
- Punch of Luck
- Heal
- Defend


## Problem Encountered

เมื่อใช้ if/elif จำนวนมาก โค้ดเริ่มมีความซับซ้อน

ตัวอย่าง:

```python
if action == "attack":
    ...
elif action == "heal":
    ...
elif action == "defend":
    ...
```

เมื่อเพิ่ม skill ใหม่จะต้องแก้หลายจุด


## Solution

เปลี่ยนมาใช้ Dictionary เพื่อจัดเก็บข้อมูล Skill


```python
skills = {
    "1": {
        "name": "attack",
        "type": "damage",
        "value": (10,20)
    }
}
```


## Learning

- เรียนรู้การใช้ Dictionary เป็น Data Structure
- ลดความซ้ำซ้อนของ Code
- ทำให้สามารถเพิ่ม Feature ได้ง่ายขึ้น

---

# 3. Input Validation

## Objective

ป้องกัน User Input ที่ไม่ถูกต้อง


## Problem Encountered

ผู้ใช้อาจกรอกค่าที่ไม่มีอยู่ในระบบ


Example:

```
Enter number: 5
```


## Solution

เพิ่มระบบตรวจสอบ Input


```python
if choice in skills:
    return choice
else:
    print("Invalid input")
```


## Learning

- เข้าใจ Defensive Programming
- สามารถจัดการ Error จาก User Input
- ทำให้โปรแกรมไม่ Crash

---

# 4. Random Damage System

## Objective

ทำให้การต่อสู้มีความหลากหลายมากขึ้น


## Implementation

ใช้ random module ในการสุ่ม Damage


```python
damage = random.randint(10,20)
```


## Problem Encountered

การโจมตีแบบ Fixed Damage ทำให้เกมไม่มีความแตกต่างในแต่ละรอบ


## Solution

เพิ่ม Random Damage เพื่อสร้างความไม่แน่นอน


## Learning

- เรียนรู้การ Import และใช้งาน Module
- เข้าใจการสร้าง Game Mechanic ด้วย Random

---

# 5. Creating Enemy AI

## Objective

สร้างระบบให้ Enemy สามารถเลือก Action ได้เอง


## Problem Encountered

การสุ่ม Action อย่างเดียวทำให้ Enemy ไม่มี Logic


## Solution

เพิ่ม Decision Making


```python
if enemy_hp < 30:
    enemy_action = "heal"
else:
    enemy_action = random.choice(
        ["attack","attack","heal"]
    )
```


## Learning

- เข้าใจพื้นฐานของ AI Decision Logic
- ใช้ Conditional Statement ในการสร้างพฤติกรรมของตัวละคร

---

# 6. Status Management System

## Objective

เพิ่มระบบ Defend ที่ส่งผลต่อ Damage ที่ได้รับ


## Problem Encountered

จำเป็นต้องเก็บสถานะของ Player ระหว่าง Turn


## Solution

สร้าง Status Dictionary


```python
player_status = {
    "defend": False
}
```


เมื่อใช้ Defend:

```python
player_status["defend"] = True
```


## Learning

- เข้าใจการจัดการ State ของโปรแกรม
- เข้าใจการเก็บข้อมูลที่เปลี่ยนแปลงระหว่าง Runtime

---

# 7. Debugging Process

## Problem 1: random is not defined


Error:

```
NameError: name 'random' is not defined
```


Cause:

ไม่ได้ Import random module


Solution:


```python
import random
```


---

## Problem 2: Code Structure Too Complex


Cause:

จำนวน if/elif เพิ่มขึ้นเมื่อเพิ่ม Feature


Solution:

ใช้ Dictionary-based Design


Result:

- Code อ่านง่ายขึ้น
- เพิ่ม Skill ใหม่ได้ง่าย


---

## Problem 3: Invalid User Input


Cause:

ไม่มีการตรวจสอบ Input


Solution:

เพิ่ม Input Validation Loop


Result:

โปรแกรมสามารถรับมือกับข้อมูลผิดได้

---

# 🎯 Final Reflection

จากการทำโปรเจกต์ Turn-Based Battle Game ได้เรียนรู้:

- การใช้ Python Data Structure โดยเฉพาะ Dictionary
- การออกแบบ Control Flow ด้วย if/elif/else
- การใช้ Loop เพื่อสร้าง Interactive Program
- การจัดการ User Input
- การ Debug และแก้ไขปัญหา
- การออกแบบโปรแกรมให้สามารถขยายต่อได้


## Group Learning Outcome Mapping

| Learning Outcome | Implementation |
|---|---|
| LO1 Data Structure | ใช้ Dictionary จัดการ Skill และ Status |
| LO2 Collection Manipulation | จัดการข้อมูล Player, Enemy และ Skill |
| LO3 Control Flow | ใช้ Loop และ Conditional Statement |
| LO4 Defensive Programming | Input Validation |
| LO5 Process Documentation | บันทึก Learning Process |

---

# End of Learning Log