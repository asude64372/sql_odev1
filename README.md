
# SQL Assignment - Employee and Department Queries

This document contains SQL queries used to retrieve specific data from the `employees` and `departments` tables.

## 1. Retrieve Employee Names and Salaries
```sql
SELECT first_name, last_name, salary 
FROM employees;
```
- This query selects the first name, last name, and salary of all employees from the `employees` table.

## 2. Retrieve Unique Department Names
```sql
SELECT DISTINCT department_name 
FROM departments;
```
- This query fetches all unique department names from the `departments` table.

## 3. Retrieve IT Department Information
```sql
SELECT * 
FROM departments 
WHERE department_name = 'IT';
```
- This query retrieves all details of the department where `department_name` is **IT**.
- Ensure there is no extra space before or after 'IT' to avoid errors.

## 4. Retrieve Employees Ordered by Salary
```sql
SELECT * 
FROM employees 
ORDER BY salary;
```
- This query retrieves all employee details and sorts them by salary in ascending order.
- To sort in descending order, use `ORDER BY salary DESC`.

## 5. Retrieve Full Names of Employees
```sql
SELECT first_name || ' ' || last_name AS full_name 
FROM employees;
```
- This query concatenates the first and last name of each employee into a single column named `full_name`.

## Notes
- Ensure the database schema matches the table and column names in these queries.
- Modify queries as needed based on your specific database structure.
- If any issues arise, check for typos or formatting errors in column/table names.
