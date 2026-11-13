# BLOGged: ASP.NET Core Blog API (Starter)

A planned blog backend built with **ASP.NET Core Web API on .NET 6**.

> **Status: early starter, not built yet (August 2023).**
> The repo has only the default project setup from the .NET Web API template. It has no controllers, models or database yet, so the API has no endpoints.

---

## What's Included

- An ASP.NET Core Web API project that targets **.NET 6**
- **Swagger / OpenAPI** set up with Swashbuckle. The Swagger UI opens automatically in Development mode.
- HTTPS redirection and the authorization middleware are turned on
- Controller routing is ready (`MapControllers`), but there are no controllers yet

---

## Tech Stack

| Part        | Technology                         |
|-------------|------------------------------------|
| Framework   | ASP.NET Core Web API (.NET 6, C#)  |
| API docs    | Swashbuckle.AspNetCore 6.2.3 (Swagger) |

---

## Project Structure

```
BLOGged/
├── BLOGged.sln                      # Visual Studio solution
└── BLOGged/
    ├── BLOGged.csproj               # Project file (.NET 6, Swashbuckle)
    ├── Program.cs                   # App startup and middleware
    ├── appsettings.json             # Logging and allowed hosts
    ├── appsettings.Development.json
    └── Properties/
        └── launchSettings.json      # Local URLs and launch profiles
```

---

## Running Locally

You need the [.NET 6 SDK](https://dotnet.microsoft.com/download/dotnet/6.0) or newer.

```bash
git clone https://github.com/AhnafIfti/BLOGged.git
cd BLOGged/BLOGged
dotnet run
```

Then open https://localhost:7288/swagger. The Swagger page will load, but it will show no endpoints yet.

You can also open `BLOGged.sln` in Visual Studio and press **F5**.

---

## Planned Next Steps

- Add `Blog`, `User` and `Comment` models
- Add a database with Entity Framework Core
- Add controllers for blog and user CRUD
- Add authentication (for example, JWT)
