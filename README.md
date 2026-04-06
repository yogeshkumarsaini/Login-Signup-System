# 🔐 Login & Signup System

A simple and secure **User Authentication System** built using **PHP & MySQL**.  
This project demonstrates core concepts like user registration, login/logout, password hashing, and session management.

---

## 🚀 Features

- User Registration 📝  
- User Login & Logout 🔑  
- Secure Password Hashing 🔐  
- Session Management  
- Form Validation  
- MySQL Database Integration  

---

## 🛠️ Tech Stack

- PHP  
- MySQL  
- HTML/CSS  
- Apache (XAMPP/LAMP)

---

## 📂 Project Structure

```
login-system/
│── config.php
│── register.php
│── login.php
│── dashboard.php
│── logout.php
```

---

## ⚙️ Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/your-username/login-system.git
```

2. Move project to server directory:

- XAMPP → htdocs/
- WAMP → www/
  
3. Create Database in MySQL:
```
CREATE DATABASE login_system;

USE login_system;

CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100) UNIQUE,
    password VARCHAR(255),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

4. Update database credentials in config.php:
```
$conn = new mysqli("localhost", "root", "", "login_system");
```

5. Run the project:
```
http://localhost/login-system/
```
---
## 🔐 Security Features

- Passwords are hashed using password_hash()
- Login verification using password_verify()
- Session-based authentication
- Basic input validation

---

## 📸 Screens
- Register Page
- Login Page
- Dashboard
