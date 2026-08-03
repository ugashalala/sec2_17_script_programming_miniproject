# ⚔️ Turn-Based Battle Game

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
run code cell ตัวสุดท้ายเพื่อเป็นการรันเกม
แต่ในการ run ครั้งแรกควร run code cell ทั้งหมดที่มีก่อนเพื่อไม่ให้ตัวเกมเกิดการ error 
```

---

## Workflow

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

# Kanban Backlog & Run

## 🗂️ Backlog

```md
- [ ] เพิ่ม enemy AI
- [ ] เพิ่มระบบ item
- [ ] เพิ่ม character class
```

## 🚀 In Progress

```md
- [ ] ปรับปรุง balancing damage
- [ ] เพิ่ม test case
```

## ✅ Done

```md
- [x] ระบบ battle ทำงานครบ
- [x] สร้างระบบ attack
- [x] สร้างระบบ defend
- [x] สร้างระบบ heal
- [x] เพิ่ม input validation
- [x] ปรับ UX (input เป็นตัวเลข)
- [x] ระบบ loop เกม
- [x] ทดสอบการเล่นเกม
```

---

# Learning Outcomes

```md
- LO1: ใช้ dictionary ในการจัดการ action และ skill
- LO2: จัดการข้อมูล HP และ state ของผู้เล่น
- LO3: ใช้ while loop และ if/elif/else ควบคุมเกม
- LO4: มี input validation ป้องกัน error
```

---

# Group Grading Rubric

## 1. Achievement of Group Objectives (30%)

โครงงานสามารถสร้างเกม Turn-Based Battle ได้ตามเป้าหมายที่กำหนด
โดยมีระบบต่อสู้หลัก ได้แก่ Attack, Defend, Heal และ Enemy

## 2. Content Consistency and Work Standard (30%)

โครงสร้างโปรแกรมมีการแบ่งส่วนการทำงานชัดเจน
มีการใช้ Python fundamentals เช่น Dictionary, Loop, Conditional Statement

## 3. Quantity, Quality and Work Process (30%)

มีการพัฒนาโปรเจกต์เป็นลำดับขั้นตอนผ่าน Kanban Backlog
มีการบันทึกการเปลี่ยนแปลงผ่าน CHANGELOG
และมีการทดสอบระบบก่อนนำเสนอ

## 4. Overall Group Work (10%)

ติดต่อสมาชิกกลุ่มค่อนข้างยาก

---

# 👥 Group Assessments

```md
1. อัครพงษ์ ศรีโฉม 653380220-8 
self : 7/10
group : -/10


2. นายภาสุ สมมีย์ 683380435-0
self : -/10
group : -/10 

3. นายณัฐพัชร์ คงสวัสดิ์ 683380415-6
self : -/10
group : -/10
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
