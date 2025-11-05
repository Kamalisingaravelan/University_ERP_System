# University ERP System (Hibernate + Maven + MySQL)
A **comprehensive University Management System (ERP)** built using **Java, Hibernate ORM, and MySQL**. This project automates workflows including student management, faculty operations, library management, and admin reporting — all in a **command-line interface (CLI)** application

## Project Overview
This project automates and manages major activities within a university setup 
It supports various user roles such as **Admin**, **Faculty**, **Librarian**, and **Student** to perform CRUD and reporting operations efficiently

## Features

### Student Module
- view records using ID
- Manage attendance and marks
- Track fees (paid/pending) and total dues
### Faculty Module
- Add new students
- Manage course-related students
- Update student marks and attendance
- View academic reports and performance summaries
### Library & Member Module
- Issue and return books to students/faculty
- Auto-generate library member IDs
- Track due dates and calculate fines for late returns
### Admin Module
- View summarized dashboards (student, faculty, course, and fee reports)
- Filter students with **low attendance** or **pending fees**
- Remove any entity (students, faculty, courses, etc.)
- Monitor complete university data operations
### Authentication & Roles
- Supports multiple roles: `student`, `faculty`, `admin`, and `librarian`
- Each role has restricted access and dedicated menus

## Technology Stack

| Category | Technology Used |
|-----------|-----------------|
| **Language** | Java 17 |
| **ORM Framework** | Hibernate 6.2.7.Final |
| **Database** | MySQL |
| **Database Config** | `hibernate.cfg.xml` |
| **Architecture** | Layered MVC (Controller → Service → DAO → Entity) |
| **IDE** | Eclipse / IntelliJ IDEA |

 ## System Workflow
- **Admin**: Logs in to oversee university operations, manages users and data integrity, and monitors overall system reports
- **Faculty**: Authenticates, updates students’ marks and attendance, and reviews academic performance across assigned courses
- **Studen**t: Logs in to view attendance, marks, course details, and library records maintained by the university system
- **Librarian**: Manages book inventory, issues and returns books, and maintains library records linked to students and faculty
- **Library Member** (Student/Faculty): Requests or borrows books, and returns them within due dates as recorded by the librarian
- **System** (Backend Workflow): Handles all database operations through Hibernate DAO and Service layers, ensuring data consistency across modules

 ## Database Table Overview
- **Table Name**	Description	**Key Fields**
- students	Stores student details including **roll no, name, course, marks, and attendance	student_id (PK)**
- faculty	Contains faculty information and associated **departments	faculty_id (PK)**
- courses	Lists available **courses and subjects	course_id (PK)**
- library	Maintains book details including **title, author, and quantity	book_id (PK)**
- members	Tracks library **membership details** (linked with students/faculty)	**member_id (PK)**
- book_issues	Records **books issued, due dates, and fines	issue_id (PK), member_id (FK)**
- admin	Stores admin credentials and configuration data	**admin_id (PK)**

## **Project Structure**
<img width="304" height="678" alt="image" src="https://github.com/user-attachments/assets/77c32ca0-57bc-439c-9be6-3686ccd481ec" /> <img width="320" height="633" alt="image" src="https://github.com/user-attachments/assets/8bcd27f1-67fc-4d74-8175-56d11e781401" />

### **ER Diagram**
<img width="716" height="761" alt="image" src="https://github.com/user-attachments/assets/5d8fb987-b303-40aa-9dcf-1ee2ceb4a3ac" />

### **Sample Input & Output**
<img width="690" height="265" alt="image" src="https://github.com/user-attachments/assets/a8ff4c97-41b1-485b-b749-8fa3fe0b57c7" />
<img width="644" height="209" alt="image" src="https://github.com/user-attachments/assets/2aca20ec-1bbb-42ff-9914-609dd4e44927" />
<img width="654" height="314" alt="image" src="https://github.com/user-attachments/assets/1d8e2772-88a2-4034-8703-18a161632786" />
<img width="680" height="250" alt="image" src="https://github.com/user-attachments/assets/b63eb3c6-804d-48a4-a399-7050dc26316d" />
<img width="533" height="272" alt="image" src="https://github.com/user-attachments/assets/1ce79a77-21df-481d-b023-0a58a3aec37a" />


## Future Enhancements

- **Web-based Interface**: Upgrade console application into a Spring Boot + React full-stack system
- **Automated Email Alerts**: Notify students about attendance shortages, overdue books
- **Role-Based Authentication** (JWT): Secure login sessions using token-based access
- **Analytics Dashboard**: Add charts for attendance trends, department strength, and fee collection
- **Cloud Deployment**: Host the system on AWS / Azure with CI/CD integration

## Conclusion

The University Management System (ERP) provides an **integrated and efficient platform** for managing operations
It ensures seamless coordination between **students, faculty, librarians, and admin through a modular, role-based design**
By leveraging Hibernate ORM and Maven architecture, the project demonstrates scalability, maintainability, and industry-level standards for university management systems

**Author**

**Kamali Singaravelan**
