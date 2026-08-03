# ⚔️ Turn-Based Battle Game (Python CLI)

---

## 📌 Project Description

โปรเจกต์นี้เป็นเกมต่อสู้แบบ Turn-Based (Text-based CLI) ที่ผู้เล่นสามารถเลือกคำสั่งในแต่ละเทิร์น เช่น Attack, Defend และ Heal เพื่อต่อสู้กับศัตรู (Enemy) โดยระบบจะทำงานจนกว่าฝ่ายใดฝ่ายหนึ่งจะมี HP = 0

---

## 🎯 Features

* ⚔️ Attack → สุ่ม damage
* 🍀 Punch of Luck → สุ่มดาเมจ
* 🛡️ Defend → ลด damage ที่ได้รับ
* 💊 Heal → ฟื้นฟู HP (ไม่เกิน max)
* 🔁 Loop gameplay → เล่นต่อเนื่อง
* ❗ Input Validation → กัน input ผิด

---

## ⚙️ How to Run

```bash
run in the last code cell
in code cell have main()  
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
- [x] สร้างระบบ attack
- [x] สร้างระบบ defend
- [x] สร้างระบบ heal
- [x] เพิ่ม input validation
- [x] เพิ่ม enemy AI
- [x] ปรับ UX (input เป็นตัวเลข)
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
--- Turn 1 ---
❤️ Player HP: 100 | 👾 Enemy HP: 100

Choose action:
[1] Attack ⚔️
[2] Punch of Luck 🍀
[3] Heal 💊
[4] Defend 🛡️

⚔️ You used punchofluck and deal 46 damage!
👾 Enemy attacks and deals 27 damage!
```

---
