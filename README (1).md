# Student Management System

A simple console-based **Student Management System** built in Java. It lets a user add student records and view all stored students, using an in-memory list for storage during the program's runtime.

## Features

- **Add Student** — capture ID, Name, and Age for a new student
- **View Students** — display all currently stored student records
- **Exit** — safely close the program and the input scanner

## Tech Stack

- **Language:** Java (JDK 8+)
- **Core Classes:** `java.util.ArrayList`, `java.util.Scanner`
- **Paradigm:** Object-Oriented Programming (OOP)

## Project Structure

```
Main.java        # Contains the Student class and the Main class with program logic
```

## Class Overview

### `Student`
Represents a single student record.

| Field  | Type   | Description          |
|--------|--------|-----------------------|
| id     | int    | Unique student ID     |
| name   | String | Student's name        |
| age    | int    | Student's age         |

Method: `display()` — prints the student's details in a formatted line.

### `Main`
Runs the menu-driven console program in a loop:

1. Add Student
2. View Students
3. Exit

Student records are stored in an `ArrayList<Student>` for the duration of the session (not persisted to a file or database).

## How to Compile and Run

```bash
javac Main.java
java Main
```

## Sample Usage

```
===== Student Management System =====
1. Add Student
2. View Students
3. Exit
Enter choice: 1
Enter ID: 101
Enter Name: John Doe
Enter Age: 20
Student Added Successfully!
```

## Possible Enhancements

- Add **Update** and **Delete** student options
- Persist data to a file or database (so records survive program restarts)
- Add input validation (e.g., reject negative IDs/ages, handle non-numeric input gracefully)
- Add search functionality by ID or Name
- Migrate to a GUI (JavaFX/Swing) or a web interface

## Author

Student Management System — Java Console Application
