# NotificationsWithDI
NotificationsWithDI API built using ASP.NET Core (.NET 8) demonstrating clean architecture with Dependency Injection (DI), Repository Pattern, and Entity Framework Core.
This project sends Email and SMS notifications and stores them in a SQL Server database using a fully layered structure:

Controllers → Handle API requests

Services (Business Layer) → Send notifications

Repositories (Data Access Layer) → Perform DB operations

EF Core DbContext → Connects to SQL Server

Dependency Injection (DI) is implemented across the entire application for clean separation of concerns and testability:

INotificationService → injected into the Controller

INotificationRepository → injected into the Service

AppDbContext → injected into the Repository

IMessageService → injected as an example of DI usage

Includes Swagger support, async programming, clean folder structure, and real-world API design principles.
