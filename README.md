# Module 9- SQL challenge

## Overview

This project involves setting up and querying a PostgreSQL database utilizing pgAdmin. Tasks include importing CSV data, designing tables and executing SQL queries to retrieve insights related to employee and employer data. 

## Database Schema

### The database consists of the following tables:

1. **departments** - Stores department details
2. **employees** - Stores employee personal details
3. **dept_emp** - Tracks department assignments for employees
4. **dept_manager** - Stores department manager information
5. **salaries** - Tracks employee salaries
6. **titles** - Stores job titles

<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\SQL_challenge_ERD.png" style="zoom: 67%;" />



## Creating Tables

Prior to importing the CSVs to run queries, tables must be created to provide a "landing spot" for the CSV files. This was accomplished by using the CREATE TABLE function followed by the name of the CSV file (department, titles, etc.), then creating column headers and specifying the data type (VARCHAR, INT) and finally setting either PRIMARY KEY (ensures that  no 2 rows can have the same value) or NOT NULL (ensuring that a column cannot have NULL values in the table). 

### Example of  Table creation 

1.  **departments** 

   ​	<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\departments_table.png" style="zoom: 50%;" />

2. **titles** 

   ​	<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\titles_table.png" style="zoom: 67%;" />

3. **employees** 

   ​	<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\employees_table.png" style="zoom:50%;" />

## Importing data

After the tables have been created in the database, you can now import the CSV files. This step must be taken to be able to run queries on the data. 

<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\created_tables.png" style="zoom:33%;"				  	/>		

After the tables have been created, the ability to import the CSV can be achieved by right clicking on the corresponding table for which CSV is to be imported, and selecting the import/export option. and follow the prompts within the sub menu.

## Queries and Outputs 

1. **employee information** - defines specific employee information (employee number, first and last name, sex and salary)

​	<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\employee_data.png" style="zoom: 50%;"								 	/>

<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\emp_output.png" style="zoom:50%;" 		/>	

2. **Employees hired in 1986** - lists only employees hired in 1986

<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\employees_1986.png" style="zoom:50%;" 		/>	

<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\1986_output.png" style="zoom:50%;" 			/>	



3. **Listing of Department Manager**-  lists the manager of each department with their employee information, along with department information

   ​	<img src="C:\Repos\sql-challenge\EmployeeSQL\Images\dept_manager.png" style="zoom:50%;" 			/>

   <img src="C:\Repos\sql-challenge\EmployeeSQL\Images\dept_manager_output.png" style="zoom:50%;" />	

   

   

   **Option to export quires to CSV Files** - to export the query results to CSV file, run the following input, and note it will need to be changed for each query: 

   <img src="C:\Repos\sql-challenge\EmployeeSQL\Images\to_csv.png" style="zoom:50%;" 		/>	

   







