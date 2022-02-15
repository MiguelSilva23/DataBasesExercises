# Exercise # 2 - Add Foreign Key reference

> **Ensure "Employees" table exist.**

***Hint:*** Use SELECT command.

> **Define a Table named "Projects" as follows**

 | Column Name | Description | Data Type | Is Unique? | Is Nullable?|
 |:--- | :--- | :---: | --- | --- |
 |project_id|Project ID|serial|Yes|No|
 |name|Project Name|Character (50)|Yes|No|
 |manager_id|Manager ID|Integer|No|No|

> **Add A Foreign Key Constraint on "Projects" with "Manager ID - manager_id" field referring to "Employee ID - emp_id" field of "Employees"**
 
 ***Hint:*** use ALTER TABLE command with ADD CONSTRAINT clause.
 
 ==================================== Exercise =================================================
 
 > **Define a Table named "Projects" as follows**

```
create table Projects 
(
project_id SERIAL unique not null, -- Project ID
name varchar(50) unique not null, -- Project Name
manager_id int not null -- Manager ID
);
```

> **Add A Foreign Key Constraint on "Projects" with "Manager ID - manager_id" field referring to "Employee ID - emp_id" field of "Employees"**

`alter table projects add FOREIGN key (manager_id) references employees(emp_id);`
