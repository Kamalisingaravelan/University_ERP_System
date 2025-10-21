# University ERP System (Hibernate + Maven + MySQL)
A **comprehensive University Management System (ERP)** built using **Java, Hibernate ORM, and MySQL**. This project automates workflows including student management, faculty operations, library management, and admin reporting - — all in a **command-line interface (CLI)** application.

## Project Overview
This project automates and manages major activities within a university setup.  
It supports various user roles such as **Admin**, **Faculty**, **Librarian**, and **Student** to perform CRUD and reporting operations efficiently.

## Features

### Student Module
- view records using ID.
- Manage attendance and marks.
- Track fees (paid/pending) and total dues.
### Faculty Module
- Add new students
- Manage course-related students.
- Update student marks and attendance.
- View academic reports and performance summaries.
### Library & Member Module
- Issue and return books to students/faculty.
- Auto-generate library member IDs.
- Track due dates and calculate fines for late returns.
### Admin Module
- View summarized dashboards (student, faculty, course, and fee reports).
- Filter students with **low attendance** or **pending fees**.
- Remove any entity (students, faculty, courses, etc.).
- Monitor complete university data operations.
### Authentication & Roles
- Supports multiple roles: `student`, `faculty`, `admin`, and `librarian`.
- Each role has restricted access and dedicated menus.

## Technology Stack

| Category | Technology Used |
|-----------|-----------------|
| **Language** | Java 17 |
| **ORM Framework** | Hibernate 6.2.7.Final |
| **Database** | MySQL |
| **Database Config** | `hibernate.cfg.xml` |
| **Architecture** | Layered MVC (Controller → Service → DAO → Entity) |
| **IDE** | Eclipse / IntelliJ IDEA |
