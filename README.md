# Library Management System (LMS)

This is a Java-based Library Management System (LMS) integrated with MySQL. The system allows administrators, librarians, clerks, and borrowers to manage library operations like issuing books, checking fine statuses, placing books on hold, and managing user data. It stores all data in a MySQL database.

## Features

- **Book Management**: Add, remove, update books and search books by title, author, and subject.
- **Borrower Management**: Create, view, and manage borrower information and books borrowed.
- **Hold Requests**: Borrowers can place books on hold, and librarians/clerks can manage these requests.
- **Loan Management**: Issue and return books, track loan history, and calculate fines.
- **Admin Panel**: Admin functionality to add/remove librarians and clerks and manage the library's inventory of books.

## Technologies Used

- **Java**: The main programming language for building the system.
- **MySQL**: Database management system to store user and book data.
- **JDBC**: Java Database Connectivity for interacting with the MySQL database.
- **CLI (Command-Line Interface)**: For user interaction.

## Installation

### Prerequisites

- **Java 8+**: Make sure Java is installed on your system.
- **MySQL**: Install and set up MySQL on your local machine or a remote server.
- **IDE**: Use an IDE like IntelliJ IDEA or Eclipse to run and manage the project.


Usage
Login
Upon running the program, you will be prompted to log in. Enter the ID and password of the user (borrower, clerk, librarian).

Admin Portal
Admin users can:

Add/remove librarians and clerks.

Manage the library's book inventory.

View loan history of all books in the library.

Borrower Portal
Borrowers can:

Search and view books.

Place books on hold if they are issued.

View borrowed books and fine status.

Staff Portal (Clerks and Librarians)
Clerks and Librarians can:

Search books and issue/return them.

Place/Manage book hold requests.

View and update borrower information.

Fine Calculation
The system automatically calculates the fine for a borrower if they return a book after the due date.

Book Search and Hold Requests
Users can search for books by title, subject, or author. If a book is issued, they can place a hold request.

Loan History
All users can view loan history including the borrower's name, issue date, return date, and any fine paid.

Code Structure
Library.java: Manages the overall library system and interaction with the database.

Book.java: Represents a book object in the system.

Borrower.java: Represents a borrower (a person who can borrow books).

Clerk.java: Represents a clerk (library staff who handles book transactions).

Librarian.java: Represents the librarian (oversees all library operations).

Loan.java: Represents a book loan (issued and returned books).

HoldRequest.java: Represents a hold request for a book.

Person.java: A base class for Clerk, Librarian, and Borrower.

Main.java: The entry point for the application.

Contributions
Feel free to fork this project, contribute to it, or report any issues.

Fork the repository

Create a new branch (git checkout -b feature-branch)

Commit your changes (git commit -m 'Add feature')

Push to your forked branch (git push origin feature-branch)

Create a pull request

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
MySQL for database management.

Java for building the core functionality.

JDBC for connecting the application to the MySQL database.
