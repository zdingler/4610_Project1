# MIST4610-Project1-Group9

## Team Name:
61608 Group 9

## Team Members:
1. Zack Dingler - [@zdingler](https://www.github.com/zdingler)
2. Mingyang (Amanda) Li - [@MingyangLiAmanda](https://www.github.com/MingyangLiAmanda)
3. Andrew Toeppner - [@AToeppner](https://www.github.com/AToeppner)
4. Zuhair Baig - [@ZuhairBaig0](https://www.github.com/ZuhairBaig0)
5. Koty Hall - [@kah02358](https://www.github.com/kah02358)

## Problem Description:
Our University Course Management System is a database designed to help efficiently manage student enrollment, professor assignments, academic performance, and department administration in a university setting. The system is designed to give a structured way to store, retrieve, and analyze key academic data to ensure smooth operations for students, faculty, and administration. The database's primary function is to provide an optimized query system to analyze enrollments, GPA trends, professor workloads, and departmental performance.

## Data Model:
The data model displays important entities that go into student enrollment as well as professor evaluations. The Student entity holds relevant student information that is connected to the transcript entity to track performance and also links to the Courses entity to track enrollment. To keep professor workloads balanced there is a Professor entity that links to the Courses entity to track which professors teach what classes. The Professors entity also links to the Departments entity to track budgets and also overall department performance. 

The Students entity is one of the core elements of the data model. It stores the student's name, academic year, major, hometown, and whether they have graduated or not. Students have a one to one relationship with the Transcript entity as a student has one transcript (at this university) and one transcript shows only a single student's data. Students also have a many to many relationship with Courses as a student can enroll in many courses, and a course can have many students enrolled.

The Professors entity is the second main component of the data model. It holds the professor's salary, name, office hours, contact email, position, and research area. Professors have a one to many relationship with the Courses entity as one professor can teach a number of courses, and one course is taught by a single professor. Professors also have a many to one relationship with the Departments entity. A department can have numerous professors and a professor teaches under one department. 

The Courses entity stores the course name and credit hours. The Departments entity stores the department name, building name, head of department, and also the department budget. These serve as data to provide order and also as attributes to look at to evaluate performance. 

![Project1_UPDATED_MODEL](https://github.com/user-attachments/assets/0237dcbf-bdff-47a7-aa76-0d6b77e182b6)

## Data Dictionary:

![Students](https://github.com/user-attachments/assets/8a0a4a6d-be6b-4848-9ad8-f6abe9be868c)

![Professors](https://github.com/user-attachments/assets/7d1bc825-280e-402b-89e2-5f2ef9b7b9db)

![Courses](https://github.com/user-attachments/assets/fec96d9e-ae12-4b2a-a8a2-c9a4b476656a)

![Departments](https://github.com/user-attachments/assets/242113fd-015c-4e61-829e-67a9fe058868)

![Transcript](https://github.com/user-attachments/assets/f27cb2f9-1fa9-4796-bcc2-ee8524c57783)

![Enrollment](https://github.com/user-attachments/assets/2f671857-2a29-4005-95c0-b889e161bdda)

## Queries:

1. Query 1 displays all of the courses currently offered at the University. The results are ordered by department in descending order.

![Query1](https://github.com/user-attachments/assets/348d92c2-bdb5-421a-bcaa-cd67899f01e4)

University administrators are able to view what courses are offered and also what department they are in. This can be helpful to administrators looking to add a class to a professor's workload if that professor has the ability to take on another course. It also lets administrators see if a professor may be overworked with too many courses.

2. Query 2 shows all of the students currently enrolled in a specific class. The results are ordered by overall GPA in descending order.

![Query 2](https://github.com/user-attachments/assets/d4745d0b-d6c7-4541-b5be-05357b47f9ac)

This query would be helpful to administrators seeking to make sure there are not any classes with too many or too little students. If one class has a large number of students administrators may look to add another section of the course. It also allows professors to see students in their class that may be eligible for the honors section of that course by viewing their GPA.

3. Query 3 shows how many active students each professor is currently teaching. The results are ordered by the number of counted students in descending order.

![Query3](https://github.com/user-attachments/assets/55629458-8803-4572-920f-a1172302ae1e)

This query would be helpful to professors and administrators seeking to balance workloads between professors if possible. This also serves as a factor to look at with professor evaluation. Professors may have more students in their class as students may view that professor as being "better" than others. This also helps administrators identify if certain majors are more popular than others which would allow them to make changes so that majors and courses show more even distributions. 

4. Query 4 shows the average salary of a professor. The results are grouped by the departments the professors are in and are ordered by the average salary in descending order.

![Query4](https://github.com/user-attachments/assets/e60eab41-6f17-4474-86ee-1ef82ca664bc)

This query would be helpful to department heads looking to budget for the year. If paying salaries takes up a lot of the department's budget they would want to then evaluate professors to ensure the money is being used wisely. They may also want to change salaries if the department is looking to allocate money to do building renovations or give a better learning experience by providing more resources.

5.  Query 5 lists all of the students that have a GPA higher than the overall GPA of all of the students at the university.

![Query5](https://github.com/user-attachments/assets/91672318-8425-42df-89bc-6c701552e018)

This query would be helpful to administrators looking to identify students that are excelling in their academics. Students with a GPA higher than the school average are eligible to receive an award. Professors may also want to reach out to these excelling students and ask if they would be willing to offer help to those that may be struggling. These students that are performing well may also be eligible to be hired as a TA.

6. Query 6 lists the overall GPA of students that have graduated from the university.

![Query6](https://github.com/user-attachments/assets/2132ae85-bbfa-4a7f-86fb-19c450688798)

This query would be important to administrators and department heads that want to compare current students' academic performance to those that have graduated. It is important for administrators to track academic performance each year to ensure the university's prestige academic reputation. If students' performance starts to decline then administrators may look to make some changes within the curriculum.

7. Query 7 lists all active students and their current overall GPA as well as all of the courses they are currently taking.

![Query7](https://github.com/user-attachments/assets/fb5a099a-a4df-487a-86ba-cc0754a73b87)

This query would be very important to academic advisors looking to evaluate a student's current standing in school. Advisors will want to ensure that students are not in poor academic standing with their GPA, and also would want to make sure that students are currently enrolled in courses that they need to be taking in order to graduate.

8. Query 8 lists the 5 active students that have the highest GPAs.

![Query8](https://github.com/user-attachments/assets/73ae5681-1d3e-4846-938e-cc8b5418f36d)

This query would be vital to administrators that are in charge of finding the valedictorian and salutatorian for the current academic year. 

9. Query 9 lists all of the active students that have 12 or more credit hours of courses this semester.

![Query9](https://github.com/user-attachments/assets/2e9dacdf-c0d7-4092-933e-69d9e67569d2)

This course is important for administrators and the financial aid department. Identifying full time students (those with at least 12 credit hours) is a key factor in the amount of financial aid given to a student. Administrators will also use this to contact students that have more than the maximum number of credit hours one can take.

10. Query 10 finds students that are not enrolled in any courses

![Query10](https://github.com/user-attachments/assets/3338e069-e4c6-4a96-aa1a-e22e201fd4ba)

This query helps the university identify students that may no longer want to be enrolled at the university whether it is because they would like to transfer or drop out. The school will want to find these students and contact them to learn the reason they are not enrolled in any classes. They may offer academic or non academic counseling if the student is struggling due to external factors. Taking care of students is a university's primary goal, and this query helps identify those that may be struggling.

## Database Information:

![Database_info](https://github.com/user-attachments/assets/3faa9d0c-16a3-4ff4-83cb-6d8af6a0d89c)


Name of the database: ha_group9
All queries are bookmarked through stored procedures and can be called using this format: CALL TP_Qx(); where 'x' is the query number.
