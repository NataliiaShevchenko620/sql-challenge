# Employee SQL

This project is designed to address a comprehensive data challenge related to designing and creating a modern employee database using PostgreSQL database instead of legacy CSV files. 
The project is divided into three key areas: Data Modeling, Data Engineering, and Data Analysis. The challenge involves working with CSV files to create a relational database model, importing data into a database, and performing various data analysis queries.

## Project Structure

The project consists of a few files:

1. **EmployeeSQL/schema.png** - graphical representation of the database schema created using [Quick Database Diagrams](http://www.quickdatabasediagrams.com/)
2. **EmployeeSQL/schema.txt** - text representation of the database schema created using the tool above
3. **EmployeeSQL/EmployeeDB-schema.sql** - SQL file with DDL statements to create a structure of Employee DB. This script at the beginning contains commands to clean up the database, therefore it can be run both against empty and non-empty database
4. **EmployeeSQL/data** - a set of CSV files with source data
5. **EmployeeDB-insert-data.sql** - SQL script that performs filling out the tables with data. Data is a the same as in the CSV files
6. **EmployeeSQL/EmployeeDB-analysis.sql** - SQL file with queries that performs the following analytics:
   - List the employee number, last name, first name, sex, and salary of each employee.
   - List the first name, last name, and hire date for the employees who were hired in 1986.
   - List the manager of each department along with their department number, department name, employee number, last name, and first name.
   - List the department number for each employee along with that employee’s employee number, last name, first name, and department name.
   - List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.
   - List each employee in the Sales department, including their employee number, last name, and first name.
   - List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.
   - List the frequency counts, in descending order, of all the employee last names (that is, how many employees share each last name).

## Requirements

- PostreSQL 14

## Installation

1. Clone the repository to your local machine:

   ```
   [git clone https://github.com/NataliiaShevchenko620/sql-challenge.git](https://github.com/NataliiaShevchenko620/sql-challenge.git)
   ```

2. Create *EmployeeDB* in your PostgreSQL server
3. Run **EmployeeSQL/EmployeeDB-schema.sql** to create a schema
4. (option 1) Import data manually from **EmployeeSQL/data** using *Import/Export Data...* feature of pgAdmin 4. Use the following order:
   - departments
   - titles
   - employees
   - salaries
   - dept_emp
   - dept_manager
5. (option 2) Run **EmployeeDB-insert-data.sql** to import all data automatically

## Usage

Run **EmployeeSQL/EmployeeDB-analysis.sql** to conduct the analysis.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
