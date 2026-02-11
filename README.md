

🏦 Bank Account Management System

A simple Core Java console application built using JDBC and Oracle Database to perform basic banking operations such as deposits, withdrawals, and balance checks.
This project demonstrates Object-Oriented Programming (OOP) principles and follows a layered architecture (Bean → DAO → Service → Util → Main) to separate business logic, database access, and application flow.

🚀 Features

Account Operations
Deposit money into account
Withdraw money from account
Check account balance
Transaction Handling
Records transactions in database
Updates account balance automatically
Validation
Prevents insufficient balance withdrawals
Prevents negative/zero transactions
Handles invalid inputs gracefully
Custom exception for insufficient funds

🛠 Technologies Used

Java (Core Java)
JDBC
Oracle Database (XE)
Console-based UI
Eclipse/IntelliJ

📂 Project Structure

The project is organized into layers:
Bean Layer
Contains JavaBeans that hold data.
TransferBean.java → Stores transaction/account details
DAO Layer
Handles all database operations.
BankDAO.java → Deposit, withdraw, balance queries

Service Layer

Contains business logic and validations.
BankService.java
Util Layer
Manages database connection and utilities.
DBUtil.java → JDBC connection setup
InsufficientFundsException.java → Custom exception

Main Layer

Entry point of the application.
BankMain.java → Console menu and user interaction

⚙️ Configuration
Update database details inside:
DBUtil.java
Change:
URL
Username
Password
Add Oracle JDBC driver (ojdbc.jar) to project libraries.

▶️ How to Run

Import project into Eclipse/IntelliJ
Add Oracle JDBC driver to build path
Configure database
Run:

BankMain.java
🧩 Application Flow

User selects option → Main → Service → Validation → DAO → Database → Result displayed

▶️ Sample Console Menu
1. Deposit
2. Withdraw
3. Check Balance
4. Exit

Example:

Enter account number: 101
Enter amount to deposit: 5000
Deposit successful
Updated Balance: 15000
🎯 Learning Objectives

This project helps understand:

Core Java programming
JDBC connectivity
CRUD operations
Layered architecture
Exception handling
Custom exceptions
Console application design

🔮 Future Enhancements
Add account creation
Transaction history
Money transfer between accounts
Logging
GUI using JavaFX/Swing
Convert to Web using Servlets/Spring Boot
Add connection pooling

👨‍💻 Author

Developed as a learning project for practicing Core Java + JDBC + Database integration concepts.

📜 License

This project is free to use for educational purposes.
