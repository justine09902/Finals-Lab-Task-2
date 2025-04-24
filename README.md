# Finals-Lab-Task-2

# 1. Create the student table:

Define username as a VARCHAR(50)
Set username as the Primary Key

# 2. Create the assignment table:

Define shortname as a VARCHAR(50) and set it as the Primary Key
Define due_date as a DATE NOT NULL
Define url as a VARCHAR(255), which can be null

# 3. Create the submission table:

Define username and shortname both as VARCHAR(50)
Define version as an INT
Define submit_date as a DATE NOT NULL
Define data as TEXT
Set a composite primary key of (username, shortname, version)
Add foreign keys referencing the student and assignment tables

Table Relationships
# 1. student table
Primary Key: username
Relationships:
One-to-Many with submission: One student (username) can have many submissions.

# 2. assignment table
Primary Key: shortname
Relationships:
One-to-Many with submission: One assignment (shortname) can have many submissions.

# 3. submission table

Composite Primary Key: (username, shortname, version)
Relationships:
Many-to-One with student: Each submission belongs to one student.
Many-to-One with assignment: Each submission is for one assignment.
This models a Many-to-Many relationship between students and assignments, with version tracking multiple submissions.

## Screenshots of the Process
 - Query Statements:
 - Student Table
 - 
![21](https://github.com/user-attachments/assets/dd22a4cb-064a-465f-8ff9-1ca539ad4e40)

 - Assignment Table
 - 
![22](https://github.com/user-attachments/assets/09358fc3-b6b5-4299-aec7-1a9b46f93b68)

 - Submission Table
 - 
![23](https://github.com/user-attachments/assets/7040a2ab-a8e8-4151-9c21-53d1bbc0735f)

 - Table Structures

 - Student Table
 - 
![24](https://github.com/user-attachments/assets/c2b13038-261e-449b-a323-180afa1f4590)

 - Assignment Table
 - 
![25](https://github.com/user-attachments/assets/95c312b6-e032-4a49-bd67-045076901ee3)

 - Submission Table
 - 
![26](https://github.com/user-attachments/assets/6cf1809e-2534-470a-b48f-eef1bb7895ca)

  - ER Diagram
  - 
 ![27](https://github.com/user-attachments/assets/f85186e0-55e6-4544-8d35-62d716ddecd8)
