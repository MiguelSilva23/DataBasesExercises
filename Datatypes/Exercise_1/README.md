# Exercise # 1 - Add more fields to Employees

> **Ensure "Employees" table exist.**

***Hint:*** Use SELECT command.

> **Add more fields to "Employees" as follows**
 
 | Column Name | Description | Data Type | Is Unique? | Is Nullable?|
 |:--- | :--- | :---: | --- | --- |
 |emp_id|Employee ID|serial|Yes|No|
 |dob|Date of Birth|Date|No|Yes|
 |is_manager|Is a Manager|Boolean|No|Yes|

***Hint:*** use ALTER TABLE command with ADD COLUMN clause.

> **Verify that above columns are added to the Employees table**

***Hint:*** Use SELECT * FROM command.

> **Confirm that emp_id column in in each record has a unique (serial) value specified automatically**