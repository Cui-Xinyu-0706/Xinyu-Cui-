# Course Registration System

This project is a hands-on implementation of an Object-Oriented Programming (OOP) system for managing courses and student registrations. The system allows students to enroll in courses, drop courses, and view their registered courses, while administrators can manage courses and students and calculate students' GPA.

## Table of Contents

- [Overview](#overview)
- [Classes and Methods](#classes-and-methods)
  - [Course Class](#course-class)
  - [Student Class](#student-class)
  - [Registration Class](#registration-class)
- [Requirements](#requirements)
- [Usage](#usage)
- [Homework](#homework)
- [License](#license)

## Overview

This project consists of three main classes:

1. **Course**: Represents a course with a name, description, and list of enrolled students.
2. **Student**: Represents a student with details like name, ID, address, enrolled courses, and grades.
3. **Registration**: Manages the overall enrollment process, allowing students to enroll in and drop courses.

### Key Features

- Enroll and drop students from courses.
- Enroll students in specific courses and display all registered courses.
- Show all courses and all students in the system.
- Calculate GPA for students based on course grades.

## Classes and Methods

### Course Class

The `Course` class represents each course offered in the system.

#### Attributes

- `name`: The course name.
- `description`: A brief description of the course.
- `enrolled_students`: A list of students enrolled in the course.

#### Methods

- `add_student(student)`: Adds a student to the course.
- `remove_student(student)`: Removes a student from the course.
- `show_students()`: Lists all students currently enrolled in the course.

### Student Class

The `Student` class represents each student in the system.

#### Attributes

- `name`: The student's name.
- `id_number`: The student's unique ID.
- `address`: The student's address.
- `enrolled_courses`: A dictionary where each key is a course object and each value is the grade (if any) the student received in that course.

#### Methods

- `enroll_in_course(course)`: Enrolls the student in a specific course.
- `drop_course(course)`: Removes the student from a specific course.
- `show_courses()`: Displays all courses the student is currently enrolled in.

### Registration Class

The `Registration` class manages the central system for students and courses.

#### Attributes

- `students`: A list of all students in the system.
- `courses`: A list of all courses available.

#### Methods

- `enroll_student_in_course(student, course)`: Adds a student to a course.
- `drop_student_from_course(student, course)`: Removes a student from a course.
- `show_all_courses()`: Lists all available courses.
- `show_all_students()`: Lists all registered students.

## Requirements

- Python 3.x
- A terminal or code editor to run the Python script.

## Usage

1. Create instances of `Course`, `Student`, and `Registration`.
2. Use methods from each class to manage courses, students, and enrollments.
3. Example:
   ```python
   # Creating instances
   course = Course(name="Math 101", description="Basic Mathematics")
   student = Student(name="Alice", id_number="S1001", address="123 Main St")
   registration_system = Registration()

   # Adding course and student to the registration system
   registration_system.courses.append(course)
   registration_system.students.append(student)

   # Enrolling student in course
   registration_system.enroll_student_in_course(student, course)

   # Viewing enrolled students and courses
   course.show_students()
   student.show_courses()

