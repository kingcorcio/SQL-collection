# SQL-collection
just a collection of sql stuff


Here is a basic SQL cheatsheet with some common SQL commands and syntax:
SELECT statement:
SELECT column1, column2, ... FROM table_name WHERE condition; 
SELECT: specifies the columns to retrieve data from.
FROM: specifies the table from which to retrieve the data.
WHERE: filters the rows based on a condition.
Example:
SELECT * FROM employees WHERE department = 'Sales'; 
UPDATE statement:
UPDATE table_name SET column1 = value1, column2 = value2, ... WHERE condition; 
UPDATE: modifies existing records in a table.
SET: specifies the new values for the columns.
WHERE: filters the rows to be updated.
Example:
UPDATE employees SET salary = salary * 1.1 WHERE department = 'Engineering'; 
INSERT statement:
INSERT INTO table_name (column1, column2, ...) VALUES (value1, value2, ...); 
INSERT INTO: inserts new records into a table.
VALUES: specifies the values to be inserted into the columns.
Example:
INSERT INTO employees (name, age, salary) VALUES ('John Smith', 30, 50000); 
DELETE statement:
DELETE FROM table_name WHERE condition; 
DELETE: deletes existing records from a table.
WHERE: filters the rows to be deleted.
Example:
DELETE FROM employees WHERE department = 'HR'; 
JOIN statement:
SELECT column1, column2, ... FROM table1 JOIN table2 ON table1.column = table2.column WHERE condition; 
JOIN: combines rows from two or more tables based on a related column between them.
ON: specifies the condition for the join.
WHERE: filters the rows based on a condition.
Example:
SELECT employees.name, departments.department_name FROM employees JOIN departments ON employees.department_id = departments.department_id; 
GROUP BY statement:
SELECT column1, SUM(column2) FROM table_name GROUP BY column1; 
GROUP BY: groups the rows based on the values of a column.
SUM: calculates the sum of a column for each group.
Example:
SELECT department, SUM(salary) FROM employees GROUP BY department; 
ORDER BY statement:
SELECT column1, column2, ... FROM table_name ORDER BY column1 ASC/DESC; 
ORDER BY: sorts the rows based on the values of one or more columns.
ASC: sorts the rows in ascending order (default).
DESC: sorts the rows in descending order.
Example:
SELECT name, age FROM employees ORDER BY age DESC;

