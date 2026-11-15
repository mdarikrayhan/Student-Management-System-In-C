# Student Management System in C

A menu-driven Windows console program in C that keeps student records (ID, name, gender, and quiz, mid-term and final scores) in a file and works out totals, averages and rankings. It was a classwork mini project from March 2021, written during my B.Sc. in CSE at BAUET.

## Features

The main menu has ten options:

1. Add student records, several in a row.
2. Delete a record by student ID.
3. Update a record by student ID.
4. View all records with each student's total score (quiz + mid + final).
5. Show one student's scores, total and average (total ÷ 3).
6. Show the student or students with the highest total.
7. Show the student or students with the lowest total.
8. Find a student by ID.
9. Sort the records by total score, ascending or descending.
10. Exit.

Records are written as fixed-size binary structs to `record.txt` in the working directory, despite the `.txt` extension.

## Tech stack

C with the standard library, plus `conio.h` and `windows.h` for `getch()` and cursor positioning, so it builds and runs on Windows only.

## Getting started

On Windows with MinGW:

```
gcc "Student Management System.c" -o student-management.exe
student-management.exe
```

The code reads input with `gets()`, so expect compiler warnings. Add at least one record (option 1) first: until `record.txt` exists, the other options stop with "Error opening file".

## Project structure

```
Student Management System.c   the whole program
```

## Author

Md Arik Rayhan — [mdarikrayhan.com](https://mdarikrayhan.com)
