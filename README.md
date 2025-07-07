# Group_5_big_data
Integrating basic python 
# Student Management System 📚
## Overview 🌟
This project addresses solutions to practical programming challenges posed in the "Introduction to Big Data Analytics" course (INSY 841J). The course aims to equip students with foundational skills in handling and analyzing large datasets using Python, focusing on data input, processing, and output techniques. The questions explored here—building a Student Management System and checking palindromes—serve to enhance problem-solving abilities, reinforce functional programming concepts, and prepare students for real-world data management tasks.

### Project Details 📋
- **Total Marks**: 10 points
### 👥Team Members:
   1. 25711- Tuyumvire Schiphtan  
   2. 27120 - Munezero Cindy
   3. 26600 - Mugeni Cynthia
   4. 26622 - Gatsinzi Ernest
   5. 26939 - Bucagu Chedrick Elisa
   6. 26953 - Shema Owen

## Questions and Solutions 💻
### Question I: Student Management System Function
**Objective**: Create a Student Management System that:
- Combines all concepts to build a function which:
  - Inputs student information (name, age, and grades for two or three courses)
  - Calculates the average of the marks
  - Stores and displays the student’s information along with their average grade
- Uses separate functions for each operation (input, calculation, display)

**Solution**: The following Python code implements the Student Management System:

```python
def calculate_average(grades):
    return sum(grades) / len(grades)

def input_student_info():
    name = input("Enter student name: ")
    age = int(input("Enter student age: "))
    marks = []
    
    for i in range(3):  # Assuming 3 subjects
        grade = float(input(f"Enter grade for subject {i+1}: "))
        marks.append(grade)
    return name, age, marks

def display_result(name, age, grades, average):
    print("\n--- Student Report ---")
    print("Name:", name)
    print("Age:", age)
    print("Grades:", grades)
    print("Average:", round(average, 2))

def student_management_system():
    name, age, grades = input_student_info()
    avg = calculate_average(grades)
    display_result(name, age, grades, avg)

# Run the program
student_management_system()
```

- **How it Works**: The system prompts the user to input a student's name, age, and grades for three subjects, calculates the average, and displays the results.

