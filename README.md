# StudentRegSystem
🎓 Student Admission Management System

A full-stack ASP.NET Core MVC web application for managing student admissions, built with a custom (DIY) admin authentication system and SQL Server.

This project demonstrates backend fundamentals, MVC architecture, Entity Framework Core, and real-world CRUD workflows without relying on ASP.NET Identity.

🚀 Features
👨‍🎓 Student Side

Student admission form

Stores applicant details securely

Admission status tracking:

Pending

Accepted

Rejected

🛠 Admin Dashboard

Custom admin login (DIY authentication)

View total number of applicants

View counts by admission status

List all students in a table

Edit student admission status

Delete student records

Recent students overview

🧱 Tech Stack

Backend: ASP.NET Core MVC

Database: SQL Server

ORM: Entity Framework Core

Frontend: Razor Views, Bootstrap

Authentication: Custom admin login (No ASP.NET Identity)

Architecture: MVC + ViewModels

📁 Project Structure
StudentAdmissionSystem/
│
├── Controllers/
│   ├── AdminController.cs
│   └── StudentController.cs
│
├── Models/
│   ├── Entities/
│   │   └── Student.cs
│   └── ViewModels/
│       ├── DashboardVM.cs
│       └── AdminLoginVM.cs
│
├── Views/
│   ├── Admin/
│   │   ├── Dashboard.cshtml
│   │   ├── Edit.cshtml
│   │   ├── Delete.cshtml
│   └── Student/
│       └── Apply.cshtml
│
├── Data/
│   └── ApplicationDbContext.cs
│
└── Program.cs

🧠 Key Concepts Demonstrated

MVC pattern in ASP.NET Core

Entity Framework Core (CRUD operations)

ViewModels for clean separation of concerns

Enum usage for admission status

Server-side validation

Secure admin-only routes

Dashboard metrics using LINQ

Razor syntax and data binding

⚙️ Setup Instructions

Clone the repository

git clone https://github.com/yourusername/StudentAdmissionSystem.git


Update connection string

Edit appsettings.json

Point it to your SQL Server instance

Apply database migration

dotnet ef database update


Run the project

dotnet run


Access admin dashboard

/Admin/Login

🔐 Authentication Note

This project uses a DIY admin authentication system (session-based) instead of ASP.NET Identity.

ASP.NET Identity is intentionally skipped in this project to demonstrate low-level authentication logic.
Identity will be covered in subsequent projects.

📌 Why This Project Matters

This project shows:

You understand how things work under the hood

You can build real admin systems

You can manage state, data, and roles

You can ship a complete, usable application

Perfect for:

Internship applications

Junior backend roles

Portfolio demos

🧑‍💻 Author

Divine
Backend Developer (ASP.NET Core)
📍 Nigeria
