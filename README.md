# 🏦 Banking Management System (C++ | OOP)

<div align="center">

**A console-based Banking Management System built using C++ to demonstrate core Object-Oriented Programming (OOP) concepts through a real-world use case.**

📌 *Designed for academic learning, practical OOP implementation, and system-level understanding.*

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Key OOP Concepts Implemented](#-key-oop-concepts-implemented)
- [System Architecture](#-system-architecture)
- [Class Breakdown](#-class-breakdown)
- [Features](#-features)
- [File Handling & Data Persistence](#-file-handling--data-persistence)
- [Project Structure](#-project-structure)
- [Installation & Execution](#-installation--execution)
- [How to Use](#-how-to-use)
- [Learning Outcomes](#-learning-outcomes)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)
- [Author](#-author)

---

## 🌟 Overview

The **Banking Management System** is a **menu-driven C++ application** that simulates basic banking operations such as opening accounts, depositing money, withdrawing funds, and managing different account types.

The primary goal of this project is to **demonstrate Object-Oriented Programming (OOP) principles** including:

- Encapsulation  
- Abstraction  
- Inheritance  
- Polymorphism  

while also incorporating **file handling** for data persistence.

---

## 🧠 Key OOP Concepts Implemented

| Concept | Implementation |
|---------|---------------|
| **Encapsulation** | Private data members with public getters/setters |
| **Abstraction** | Menu-driven interface hides internal logic |
| **Inheritance** | Specialized account types derived from base class |
| **Polymorphism** | Virtual functions for transaction handling |

---

## 🏗️ System Architecture

```
User
  ↓
Menu Interface (main)
  ↓
Bank Class
  ↓
Account / Transaction Hierarchy
  ↓
File Storage (Bank.data)
```

---

## 🧩 Class Breakdown

### 1️⃣ Account Class
- Represents a generic bank account
- Stores:
  - Account Number
  - First Name
  - Last Name
  - Account Balance
- Provides:
  - Deposit
  - Withdraw
  - Balance inquiry
- Demonstrates **encapsulation** using private members

---

### 2️⃣ SavingsAccount & CheckingAccount Classes
- Inherit from the `Account` base class
- Demonstrate **inheritance & specialization**

#### SavingsAccount
- Applies interest to balance using `applyInterest()`

#### CheckingAccount
- Deducts monthly service fees using `deductFees()`

---

### 3️⃣ Transaction Hierarchy
- `Transaction` → Abstract base class
- Derived classes:
  - `DepositTransaction`
  - `WithdrawTransaction`
- Uses **virtual functions** to demonstrate **runtime polymorphism**

---

### 4️⃣ Bank Class
- Manages all accounts using `std::map`
- Responsibilities:
  - Open/close accounts
  - Deposit & withdrawal handling
  - Balance inquiries
  - Load & save account data
- Acts as the **core controller** of the system

---

### 5️⃣ Menu-Driven Interface
- Console-based user interaction
- Provides options to:
  - Open account
  - Deposit money
  - Withdraw money
  - Check balance
  - View all accounts
  - Close account
- Demonstrates **abstraction** by hiding internal logic

---

## ✨ Features

- ✔️ Object-Oriented design
- ✔️ Multiple account types
- ✔️ Secure encapsulation of data
- ✔️ Persistent data storage using files
- ✔️ Menu-driven user experience
- ✔️ Real-world banking workflow simulation

---

## 💾 File Handling & Data Persistence

Account data is stored in a file named: **Bank.data**

### How it works:
- Data is **loaded** from the file when the program starts
- Updated data is **saved** back to the file before program termination
- Ensures account details persist across executions

---

## 📁 Project Structure

```
Banking_Management_System/
│
├── code.cpp        # Main C++ source file
├── Bank.data       # Persistent account storage
├── README.md       # Project documentation
└── LICENSE         # License file
```

---

## 🚀 Installation & Execution

### Prerequisites
- C++ Compiler (GCC/g++)
- Basic knowledge of terminal commands

---

### Step 1️⃣ Clone the Repository
```bash
git clone https://github.com/Thefaizanhassan/Banking_Management_System.git
```

---

### Step 2️⃣ Navigate to Project Directory

```bash
cd BankingManagementSystem
```

---

### Step 3️⃣ Compile the Program

```bash
g++ -o mybankingapp code.cpp
```

---

### Step 4️⃣ Run the Application

```bash
./mybankingapp
```

---

## 🧭 How to Use

1. Launch the program
2. Choose options from the menu
3. Perform banking operations:
   - Open account
   - Deposit/Withdraw funds
   - View account details
4. Exit safely to ensure data is saved

---

## 🎓 Learning Outcomes

By working on this project, you will gain hands-on experience with:

- Practical Object-Oriented Programming in C++
- Class hierarchies and inheritance
- Virtual functions & polymorphism
- File I/O operations
- Designing scalable console applications
- Real-world system modeling

---

## 🔮 Future Enhancements

- 🔐 User authentication (PIN-based login)
- 🗃️ Database integration (instead of file handling)
- 📊 Transaction history tracking
- 🖥️ GUI-based interface
- 🌐 Web or REST-based banking simulation

---

## 📜 License

This project is licensed under the **MIT License**.

- ✔️ Free to use
- ✔️ Free to modify
- ✔️ Free to distribute

---

## 👨‍💻 Author

**Faizan Hassan**  
Software Developer | AI/ML Enthusiast | Problem Solver

- 🔗 GitHub: [https://github.com/Thefaizanhassan](https://github.com/Thefaizanhassan)
- 🔗 LinkedIn: [https://www.linkedin.com/in/thefaizanhassan](https://www.linkedin.com/in/thefaizanhassan)

---

<div align="center">

⭐ **If this project helped you understand OOP better, consider starring the repo!** ⭐

</div>
