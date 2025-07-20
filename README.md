# 📚 Library Management System (LMS) – FastAPI

## 🢾 1. Project Overview

Build a RESTful API for a Library Management System using FastAPI that allows users to:

* Manage books (add/update/delete)
* Borrow and return books
* View borrowing history
* Authenticate securely using JWT tokens

The system supports three user roles:

* **Admin**
* **Manager**
* **Student**

---

## 👥 2. User Roles & Permissions

| Action                     | Admin | Manager | Student  |
| -------------------------- | ----- | ------- | -------- |
| Register users             | ✅     | ❌       | ❌        |
| Login                      | ✅     | ✅       | ✅        |
| Add/edit/delete books      | ✅     | ✅       | ❌        |
| View all books             | ✅     | ✅       | ✅        |
| Borrow books               | ✅     | ✅       | ✅ (self) |
| Return books               | ✅     | ✅       | ✅ (self) |
| View all borrowing logs    | ✅     | ✅       | ❌        |
| View own borrowing history | ✅     | ✅       | ✅        |

---

## ⚙️ 3. Features

### 📌 Authentication

* Register (admin-only)
* Login (all roles)
* JWT token generation with expiration
* Passwords hashed using bcrypt

### 📚 Book Management

* Add, update, delete books (admin/manager)
* View all books

### 🔄 Borrowing System

* Borrow a book (only if available)
* Return a book
* Prevent double borrowing
* History tracking (borrow date, return date)

### 🧾 Borrowing Logs

* Admin/Manager can view all logs
* Students can only view their own logs
# Library-Management-System-LMS---FastAPI-Implementation
