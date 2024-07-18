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

## Screenshots
<div align="left">
    <h2>Home Page</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td><img src="https://github.com/user-attachments/assets/f45f8552-c41d-4746-8cf0-535a501fccad" alt="Home Page" width="500"/></td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Login Page</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td><img src="https://github.com/user-attachments/assets/aa514284-5d2b-4c72-bcfb-eb97ee6ea489" alt="Credentials" width="400"/></td>
            <td><img src="https://github.com/user-attachments/assets/b0b4764a-24d7-473b-9177-4922a9e2e61e" alt="Entry" width="400"/></td>
        </tr>
        <tr>
            <td align="center">Credentials</td>
            <td align="center">Entry</td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Choosing Options</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td><img src="https://github.com/user-attachments/assets/b1859738-bb83-4004-b49c-fae3ba6b79fc" alt="Choosing Options" width="500"/></td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Option i : Inserting a Record</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td><img src="https://github.com/user-attachments/assets/5d22feef-3ab6-4a2b-9379-9514c4a2351e" alt="Insertion" width="500"/></td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Option l : List Of Records</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td>
                <img src="https://github.com/user-attachments/assets/bde23cb9-570c-44a5-9d6e-59bd69ed9422" alt="List Of Records" width="500"/>
            </td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Option e : Edit a Record</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td><img src="https://github.com/user-attachments/assets/0f0d2887-46ab-49a7-8327-48ce78fcfb71" alt="Options To Edit" width="400"/></td>
            <td><img src="https://github.com/user-attachments/assets/b0167103-cbf0-451f-a896-6a91febc9cc0" alt="After Editing" width="400"/></td>
        </tr>
        <tr>
            <td align="center">Options To Edit</td>
            <td align="center">After Editing</td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Option s : Search a Record</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td>
                <img src="https://github.com/user-attachments/assets/0a0dd46a-f425-4532-937e-9f9e2978f467" alt="Searching Records" width="500"/>
            </td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Option p : Employee Pay Slip</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td>
                <img src="https://github.com/user-attachments/assets/74dfc76e-f6aa-4c77-8af6-9862b64aed59" alt="Employee Pay Slip" width="500"/>
            </td>
        </tr>
    </table>
</div>


<div align="left">
    <h2>Option d : Deletion Of Record</h2>
</div>
<div align="center">
    <table>
        <tr>
            <td> <img src="https://github.com/user-attachments/assets/8dda1cc1-7dd6-47b0-8002-23c01d0d0fcd" alt="Employee Pay Slip" width="400"/> </td>
            <td> <img src="https://github.com/user-attachments/assets/dd69617b-1e22-42c0-9365-3d065c3f4e4d" alt="Employee Pay Slip" width="400"/> </td>
          <tr>
            <td align="center">Choose a Record To Delete</td>
            <td align="center">After Deletion</td>
        </tr>
        </tr>
    </table>
</div>
