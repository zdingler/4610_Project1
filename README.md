# MIST4610-Project1-Group9

## Team Name:
61608 Group 9

## Team Members:
1. Zack Dingler
2. Mingyang (Amanda) Li
3. Andrew Toeppner
4. Zuhair Baig
5. Koty Hall

## Problem Description:
Our University Course Management System is a database designed to helpo efficiently manage student enrollment, professor assignments, academic performance, and department administration in a university setting. The system is designed to give a structured way to store, retrieve, and analyze key academic data to ensure smooth operations for students, faculty, and administration. The database's primary function is to provide an optimized query system to analyze enrollments, GPA trends, professor workloads, and departmental performance.

## Data Model:
The data model displays important entities that go into student enrollment as well as professor evaluations. The Student entity holds relevant student information that is connected to the transcript entity to track performance and also links to the Courses entity to track enrollment. To keep professor workloads balanced there is a Professor entity that links to the Courses entity to track which professors teaches what classes. The Professors entity also links to the Departments entity to track budgets and also overall department performance. 

The Students entity is one of the core elements of the data model. It stores the student's name, academic year, major, hometown, and whether they have graduated or not. Students has a one to one relationship with the Transcript entity as a student has one transcript (at this university) and one transcript shows only a single student's data. Students also has a many to many relationship with Courses as a student can enroll in many courses, and a course can have many students enrolled.

The Professors entity is the second main component of the data model. It holds the professor's salary, name, office hours, contact email, position, and research area. Professors has a one to many relationship with the Courses entity as one professor can teach a number of courses, and one course is taught by a single professor. Professors also has a many to one relationship with the Departments entity. A department can have numerous professors and a professor teaches under one department. 

The Courses entity stores the course name and credit hours. The Departments entity stores the department name, building name, head of department, and also the department budget. These serve as data to provide order and also as attributes to look at to evaluate performance. 

![Project1_UPDATED_MODEL](https://github.com/user-attachments/assets/0237dcbf-bdff-47a7-aa76-0d6b77e182b6)
