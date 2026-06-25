🎓 Student Management System using SQL Joins

📌 Project Overview

This project demonstrates the implementation of various SQL join operations using a Student Management Database. The database contains information about students, departments, courses, grades, and mentor relationships.

The primary objective of this project is to understand and apply different types of SQL joins and relational database concepts.

---

Technologies Used

* MySQL
* SQL
* Relational Database Concepts

---

Database Tables

### STUDENT

Stores student information including marks, department, and mentor details.

### DEPARTMENT

Contains department information.

COURSE

Stores available courses.

### GRADE

Stores grade ranges and classifications.

---

SQL Concepts Implemented

* CROSS JOIN
* LEFT JOIN
* RIGHT JOIN
* FULL OUTER JOIN (using UNION)
* SELF JOIN
* INNER JOIN
* Range Join
* UNION
* BETWEEN Operator
* DISTINCT
* WHERE Clause

---

✨ Features

Student and department relationships
Student-mentor relationships
Grade calculation using marks ranges
Cross join examples
Full outer join implementation
Self join queries
Grade analysis queries

---

Sample Queries

Self Join (Student and Mentor)

```sql
SELECT
    S.StudentName AS Student,
    M.StudentName AS Mentor
FROM STUDENT S
JOIN STUDENT M
ON S.MentorID = M.StudentID;
```

Grade Assignment

```sql
SELECT S.StudentName, G.Grade
FROM STUDENT S
JOIN GRADE G
ON S.Marks BETWEEN G.MinMarks AND G.MaxMarks;
```

---

Learning Outcomes

* Understanding SQL join operations
* Database relationship concepts
* Query writing and optimization
* Self joins and hierarchical relationships
* Data analysis using SQL

---

Future Improvements

* Add stored procedures
* Create views
* Add triggers
* Build a front-end interface
* Develop a dashboard using Power BI

---

Author

**Ammar Ahmad**
BS Computer Science Student
Aspiring Business Analyst | Data Analyst | SQL Enthusiast
