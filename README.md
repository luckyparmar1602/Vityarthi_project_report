# Vityarthi_project_report
# Employee Data Management System

## Overview
A menu-driven Python program that manages employee records using **file handling** and **CSV**. Employee data is held in a **dictionary** (keyed by Employee ID) while the program runs, and is saved to `employees.csv` so the records are kept between runs.

## Features
- **Add** a new employee (ID, name, department, salary)
- **Display** all employee records in a formatted table
- **Search** an employee by ID
- **Update** an existing employee's details
- **Delete** an employee record
- Duplicate Employee ID check
- Data saved automatically to a CSV file after every change
- Input validation for invalid menu choices

## Technologies / Tools Used
- Python 3
- Built-in `csv` module (reading/writing CSV files)
- Built-in `os` module (checking whether the file exists)
- Dictionaries for in-memory data storage
- Any code editor / IDE (VS Code, IDLE, PyCharm) or terminal

## Steps to Install & Run
1. Install Python 3 from [python.org](https://www.python.org/downloads/) (no extra libraries needed).
2. Download or clone this project and open the project folder.
3. Open a terminal in that folder and run:
   ```
   python employee_manager.py
   ```
4. Choose an option (1-6) from the menu.

The file `employees.csv` is created automatically the first time you add an employee.

## Instructions for Testing
| Test | Steps | Expected Result |
|------|-------|-----------------|
| Add | Choose 1, enter ID `101`, name, department, salary | "Employee added successfully." |
| Duplicate ID | Choose 1 and enter `101` again | "Employee ID already exists!" |
| Display | Choose 2 | All records shown in a table |
| Search | Choose 3, enter `101` | Employee details displayed |
| Search (invalid) | Choose 3, enter `999` | "Employee not found." |
| Update | Choose 4, enter `101`, change salary | "Record updated successfully." |
| Delete | Choose 5, enter `101` | "Record deleted successfully." |
| Persistence | Exit (6), run the program again, choose 2 | Previously saved records are still shown |
| Invalid choice | Enter `9` or a letter at the menu | "Invalid choice! Please enter 1-6." |


## Project Structure
```
employee_manager.py   # main program
employees.csv         # data file (auto-generated)
README.md             # project documentation
```
