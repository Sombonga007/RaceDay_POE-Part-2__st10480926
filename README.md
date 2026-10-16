# RaceDay_POE-Part-2__st10480926
# RaceDay – Part 2

## Project Overview

RaceDay is an event management API developed for the PROG6212 Portfolio of Evidence. It supports user accounts, event management, categories, participant enrolments and race results.

## Technologies

- C#
- ASP.NET Core Web API
- .NET 8
- Entity Framework Core
- SQL Server LocalDB
- Swagger / OpenAPI
- xUnit
- GitHub Actions

## Main Features

- User registration and login
- Profile retrieval and updating
- Event listing and event management
- Event category management
- Participant enrolments
- Race result recording and retrieval
- Automated authentication service tests
- Automated build and test workflow

## Project Structure

- `RaceDay.Api/Controllers` – API endpoints
- `RaceDay.Api/Data` – Entity Framework database context
- `RaceDay.Api/DTOs` – request data transfer objects
- `RaceDay.Api/Models` – system entities
- `RaceDay.Api/Services` – authentication business logic
- `RaceDay.Tests` – automated tests
- `.github/workflows` – GitHub Actions configuration

## Requirements

Install the .NET 8 SDK and SQL Server LocalDB. Open the solution in Visual Studio or use the .NET CLI.

## Database Setup

From the solution directory, install the Entity Framework CLI tool if necessary:

```bash
dotnet tool install --global dotnet-ef
```

Create and apply the database migration:

```bash
dotnet ef migrations add InitialCreate --project RaceDay.Api
dotnet ef database update --project RaceDay.Api
```

## Run the API

```bash
dotnet run --project RaceDay.Api
```

Open the Swagger URL printed in the terminal and add `/swagger` if required.

## Run the Tests

```bash
dotnet test RaceDay.Tests/RaceDay.Tests.csproj
```

## Notes

The project must be tested locally before submission. Database models and API routes must be checked against the approved Part 1 ERD, SQL schema and API Endpoint Plan. Add sample data and further tests where required by the assignment rubric.

## AI Assistance Disclosure

If AI assistance was used, disclose it in accordance with the lecturer's instructions and the institution's academic integrity policy. Review, understand, test and adapt all generated code before submitting it.
