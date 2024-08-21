# DataBase

This repository contains SQL scripts for managing an `employees` table. The table includes columns for name, role, salary, age, and phone number. Below are the details of the table structure and various SQL operations performed.

- ## To create table
```bash
CREATE TABLE "employee" (
	"id"	INTEGER UNIQUE,
	"name"	TEXT NOT NULL,
	"age"	INTEGER NOT NULL,
	"role"	TEXT NOT NULL,
	"address"	TEXT,
	"salary"	INTEGER NOT NULL,
	"phone"	INTEGER NOT NULL,
	PRIMARY KEY("id" AUTOINCREMENT)
)

)
```

- ## Data Insertion

Inserting data into the `employees` table:

```bash

INSERT INTO employee (name,age,salary,role,phone) VALUES ("sanju",20,20000,"employee",9846897456);
INSERT INTO employee (name,age,salary,role,phone) VALUES ("Rohan",22,20000,"employee",9946897456);
INSERT INTO employee (name,age,salary,role,phone) VALUES ("Sumit",24,20000,"ceo",9746897456);
INSERT INTO employee (name,age,salary,role,phone) VALUES ("Hiren",26,20000,"dev",9646897456);

```

### Selecting all data from the `employees` table:

```bash
SELECT * FROM employee;
```
### Selecting specific columns:

```bash
SELECT name From employee;
SELECT salary From employee;
```

### Filtering data based on conditions:

```bash

SELECT * FROM employee WHERE role = "employee";
SELECT * FROM employee WHERE name Like 'Ra%';
SELECT * FROM employee WHERE (age > 25 AND salary > 20000);

```
- ## Data Update

### Updating data in the `employees` table:

```bash

UPDATE employee SET salary = 20000 WHERE id = 7;
UPDATE employee SET Phone = 9726548975 WHERE id = 7;

```

- ## Data Delete

### Deleting data from the `employees` table:

```bash

DELETE FROM employee WHERE id = 8;
DELETE FROM employee WHERE age > 20;

```

- ## Table :

![image](https://github.com/user-attachments/assets/bb230fad-3f4e-49f8-b729-b3933a415ce6)
