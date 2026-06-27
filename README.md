# 🏦 Bank Management System

A robust, console-based Java application that simulates a real-world banking environment. It demonstrates core Object-Oriented Programming (OOP) principles, in-memory data management, and fundamental banking operations.

## 🚀 Features

- **Account Management**: Seamlessly open new accounts (Savings or Current) with optional initial deposits. Auto-generates sequential account numbers (e.g., `AC000001`).
- **Secure Transactions**: Perform secure deposits, withdrawals, and inter-account transfers.
- **Account Statements**: View chronological transaction histories for any account, including deposits, withdrawals, and transfers.
- **Search & Listing**: Easily search for accounts using a customer's name, or list all active accounts in the system.
- **Robust Validation**: Custom exception handling prevents negative deposits, stops withdrawals with insufficient funds, and ensures secure inter-account transfers.

## 🛠️ Technologies Used

- **Language**: Core Java (Java 8+ recommended)
- **Data Storage**: In-Memory Data Structures (`HashMap`, `ArrayList`)
- **Key Concepts**: 
  - Object-Oriented Architecture (Domain Models, Services, Repositories)
  - Java 8 Streams API & Lambda Expressions
  - Custom Exception Handling (`InsufficientFundsException`, `AccountNotFoundException`, etc.)
  - UUID Generation for internal IDs

## 📁 Project Structure

```text
src/
├── app/
│   └── Main.java                 # Interactive CLI entry point
├── domain/
│   ├── Account.java              # Account entity model
│   ├── Customer.java             # Customer entity model
│   ├── Transaction.java          # Transaction entity model
│   └── Type.java                 # Transaction type Enum (DEPOSIT, WITHDRAW, etc.)
├── exceptions/
│   ├── AccountNotFoundException.java
│   ├── InsufficientFundsException.java
│   └── ValidationException.java
├── repository/
│   ├── AccountRepository.java    # In-memory storage for Accounts
│   ├── CustomerRepository.java   # In-memory storage for Customers
│   └── TransactionRepository.java# In-memory storage for Transactions
├── service/
│   ├── BankService.java          # Bank business logic interface
│   └── impl/BankServiceImpl.java # Core business logic implementation
└── util/
    └── Validation.java           # Reusable validation interface
```

## ⚙️ Getting Started

### Prerequisites

- **Java Development Kit (JDK)**: Version 8 or higher installed on your machine.
- An IDE (like IntelliJ IDEA, Eclipse) or command-line tools to compile and run Java programs.

### Installation & Execution

1. **Clone the repository:**
   ```bash
   git clone <your-repository-url>
   ```

2. **Navigate to the source directory:**
   ```bash
   cd src
   ```

3. **Compile the Java files:**
   ```bash
   javac app/Main.java
   ```

4. **Run the application:**
   ```bash
   java app.Main
   ```

## 💡 Usage

Upon running the application, you will be greeted with an interactive console menu:

```text
Welcome to Console Bank
1) Open Account
2) Deposit
3) Withdraw
4) Transfer
5) Account Statement
6) List Accounts
7) Search Accounts by Customer Name
0) Exit
CHOOSE: 
```

Simply enter the number corresponding to the action you wish to perform and follow the on-screen prompts.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! 
Feel free to open an issue or submit a pull request if you have ideas on how to improve this project (e.g., adding a real database connection using JDBC/JPA).

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).
