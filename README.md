# SQL_Edubridge

-- First Creating examination table.Using the attributes enrollmentno,studentname,section,subjectid,andmarks. 

    CREATE TABLE examination (
    EnrollmentNo int PRIMARY KEY,
    StudentName varchar(200) ,
    Section varchar(5),
    SubjectId int(20),
    Marks int);

-- Here we are inserting values into the table

     INSERT INTO  examination VALUES (1, 'Tim', 'A',1,70);
     INSERT INTO  examination VALUES (2, 'Jim', 'A',2,75);
     INSERT INTO  examination VALUES (3, 'Kim', 'B',3,65);
     INSERT INTO  examination VALUES (4, 'Tom', 'B',4,77);
     INSERT INTO  examination VALUES (5, 'John','C',5,60);
     INSERT INTO  examination VALUES (6, 'Joe', 'C',1,82);
     INSERT INTO  examination VALUES (7, 'James', 'B',2,76);
     INSERT INTO  examination VALUES (8, 'Henry', 'C',5,68);
     INSERT INTO  examination VALUES (9, 'Matt', 'B',3,71);
     INSERT INTO  examination VALUES (10, 'Paul', 'A',4,79);

--Inorder to display values we are giving select command.

      SELECT * FROM examination;

--Inorder to identify which value is greater or equal to 75.

      SELECT Section,COUNT(Section) as
      No_of_candidates_greater_than_or_equal_to_75_marks
      FROM examination WHERE Marks>=75 GROUP BY Section;
 
 
