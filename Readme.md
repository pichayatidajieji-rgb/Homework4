# 📄 Text/CSV Viewer (C# Learning Project)

***
## ข้อมูลผู้พัฒนา (Student Information)
ชื่อ-นามสกุล: [น.ส.พิชญธิดา พ่วงพิศ]
รหัสนักศึกษา: [6810301016]
วิชา: การพัฒนาซอฟต์แวร์ (Homework 4)
สถานะการส่งงาน: 
  - พัฒนาโปรแกรม (Part A: Programming Tasks) เสร็จสมบูรณ์
  - บันทึกผลการทดสอบระบบ (Part B: Testing) ในไฟล์ `Basev100.xlsx` เรียบร้อยแล้ว



## สิ่งที่ได้ปรับปรุง
โปรแกรมเวอร์ชันนี้ได้อัปเกรดความสามารถเพิ่มเติมตามโจทย์กำหนด ดังนี้:
1. รองรับการเปิดอ่านและประมวลผลไฟล์มัลแวร์ Dataset ขนาดใหญ่ โดยการอ่านข้อมูลทีละบรรทัด เพื่อรองรับข้อมูลจำนวนมากและลดการใช้หน่วยความจำ
2. เพิ่มการระบุช่วงบรรทัดที่ต้องการดึงมาแสดงผล โดยกำหนดค่าเริ่มต้น (Start Line) และค่าสิ้นสุด (End Line) ได้อย่างแม่นยำ (ข้ามบรรทัดคอมเมนต์อัตโนมัติ)
3. เพิ่มระบบกรองข้อมูลเฉพาะประเภทนามสกุลไฟล์ที่ต้องการค้นหา (เช่น exe, doc, zip)
4. รองรับการทำงานร่วมกันระหว่างการระบุช่วงบรรทัด (m-n) และการกรองประเภทไฟล์พร้อมกันในการกดประมวลผลครั้งเดียว
5. มีระบบดักจับ Error กรณีผู้ใช้กรอกช่วงบรรทัดไม่ถูกต้อง (ค่า n น้อยกว่า m) โดยจะแจ้งเตือนผ่าน MessageBox เพื่อป้องกันการทำงานผิดพลาดของโปรแกรม

## วิธีการใช้งานโปรแกรม 
1. เปิดโปรเจกต์ด้วยโปรแกรม Visual Studio
2. กด Run โปรแกรม
3. กดปุ่ม Browse เพื่อเลือกไฟล์ข้อมูล (เช่น malware_500.csv)
4. ระบุช่วงบรรทัดที่ต้องการในช่อง Start Line (m) และ End Line (n)
5. ใส่คำค้นหาที่ต้องการกรอกในช่อง File Type Filter หรือปล่อยว่างก็ได้
6. กดปุ่ม Process เพื่อแสดงผลข้อมูลบนหน้าจอ


---


## 📌 Overview

This project is a **simple Text/CSV Viewer written in C#**.  
It is designed as a **learning project for students** to practice:

* Basic C# programming
* File I/O handling
* Working with CSV data
* Git and version control
* Open-source and community practices

## 🎯 Learning Objectives

By completing this project, students will learn:

### 💻 C# Fundamentals

* Reading text and CSV files
* String manipulation and parsing
* Basic UI or console output (depending on your version)
* Error handling and input validation

### 🗂️ Software Engineering Basics

* Project structure
* Code readability and maintainability
* Separation of concerns

### 🔧 Git & Version Control

* Initialize a Git repository
* Commit changes with meaningful messages
* Use branches (optional for advanced students)
* Collaborate using pull requests (if working in groups)

### 🌍 Open Source & Community Discipline

* Understanding open-source licenses (MIT License)
* Giving proper credit to data sources
* Writing clean documentation
* Respecting third-party Terms of Use

***

## 🧱 Project Structure

```
/TextCsvViewer
│
├── Program.cs
├── CsvViewer.cs
├── LICENSE
├── README.md
└── data/
    └── malware_500.csv
```

> Note: Some files such as `*.Designer.cs` and `*.resx` are auto-generated and should not be manually edited.

***

## ▶️ How to Run

1. Open the project in **Visual Studio** or compatible IDE
2. Build the solution
3. Run the program
4. Load a `.txt` or `.csv` file to view its contents

***

## Data Source

This project uses malware metadata from MalwareBazaar
(https://bazaar.abuse.ch/), operated by abuse.ch.

Terms of Use:
https://bazaar.abuse.ch/faq/#tos

### Modifications to Dataset

The original dataset has been modified for educational purposes:

- Only the first 500 records are included
- The header line has been adjusted:
  - From:
    # "first_seen_utc", ...
  - To:
    #HEADER: "first_seen_utc", ...

These changes are intended to simplify usage and improve clarity for students.

The original dataset structure and attribution remain unchanged where applicable.
``
***

## 📜 License

This project is licensed under the **MIT License**.

You are free to:

* Use
* Modify
* Distribute

As long as you include the original license notice.

See the `LICENSE` file for full details.

***

## ✅ Student Tasks

Students are encouraged to:

### Beginner

* Load and display a CSV file
* Format output neatly
* Handle missing or invalid data

### Intermediate

* Add search/filter functionality
* Highlight specific columns
* Support large file handling

### Advanced

* Build a GUI (WinForms or WPF)
* Implement sorting and column selection
* Improve performance and memory usage

***

## 🧪 Suggested Git Exercises

* Create your repository
* Commit your initial version
* Add new features step by step
* Write clear commit messages:
  * ✅ `Add CSV file reader`
  * ✅ `Fix parsing bug in column handling`
  * ❌ `fix stuff`

***

## 🤝 Contribution Guidelines (For Students)

* Write clean, readable code
* Add comments when necessary
* Respect original authors and data sources
* Do not remove license or attribution
* Follow project structure and naming conventions

***

## Contribution Policy (Current Stage)

This repository is provided for **learning and reference purposes only**.

At this stage of the course:

- Students should NOT submit Pull Requests
- Do NOT attempt to modify the original repository
- Work should be done in your own copy of the project

### Student Instructions

1. Clone or download this repository
2. Create your own repository
3. Practice and modify code independently

Future assignments may introduce collaboration and Pull Requests.
***

## ⚠️ Disclaimer

This project may use metadata related to malware samples for educational purposes only.

* Do **not** execute or download actual malware
* Use data responsibly
* Follow all applicable laws and policies

***
## ⚠️ Ethical Use and Dual-Use Awareness

This project uses data related to malware for **educational purposes only**.

Students must understand the concept of **dual-use technology**:

- Software and technical knowledge can be used for **both beneficial and harmful purposes**
- The same skills used to analyze malware can also be misused to create it

### Our Objective

This project is designed to:

- Introduce students to real-world data handling
- Build skills in software development and analysis
- Promote **ethical awareness in computing**

We emphasize that:

- Students are expected to act as **responsible software developers**
- The goal is to **understand and defend**, not to exploit
- This course does **not support or encourage malicious activities**

### Professional Responsibility

As future professionals, students should:

- Follow ethical and legal guidelines
- Respect data sources and licenses
- Use their knowledge to **protect systems and improve security**
- Contribute positively to the software community

> We aim to educate **ethical programmers**, not individuals who misuse technology.

***

## 👨‍🏫 Instructor

**Sarayut Chaisuriya**  
C# Instructor / Software Development Educator

***

## 💡 Final Note

This project is not just about coding—it is about becoming a **responsible software developer**:

* Write clean code
* Use proper tools
* Respect licenses
* Learn continuously

***
