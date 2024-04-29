Table_schemata.sql

This file contains SQL commands to manage database tables for a company's employee records. Here’s what it does:

Drops existing tables if they exist to clean up the database. This is useful for resetting the table structures during development or testing.
Creates tables including departments, titles, employees, dept_emp, dept_manager, and salaries.
departments holds department numbers and names.
titles lists possible job titles.
employees stores detailed employee information, including a reference to titles.
dept_emp links employees with departments, allowing for many-to-many relationships (employees can work in multiple departments).
dept_manager tracks which employees manage which departments.
salaries records employee salaries, which presumably can change over time (though the table lacks a date range for salaries).


queries.sql

This file includes various SQL queries to retrieve information from the database structured in the previous file:

Employee details and salaries: Retrieves the employee number, last name, first name, sex, and salary for all employees.
Employees hired in 1986: Lists employees by first name, last name, and hire date, specifically for those hired in 1986, sorted by hire date.
Department managers: Lists department managers along with department numbers, names, and the managers’ names.
Employee department details: Lists department and employee details, linking each employee to their department.
Employees named Hercules with last names starting with 'B': Specifically fetches employees named Hercules whose last names begin with the letter B.
Sales department employees: Lists all employees in the Sales department.
Sales and Development department employees: Lists all employees in both the Sales and Development departments.
Employee last name frequencies: Counts how many employees share each last name, ordering the count from highest to lowest.
These scripts are typical for database management in a corporate setting, facilitating both the structural setup and everyday data retrieval needs.
