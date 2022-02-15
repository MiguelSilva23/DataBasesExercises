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
