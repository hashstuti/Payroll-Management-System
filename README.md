# Payroll-Management-System
# Employee Management Database

This repository contains SQL scripts that create and manage a comprehensive employee management database. The database consists of multiple tables designed to store employee information, salary details, department assignments, projects, attendance, and educational history.

## Database Structure

### 1. **Employee Table**
The `Employee` table stores personal and basic employment details of employees.

- **Columns:**
  - `Employee_Id` (Primary Key)
  - `First_Name`
  - `Last_Name`
  - `Hire_Date`
  - `City`
  - `State`
  - `Department_Id` (Foreign Key)

### 2. **Department Table**
The `Department` table stores department information.

- **Columns:**
  - `Department_Id` (Primary Key)
  - `Department_Name`

### 3. **Salary Table**
The `Salary` table stores salary information, including tax deductions.

- **Columns:**
  - `Salary_Id` (Primary Key)
  - `Gross_Salary`
  - `Hourly_Pay`
  - `State_Tax`
  - `Federal_Tax`
  - `Account_Id` (Foreign Key)

### 4. **DepartmentProject Table**
The `DepartmentProject` bridge table links departments and projects. Each department can have multiple projects.

- **Columns:**
  - `Department_Id` (Foreign Key)
  - `Project_Id` (Foreign Key)

## Inserting Data

Sample data is inserted into various tables including `Employee`, `Department`, `Project`, `AccountDetails`, `Education`, `Leave`, `Attendance`, `Work_Location`, `Employee_Attendance`, and `DepartmentProject`.

Example of inserting a new employee is available in the provided scripts.

## Updating Data

You can update the employee data, such as changing the department of an employee. Refer to the provided scripts for details.

## External Data Import

Salary data can be imported from an external CSV file. The necessary SQL commands to create an external table for importing the data are provided.

## Commit and Rollback

The scripts demonstrate transaction management using `COMMIT`, `ROLLBACK`, and `SAVEPOINT`. This allows rolling back changes to specific points in the transaction history.

## Learning Resources

This repository and the SQL scripts were built using the knowledge gained from the following repository:

[Repository Name - ojasphansekar/Employee-Payroll-Management-System](https://github.com/ojasphansekar/Employee-Payroll-Management-System)
