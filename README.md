# Payroll Management System

The Payroll Management System is a console-based application designed to manage employee records, including their personal details, work experience, and payroll information. This system allows administrators to perform various operations such as adding new records, editing existing records, deleting records, searching for specific records, and generating employee payslips.

## Features
- **User Authentication :** Secure login for administrators.
- **Employee Management :** Add, edit, delete, and search employee records.
- **Payroll Calculation :** Automated salary calculation based on working hours, allowances, and deductions.
- **Payslip Generation :** Generate and display employee payslips with detailed earnings and deductions.

## Technologies Used
- **C++ :** Core programming language used for developing the application.
- **File Handling :** Used for storing and retrieving employee records.
- **Windows.h :** Used for console manipulation (setting cursor position and window size).
- **conio.h :** Used for console input/output operations.
- **iomanip.h :** Used for formatted console output.

## Project Structure
### Header Files
- **include/ :** This directory contains the header files which define the classes and utility functions used in the project.
- **Employee.h**
  - Declaration of the `Employee` class.
  - Member variables: `job_code`, `employee_name`, `father_name`, `address`, `mobile_number`, `job_title`, `DOB`, `DOJ`, `email`, `basic_pay`.
  - Member functions: Constructors, getters, and setters for employee details.
- **Payroll.h**
  - Declaration of the `Payroll` class.
  - Functions related to payroll calculations, such as `calculateSalary()`, `generatePayslip()`, etc.
- **Utility.h**
  - Declarations for utility functions: `gotoXY(int X, int Y)`, `Cdelay(int msec)`, `border(int xLenS, int yLenS, int xLenE, int yLenE)`, etc.

### Source Files
- **src/**: This directory contains the source files which implement the classes and utility functions declared in the header files.
- **Employee.cpp**
  - Implementation of the `Employee` class functions.
- **Payroll.cpp**
  - Implementation of the `Payroll` class functions.
- **Utility.cpp**
  - Implementation of utility functions.

### Data File
- **data/**: This directory is used to store data files.
- **Records.txt**
  - Stores employee records in a structured format for persistence.
      
- **main.cpp**: This is the main source code file which contains the `main()` function and serves as the entry point of the application.

- **Makefile**: This file is used for building the project using the `make` command. It defines the rules for compiling and linking the source files.

## Usage
- **Login :** Enter the username admin and password password to access the system.
- **Main Menu :**
    - **Choose from the available options to perform operations :**
        - i to Insert New Record
        - e to Edit a Record
        - d to Delete a Record
        - s to Search a Record
        - l to List All Employees
        - p to Print Employee Payslip
        - q to Quit the Program
## Functions
  - **gotoXY(int X, int Y) :** Sets the cursor position in the console.
  - **Cdelay(int msec) :** Creates a delay for a specified number of milliseconds.
  - **border(int xLenS, int yLenS, int xLenE, int yLenE) :** Draws a bordered frame in the console.
  - **loginFrame(int xLenS, int yLenS, int xLenE, int yLenE) :** Draws the login frame.
  - **intro() :** Displays the introduction screen.
  - **login() :** Handles user authentication.
  - **menu() :** Displays the main menu.
  - **insert() :** Inserts a new employee record.
  - **edit() :** Edits an existing employee record.
  - **list() :** Lists all employee records.
  - **deletes() :** Deletes an employee record.
  - **search() :** Searches for an employee record by job code.
  - **setWindowSize(int width, int height) :** Sets the console window size.
  - **saverecords() :** Saves all employee records to a file.
  - **getrecords() :** Retrieves all employee records from a file.
  - **isFilePresent() :** Checks if the records file exists.
  - **displayPayslip() :** Displays the payslip for an employee.
