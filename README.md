[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-c66648af7eb3fe8bc4f294546bfd86ef473780cde1dea487d3c4ff354943c9ae.svg)](https://classroom.github.com/online_ide?assignment_repo_id=9264075&assignment_repo_type=AssignmentRepo)
# Lab 1 - Conceptual Modeling using Draw.io


## Lab Resources
- [Mark-down Syntax Cheat Sheet](https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf)
- [Make a ReadMe file Web-based Editor](https://www.makeareadme.com/)
- [Draw.io Web-based diagramming tool](https://app.diagrams.net/)
- [Creating Entity Relationship Diagrams using Draw.io](https://www.youtube.com/watch?v=lAtCySGDD48)


# Entity Descriptions

- **STUDENT** – A student is a member of the school who attends. A student will consist of ID, name and address.
- **INSTRUCTOR** – A instructor is a member of the school’s faculty. An instructor will consist of a number, name and faculty group.
- **COURSE** – A course is a class offered at school. A course consists of a name and numbers.
- **SECTION** – A section is a subset of a course. A section consists of a number.
- **PROFESSOR** – a professor is a member of the school’s faculty. A professor will consist of an ID, name and faculty group.
- **SEAT** – A seat is a option for students. A seat consists of a number and position.

# Relationships

- A **STUDENT** <ins>takes</ins> zero or more a **COURSE**, more than one **COURSE** can be taken by many **STUDENT**
- A **STUDENT** <ins>fills</ins> a **SEAT**
- An **INSTRUCTOR** <ins>teaches</ins> a **COURSE**, each **COURSE** can be <ins>taught</ins> by many **INSTRUCTOR**
- A **COURSE** <ins>has</ins> a **SECTION**
- **SECTION** – 
- A **PROFESSOR** <ins>teaches</ins> a **COURSE**, each **COURSE** can be <ins>taught</ins> by many **PROFESSOR**
- **SEAT**

# Assumptions

1.	Can a student exist without taking a course? Yes
2.	Would there/could there be a Boolean attribute for online/in-class seats? Yes
3.	Are there instances where instructors and professors teach the same course and section? Yes

# Cardinality
- SEAT can be occupied by at most one STUDENT. SEAT is singular in STUDENT fills SEAT
- Each STUDENT can take many COURSES. COURSES is plural in STUDENT takes COURSE
- Each INSTRUCTOR can teach many COURSES. COURSES is plural in INSTRUCTOR teaches COURSE
- Each PROFESSOR can teach many COURSES. COURSES is plural in PROFESSOR teaches COURSE
- Each COURSE can have many SECTIONS and each SECTION can have many COURSES. A COURSE has a SECTION is bi-directional.
- Each PROFESSOR can teach many SECTIONS. SECTIONS is plural in PROFESSOR teaches SECTION
