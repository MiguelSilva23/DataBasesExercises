# Exercise # 3 - Check Referential Integrity

> **Ensure "Exercise # 2 - Add Foreign Key reference" is completed.**

***Hint:*** The "Projects" table shall exist.

> **Insert the following records in Projects table**

|name|manager_id|
|---|---|
|Trainings|2|
|Marketing|1|
|Sales|5|
|Reserch & Development|2|

***Hint:*** Use INSERT INTO command.

> **Verify that four records are added to the Projects table**

***Hint:*** Use SELECT * FROM command.

> **Try to Insert the following records in Projects table**

|name|manager_id|
|---|---|
|Accounts|8|

***Hint:*** Use SELECT * FROM command.

> **Verify that it reports error as follows**

```
SQL Error [23503]: ERROR: insert or update on table "projects" violates foreign key constraint "fk_manager_id"
  Detail: Key (manager_id)=(8) is not present in table "employees".
```


====================================== Exercise =============================================

> **Insert the following records in Projects table**

```
insert into projects 
(
name,manager_id 
)
values
('Trainings',2),
('Marketing',1),
('Sales',5),
('Research & Development',2);
```

> **Verify that four records are added to the Projects table**

![Screenshote](VerifyProjects.png)

> **Try to Insert the following records in Projects table**

`insert into projects ('Accounts',8);`
