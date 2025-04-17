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




## Usage

### Login
Upon running the program, you will be prompted to log in. Enter the **ID** and **password** of the user (borrower, clerk, librarian).

---

### Admin Portal
Admin users can:
- **Add/Remove Librarians and Clerks**: Manage the staff of the library.
- **Manage the Library's Book Inventory**: Add, remove, or modify books in the library's collection.
- **View Loan History**: View the entire history of all books that have been issued or returned.

---

### Borrower Portal
Borrowers can:
- **Search and View Books**: Browse available books by title, subject, or author.
- **Place Books on Hold**: If the book is issued to another borrower, place a request to hold the book.
- **View Borrowed Books and Fine Status**: Check which books are currently borrowed and the fine incurred (if any).

---

### Staff Portal (Clerks and Librarians)
Clerks and Librarians can:
- **Search Books and Issue/Return Them**: Handle book transactions and manage their status (issued or returned).
- **Place/Manage Hold Requests**: Approve or cancel hold requests for books.
- **View and Update Borrower Information**: Manage borrower records and update personal details.

---

### Fine Calculation
The system **automatically calculates** the fine for a borrower if they return a book after the due date.

---

### Book Search and Hold Requests
Users can:
- **Search for Books**: Search for books by title, subject, or author.
- **Place a Hold Request**: If a book is already issued, they can place a hold request to get the book once it’s available.

---

### Loan History
All users can:
- **View Loan History**: Includes borrower’s name, issue date, return date, and any fine paid.

---

## Code Structure

### Files in the Project:
- **Library.java**: Manages the overall library system and its interaction with the database.
- **Book.java**: Represents a book object in the system.
- **Borrower.java**: Represents a borrower (a person who can borrow books).
- **Clerk.java**: Represents a clerk (library staff responsible for handling book transactions).
- **Librarian.java**: Represents the librarian (who oversees all library operations).
- **Loan.java**: Represents a book loan (issued and returned books).
- **HoldRequest.java**: Represents a hold request for a book.
- **Person.java**: A base class for `Clerk`, `Librarian`, and `Borrower`.
- **Main.java**: The entry point for the application.

---

JDBC for connecting the application to the MySQL database.
