Table: departments
id
name
head_of_department
website
phone
email_address
Table: degrees (one to many -> departments)
id
department_id (FK)
name
description
period
Table: courses (one to many -> degree)
id
degree_id (FK)
name
description
Pivot: course_teacher
course_id (FK)
teacher_id (FK)
Table: teachers
id
name
lastname
office_number
mobile_number
Table: exams
id
course_id (FK)
date
hour
Pivot: exam_student
student_id
exam_id
vote
Table: students (one to many -> degrees)
id
degree_id
name
lastname
email
phone
enrolment_date
registration_number