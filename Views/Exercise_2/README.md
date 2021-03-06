# Exercise # 2 - Create Project Managers View

> **Ensure "Exercise # 1 - List Project Managers" from "Views" section is completed**

> **Define a query to List Project records from Projects table with name of the Manager picked from Employees table. Consider the following conditions/fields.**

- Use "Project ID" as label of Projects.project_id field 
- Use "Project Name" as label of Projects.name field 
- Concatanate Employees.fname and Employees.lname with a space (' ') in the middle and label it as "Manager Name"
- Use "Manager ID" as label of Employees.emp_id field 

***Hint:*** Use SELECT command on Projects with LEFT JOIN on Employees using foreign key reference.

> **Define a view named "Project Managers" using the above created query**

***Hint:*** Use CREATE VIEW command.

> **Verify that the view is created successfully**

***Hint:*** Use SELECT * FROM command on "Project Managers" view. It should list four records.


===================================== Exercise =======================================

> **Define a view named "Project Managers" using the above created query**

```
create view Project_Managers as 
select 
projects.project_id as Project_ID,
projects."name" as Project_Name,
concat(employees.fname, ' ',employees.lname) as Manager_Name,
employees.emp_id as Manager_ID
from projects
left join employees on  projects.manager_id = employees.emp_id;
```

> **Verify that the view is created successfully**

`select * from Project_Managers;`

![Screenshot](View.png)
