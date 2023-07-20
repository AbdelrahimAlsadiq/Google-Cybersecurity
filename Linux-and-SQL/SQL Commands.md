### ```SELECT```
- Indicates which columns to return.

---
### 
```sql
FROM
```
- Indicates which table to query.
- Examples:
  - ```sql
    SELECT employee_id, device_id FROM employees;
    ```
  - ```sql
    SELECT * FROM employees;
    ```

---
### ```ORDER BY```
- sequences the records returned by a query based on a specified column or columns
- Examples:
  - ```SELECT * FROM employees ORDER BY city``` orders the result by city in ascending order.
  - ```SELECT * FROM employees ORDER BY city DESC``` orders the result by city in descending order.

---
### ```WHERE```
- Indicates the condition or a filter.
- Examples:
  - ```SELECT * FROM employees WHERE city = 'LUXOR'``` shows all employees working in LUXOR.
  - 

---
### ```LIKE```
- Used with ```WHERE``` to search for a pattern in a column.
- Examples:
  - ```SELECT * FROM employees WHERE office LIKE 'East%';``` shows all employees that has 'East' in their office name. (% is a wildcard, means any number of characters).
  - ```SELECT * FROM employees WHERE office LIKE 'a___';``` shows all employees that starts with 'a' and has 4 characters length. (_ is a wildcard, means only one character).

---
### ```BETWEEN```
- An operator that filters for numbers or dates within a range.
- Examples:
  - ```SELECT * FROM login_attempts WHERE date BETWEEN '15:00' AND '16:00';```

---
### ```AND``` | ```OR``` | ```NOT```
- ```AND``` Specifies that both conditions must be met simultaneously.
- ```OR``` Specifies that either condition can be met.
- ```NOT``` Negates a condition.
- Examples:
  - ```SELECT * FROM employees WHERE city = 'LUXOR AND department = 'Sales''``` shows all employees working in LUXOR and in sales department.
  - ```SELECT * FROM employees WHERE city = 'LUXOR OR NOT department = 'Sales''``` shows all employees that either working in LUXOR or not in sales department.

---
### ```INNER JOIN```
- Returns rows matching on a specified column that exists in more than one table.
- Examples:
  - ```SELECT username, office, operating_system FROM employees INNER JOIN machines ON employees.employee_id = machines.employee_id```

---
### ```LEFT JOIN```
- Returns all of the records of the first table, but only returns rows of the second table that match on a specified column.

---
### ```RIGHT JOIN```
- Returns all of the records of the second table, but only returns rows of the first table that match on a specified column.

---
### ```FULL OUTER JOIN```
- Returns all records from both tables.

---
### ```COUNT()```
- returns a single number that represents the number of rows returned from your query.
- Examples:
  - ```SELECT COUNT(firstname) FROM customers;```

---
### ```AVG()```
- returns a single number that represents the average of the numerical data in a column.

---
### ```SUM```
- returns a single number that represents the sum of the numerical data in a column.
