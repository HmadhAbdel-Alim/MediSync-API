# 🏥 MediSync - Healthcare & Prescription Management API

An enterprise-grade RESTful Web API built with **ASP.NET Core**, strictly adhering to **Clean Architecture** principles to manage healthcare appointments, patients, prescriptions, and automated reminder scheduling.

---

## 🏗️ Architecture & How It Works

The solution is divided into distinct decoupled layers to enforce **Separation of Concerns (SoC)** and maintainability:

```text
├── API (Controllers, Middlewares, Program.cs)
├── Application (Services, DTOs, Interfaces, Validators)
├── Core / Domain (Entities, Enums, Core Business Logic)
└── Infrastructure (Data Context, Repositories, EF Core Migrations)
Key Modules & Workflow:
Core Architecture: Built using Clean Architecture, separating Domain, Application, Infrastructure, and Presentation layers.

Prescription & Reminders: Manages prescription items, tracks daily dose schedules, and handles automated reminder notifications.

Doctor Appointments & Booking: Handles patient appointment booking, scheduling, and status tracking with strong data validation.

Data Validation & DTOs: Implements strongly-typed request/response models with clean data mapping.

Security & Authentication: Secure endpoints protected using JWT authentication and ASP.NET Core Identity.

Global Error Handling: Centralized custom middleware for catching unhandled exceptions and standardizing API JSON error responses.

🛠️ Tech Stack & Design Patterns
Framework: .NET / ASP.NET Core Web API

Database & ORM: SQL Server, Entity Framework Core (Code First), Relational database mapping with foreign key constraints

Architecture & Patterns: Clean Architecture, Repository Pattern, Dependency Injection

Version Control: Git & GitHub

⚙️ How to Setup & Run
Clone the Repository:

Bash
git clone [https://github.com/HmadhAbdel-Alim/MediSync-API.git](https://github.com/HmadhAbdel-Alim/MediSync-API.git)
cd MediSync-API
Configure App Settings:
Update your SQL Server connection string in appsettings.json inside the MediSync.API project layer.

Update Database (Run Migrations):

Bash
dotnet ef database update --project MediSync.Infrastructure --startup-project MediSync.API
Run the Application:

Bash
dotnet run --project MediSync.API
👨‍💻 Developer
Hmadh Abdel-Alim Hmad

Junior .NET Backend Developer

LinkedIn Profile | GitHub Profile
