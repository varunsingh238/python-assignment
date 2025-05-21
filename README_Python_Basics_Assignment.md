
# Assignment: Python Basics – Grade & File Handling

## 1. Grade Checker

**Description:**  
This program takes a score as input from the user and prints the grade based on predefined conditions using `if-else` statements.

**Code:**
```python
score = int(input("Enter the score: "))

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")
```

**Explanation:**  
Takes numeric input and uses if-elif-else conditions to determine the grade.

---

## 2. Student Grades using Dictionary

**Description:**  
This program manages student names and grades using a dictionary. It allows adding, updating, and viewing grades.

**Code:**
```python
students = {}

while True:
    print("\nOptions:")
    print("1. Add student")
    print("2. Update grade")
    print("3. Print all grades")
    print("4. Exit")
    
    choice = input("Enter your choice (1-4): ")

    if choice == "1":
        name = input("Enter student name: ")
        grade = input("Enter grade: ")
        students[name] = grade
        print("Student added.")
        
    elif choice == "2":
        name = input("Enter student name to update: ")
        if name in students:
            grade = input("Enter new grade: ")
            students[name] = grade
            print("Grade updated.")
        else:
            print("Student not found.")
            
    elif choice == "3":
        print("\nStudent Grades:")
        for name, grade in students.items():
            print(f"{name}: {grade}")
            
    elif choice == "4":
        break
    else:
        print("Invalid option. Try again.")
```

**Explanation:**  
Uses a dictionary to store and update student grades via a menu system.

---

## 3. Write to a File

**Description:**  
Creates a new file and writes content to it.

**Code:**
```python
with open("example.txt", "w") as file:
    file.write("Hello, this is a sample text written to the file.\n")
    file.write("This is the second line.")
print("File written successfully.")
```

**Explanation:**  
Uses 'with open' in write mode to safely write content to a file.

---

## 4. Read from a File

**Description:**  
Reads the contents of a file and displays them.

**Code:**
```python
with open("example.txt", "r") as file:
    content = file.read()
    print("File Content:\n")
    print(content)
```

**Explanation:**  
Opens the file in read mode and displays its content.

---

## Submission Instructions

- Take screenshots of each program running in your IDE or terminal.
- Paste the screenshots below each code section in this document (if using Word or Google Docs).
- Or upload your code and screenshots to GitHub and share the repository link.
