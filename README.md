# Lab 1 - Conceptual Modeling using Draw.io

## Dominique Cheris

Lab 1 Diagram.drawio FINAL.png

<br >
# Entity Descriptions

- **STUDENT** – A student is a member of the school who attends. A student will consist of ID, name and address.
- **INSTRUCTOR** – An instructor is a part of the teaching staff. An instructor will consist of a number, name and faculty group.
- **COURSE** – A course is a class offered at school. A course consists of a name and number and ID.
- **SECTION** – A section is a subset of a course offering. A section consists of a number.
- **PROFESSOR** – a professor is a member of the school’s faculty. A professor will consist of an ID, name and faculty group.
- **SEAT** – A seat is a course space reservation for students. A seat consists of a number and position.
- **COURSE SCHEDULE** - A course schedule is a list of a student's enrolled courses. A course schedule will consist of a schedule ID, student ID, student name, course name, and section number.

<!---
  # Relationships

- A **STUDENT** <ins>takes</ins> zero or more a **COURSE**, more than one **COURSE** can be taken by many **STUDENT**
- A **STUDENT** <ins>fills</ins> a **SEAT**
- An **INSTRUCTOR** <ins>teaches</ins> a **COURSE**, each **COURSE** can be <ins>taught</ins> by many **INSTRUCTOR**
- A **COURSE** <ins>has</ins> a **SECTION**
- **SECTION** – 
- A **PROFESSOR** <ins>teaches</ins> a **COURSE**, each **COURSE** can be <ins>taught</ins> by many **PROFESSOR**
- **SEAT**
--->



# Cardinality
- A **STUDENT** can <ins>take</ins> zero or more **COURSES**, a **COURSE** can be <ins>taken</ins> by zero or more **STUDENTS**

- A **SEAT** can be <ins>filled</ins> by only one **STUDENT**, a **STUDENT** can only <ins>fill</ins> one **SEAT**

- A **PROFESSOR** can <ins>teach</ins> zero or more **SECTION**, each **SECTION** can be <ins>taught</ins> by one and only one **PROFESSOR**

- A **COURSE** can be <ins>attributed</ins> one to many **SECTION**, a **SECTION** can be <ins>attributed</ins> to one or many **COURSE**

- An **INSTRUCTOR** can <ins>teach</ins> zero or more **COURSE**, a **COURSE** can be <ins>taught</ins> by one or many **INSTRUCTOR**

- A **COURSE** can be <ins>contained</ins> on zero or more **COURSE LIST**, each **COURSE LIST** can <ins>contain</ins> zero or more **COURSE**

- A **SECTION** can be <ins>contained</ins> on zero or more **COURSE SCHEDULE**, each **COURSE SCHEDULE** can <ins>contain</ins> zero or more **SECTION**

- A **STUDENT** <ins>has</ins>  zero or more **COURSE SCHEDULE**, each **COURSE SCHEDULE** can <ins>have</ins> one and only one **STUDENT**


# Assumptions

1.	Can a student exist without taking a course? **YES**
2.	Would there/could there be a Boolean attribute for online/in-class seats? **YES**
3.	Are there instances where instructors and professors teach the same course and section? **YES**


## Lab Resources
- [Mark-down Syntax Cheat Sheet](https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf)
- [Make a ReadMe file Web-based Editor](https://www.makeareadme.com/)
- [Draw.io Web-based diagramming tool](https://app.diagrams.net/)
- [Creating Entity Relationship Diagrams using Draw.io](https://www.youtube.com/watch?v=lAtCySGDD48)