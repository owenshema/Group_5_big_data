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
   6. 26253 - Shema Owen

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

   ### Result of Code After Running 
<img width="1294" height="169" alt="Image" src="https://github.com/user-attachments/assets/1ead2ff9-7a54-464a-941c-6a1fa0abcbcf" />

  ### Question II: Check Palindrome Function
**Objective**: Write a function that asks the user to input a string and checks if the string is a palindrome (reads the same forwards and backwards). Print "Yes, it is palindrome" or "No, it is not a palindrome".

**Solution**: The following Python code implements the palindrome check:

```python
def is_palindrome(text):
    text = text.lower()  # Make it case-insensitive
    return text == text[::-1]

def check_palindrome():
    word = input("Enter a string: ")
    if is_palindrome(word):
        print("Yes, it is a palindrome")
    else:
        print("No, it is not a palindrome")

# Run the function
check_palindrome()
```

- **How it Works**: The system converts the input to lowercase for case-insensitive comparison and checks if it reads the same forwards and backwards.

   ### Result of Code After Running 
<img width="1356" height="586" alt="Image" src="https://github.com/user-attachments/assets/204b87c0-4063-4b2d-9cb2-a6879e497cfd" />
