# Exercise # 1 - Rebuild Employees Table

> **Ensure "Employees" table exist.**

> **Remove the Employees table**

***Hint:*** Use DROP TABLE command.

> **Create "Employees" table with the following details**
 
 | Column Name | Description | Data Type | Is Unique? | Is Nullable?|
 |:--- | :--- | :---: | --- | --- |
 |fname|First Name|Character (30)|No|No|
 |lname|Last Name|Character (30)|No|No|
 |email|Email ID|Character (50)|Yes|No|
 |contact|Phone Number|Integer (15)|No|Yes|

***Hint:*** use CREATE TABLE command.

> **Insert the following records in Employees table**

|fname|lname|email|
|---|---|---|
|Adam|Falon|adam.falon@dci.com|
|Mary|Gold|mary.gold@dci.com|
|Adam|Currie|adam.currie@dci.com|
|Bryan|Jhonson|bryan.Jhonson@dci.com|
|Prasad|Ritesh|prasad.ritesh@dci.com|
|Mary|Jhonson|mary.jhonson@dci.com|

***Hint:*** Use INSERT INTO command.

> **Verify that six records are added to the Employees table**

***Hint:*** Use SELECT * FROM command.


============================== Exercise =========================

> **Remove the Employees table**

`DROP TABLE employees; `

> **Create "Employees" table with the following details**

```
create table Employees
(
fname varchar(30) not NULL, -- First Name
lname varchar(30) not NULL, -- Last Name
email varchar(50) not NULL unique, -- Email ID
contact numeric(15,0) -- Phone Number
);
```
