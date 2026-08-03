# ⚔️ Turn-Based Battle Game (Python CLI)

---

## 📌 Project Description

โปรเจกต์นี้เป็นเกมต่อสู้แบบ Turn-Based (Text-based CLI) ที่ผู้เล่นสามารถเลือกคำสั่งในแต่ละเทิร์น ได้แก่ Attack, Defend และ Heal เพื่อต่อสู้กับศัตรู (Enemy) โดยระบบจะทำงานจนกว่าฝ่ายใดฝ่ายหนึ่งจะมี HP = 0

---

## 🎯 Features

* ⚔️ Attack → สุ่ม damage
* 🛡️ Defend → ลด damage ที่ได้รับ
* 💊 Heal → ฟื้นฟู HP (ไม่เกิน max)
* 🤖 Enemy AI → ตัดสินใจเอง (attack / heal)
* 🔁 Loop gameplay → เล่นต่อเนื่อง
* ❗ Input Validation → กัน input ผิด

---

## ⚙️ How to Run

```bash
python main.py
```

---

## 🧠 Workflow

```text
Start 
→ Initialize HP 
→ Loop 
→ Player Input 
→ Validate 
→ Execute Action 
→ Enemy Turn 
→ Check HP 
→ Repeat 
→ End
```

---

# 📊 Kanban Backlog & Run

## 🗂️ Backlog

```md
- [ ] สร้างระบบ attack
- [ ] สร้างระบบ defend
- [ ] สร้างระบบ heal
- [ ] เพิ่ม input validation
- [ ] เพิ่ม enemy AI
- [ ] ปรับ UX (input เป็นตัวเลข)
```

## 🚀 In Progress

```md
- [x] ระบบ combat พื้นฐาน
- [x] ระบบ loop เกม
```

## ✅ Done

```md
- [x] ระบบ battle ทำงานครบ
- [x] เกมรันได้จริง
- [x] ไม่มี runtime error
```

---

# 🎯 Group Learning Outcomes

```md
- LO1: ใช้ dictionary ในการจัดการ action และ skill
- LO2: จัดการข้อมูล HP และ state ของผู้เล่น
- LO3: ใช้ while loop และ if/elif/else ควบคุมเกม
- LO4: มี input validation ป้องกัน error
- LO5: มี CHANGELOG และ LEARNINGLOG
```

---

# 🧾 Group Grading Rubric (Self Reflection)

## 🔹 Technical Rigor & Accuracy

```text
โค้ดทำงานถูกต้อง ใช้ dictionary + control flow อย่างเหมาะสม
มีการป้องกัน error เช่น invalid input
```

## 🔹 Architectural Usability

```text
ระบบ menu ใช้งานง่าย เล่นต่อเนื่องได้ และจบเกมได้ถูกต้อง
```

## 🔹 Reflective Process Ownership

```text
มีการบันทึกขั้นตอนการพัฒนา ปัญหา และวิธีแก้ใน LEARNINGLOG
```

---

# 👥 Group Assessments

```md
Group Score: 9/10
เหตุผล: ระบบครบ มี logic ชัดเจน และพัฒนาเป็นขั้นตอน

Individual Score: 9/10
เหตุผล: มีส่วนร่วมทั้ง coding, design และ debugging
```

---

# 🧪 Example Output

```text
Player HP: 100 | Enemy HP: 100
Choose action:
1 = Attack
2 = Defend
3 = Heal

You attack and deal 15 damage!
Enemy HP: 85
```

---
