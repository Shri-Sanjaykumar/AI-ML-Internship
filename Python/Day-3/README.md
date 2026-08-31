# Day 3 – Python Data Structures & File Handling

- **Date:** 31 August 2026
- **Training Day:** Day 3
- **Focus Area:** Python Data Structures (`list`, `tuple`, `dict`, `set`) and Flat-File Persistence (`with open`)

---

## 🎯 Overview & Objectives

The primary goal of Day 3 was to master Python's core data structures, understand their distinct properties (mutability, indexing, uniqueness, key-value mapping), and apply them alongside persistent file handling to build a console-based **Student Record Management System**.

---

## 🛠️ Concepts Breakdown: Where, Why & How Each is Used

```text
┌─────────────────────────────────────────────────────────────────────────┐
│                      STUDENT RECORD MANAGEMENT SYSTEM                   │
├─────────────────┬───────────────────┬───────────────────────────────────┤
│ Concept         │ Implementation    │ Why & How It Is Used              │
├─────────────────┼───────────────────┼───────────────────────────────────┤
│ 1. Tuple        │ SUBJECTS          │ Immutable fixed subjects tuple    │
│ 2. Set          │ registered_rolls  │ Fast O(1) duplicate prevention    │
│ 3. Dictionary   │ student_record    │ Structured key-value student data │
│ 4. List         │ students, marks   │ Ordered collection of all records │
│ 5. File I/O     │ with open(...)    │ Persistent read/append storage    │
└─────────────────┴───────────────────┴───────────────────────────────────┘
```

### 1. 🔹 Tuple (`tuple`) — Immutable Fixed Schema
- **Code Reference:** `SUBJECTS = ("Python", "Math", "Data Science")`
- **Why Used:** Tuples are ordered and **immutable** (cannot be altered after creation). Since curriculum subjects are constant, a tuple guarantees fixed integrity.

### 2. 🔹 Set (`set`) — Fast Unique Membership Checking
- **Code Reference:** `registered_rolls = set()`, `if roll_no in registered_rolls:`
- **Why Used:** Sets store **unique elements only** and provide $O(1)$ constant-time lookup, immediately preventing duplicate roll numbers.

### 3. 🔹 Dictionary (`dict`) — Key-Value Entity Modeling
- **Code Reference:** `student_record = {"roll_no": roll_no, "name": name, "marks": marks}`
- **Why Used:** Dictionaries represent real-world entities through structured **key-value pairs**, allowing intuitive attribute access (`record["name"]`, `record["marks"]`).

### 4. 🔹 List (`list`) — Dynamic Ordered Collections
- **Code Reference:** `students = []`, `marks = []`
- **Why Used:** Lists are **mutable and ordered**, making them ideal for growing collections of items.

### 5. 🔹 File Handling (`with open(...)`) — Persistent Storage
- **Code Reference:** `with open("students.txt", "r")` and `with open("students.txt", "a")`
- **Why Used:** Ensures all student data persists across sessions without memory leaks by utilizing Python's context manager.

---

## 📂 Files in This Directory

- [`student_record_management.py`](student_record_management.py) — Console-based Student Record Management System.
- [`students.txt`](students.txt) — Flat-file database storing student records.
- [`README.md`](README.md) — Technical documentation and concept mapping.

---

## 🚀 How to Run

Execute in your terminal:
```bash
python student_record_management.py
```
