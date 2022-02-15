# Exercise # 1 - List Project Managers

> **Ensure All exercises from "Primary Key and Foreign Key" section are completed**

***Hint:*** Use SELECT * FROM command on Projects table. It should list four records.

> **List Project records from Projects table with name of the Manager picked from Employees table. Consider the following conditions/fields.**

- Use "Project ID" as label of Projects.project_id field 
- Use "Project Name" as label of Projects.name field 
- Concatanate Employees.fname and Employees.lname with a space (' ') in the middle and label it as "Manager Name"
- Use "Manager ID" as label of Employees.emp_id field 

***Hint:*** Use SELECT command on Projects with LEFT JOIN on Employees using foreign key reference.

> **Verify that it displays the following result**

|Project ID|Project Name|Manager Name|Manager ID|
|---|---|---|---| 
|1|	Trainings|	Mary Gold|	2|
|2|	Marketing|	Adam Falon|	1|
|3|	Sales|	Prasad Ritesh|	5|
|4|	Reserch & Development|	Mary Gold|	2|
