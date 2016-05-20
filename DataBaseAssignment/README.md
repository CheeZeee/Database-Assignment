##A UNIVERSITY EXAMINATION DATABASE
####This lists the queries contained in the tables

######1. Create a table to store Examination Results
```sql
CREATE TABLE Exam_results (Exam_id SMALLINT, Semester_id SMALLINT, Student_id SMALLINT, Scores SMALLINT, Grades VARCHAR(5), Result_category VARCHAR(25))
```
######2. Add record to Student Information table
```sql
INSERT INTO Students (Student_id, First_name , Middle_name, Last_name, Course, Current_level) VALUES ('PHY/2009/053', 'Chika', 'Chikwendu', 'Onwueyi', 'Engineering Physics', '400')
```
######3. Get particular information of a certain student
```sql
SELECT * FROM Students WHERE Student_id = <student_id>
```
######4. Update a record in the database
```sql
UPDATE Semester_records SET NoOfTimes_absent = '19' WHERE Student_id = <student_id>
```
######5. Get the number of times a student was present in a particular semester
```sql
SELECT * FROM Semester_records WHERE Student_id = <student_id> AND Semester_id = <semester_id> AND NoOfTimes_present = <times_present>
```
######6. Get the date that a particular exam was taken
```sql
SELECT * FROM Exams WHERE Exam_id = <exam_id> AND Exam_date = <exam_date>
```
######7. Get the result of a student for a particular semester
```sql
SELECT * FROM Exam_Results WHERE Semester_id = <semester_id> AND Student_id = <student_id> AND Scores = <score> AND Grades = <grade>
```
