# 🎓 Student Grade Tracker (OOP System)

A comprehensive Python application designed to manage and track student academic performance. This project is built using **Object-Oriented Programming (OOP)** principles to ensure clean, modular, and maintainable code.

## 🚀 Key Features
- **Student Management:** Register students with unique IDs (supports both manual entry and auto-generation).
- **Academic Tracking:** Manage multiple subjects for each student dynamically.
- **Grade Analysis:** Add multiple grades per subject with built-in validation (0-100).
- **GPA Calculation:** Automatically calculates averages for individual subjects and an overall GPA for the student.
- **Data Persistence:** Save your data to a local text file (`student_data.txt`) and reload it automatically when restarting the app.
- **Search Functionality:** Quickly find student records using either their **Name** or **ID**.

## 🏗️ System Architecture (OOP Design)
The project is structured into three main classes that work together:

### 1. `Subject` Class
Represents an individual course or subject.
- **Attributes:** Name, Grades list.
- **Methods:** `add_grade()`, `get_average()`.

### 2. `Student` Class
Represents a student profile within the system.
- **Attributes:** Name, Unique ID, Subjects dictionary.
- **Methods:** `add_subject()`, `add_grade()`, `get_average()` (Overall GPA).

### 3. `GradeTracker` Class (The Controller)
The core engine that manages the entire database and user interface.
- **Functions:** Handles CRUD operations for students, facilitates file I/O (Save/Load), and manages the search logic.

## 🛠️ Tech Stack
- **Language:** Python 3.x.
- **Key Concepts:** Classes & Objects, Encapsulation, File Handling, Exception Handling.

## 📋 Prerequisites
- Python installed on your machine.
- No external libraries required (uses standard Python libraries).

## 🔧 Installation & Usage
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/tahamo22/AI-mock-interview-practice-and-feedback.git](https://github.com/tahamo22/AI-mock-interview-practice-and-feedback.git)

```

2. **Navigate to the project folder and run:**
```bash
python oop_project(grade_tracker)_.py

```


3. **Menu Options:**
* **1:** Add a new student.
* **2:** Add a subject and its grade.
* **3/4:** View specific or all student reports.
* **5:** Save data and exit.



## 💾 Data Example

Data is stored in `student_data.txt` using a custom structured format for reliability:

```text
STUDENT:123:taha
SUBJECT:math:80.0,50.0
SUBJECT:english:70.0
END_STUDENT

```

## 📊 Sample Output

```text
===== Student Grade Tracker =====
1. Add Student
...
Enter your choice: 3
Enter student name or ID: 123

Student ID: 123 | Name: taha
  math: Grades [80.0, 50.0], Average: 65.00
  english: Grades [70.0], Average: 70.00
Overall Average: 67.50

```

---

*This project was developed as part of a Python OOP learning journey.*

