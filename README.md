AirMode-play

Project Overview

AirMode-play is an ASP.NET Core Web API built using Visual Studio Code and .NET 10.

This project demonstrates a complete CI/CD implementation using:

ASP.NET Core Web API
Visual Studio Code
GitHub
GitHub Actions
Azure App Service
Azure Deployment using Publish Profile

The CI/CD pipeline automatically:

Restores NuGet dependencies
Builds the application
Runs automated tests
Publishes application artifacts
Deploys to Azure App Service

Technologies Used
| Technology           | Purpose                 |
| -------------------- | ----------------------- |
| ASP.NET Core Web API | Backend API             |
| .NET 10              | Application Framework   |
| Visual Studio Code   | Development Environment |
| Git & GitHub         | Source Control          |
| GitHub Actions       | CI/CD Automation        |
| Azure App Service    | Application Hosting     |


Architecture

Developer (VS Code)
│
▼
GitHub Repository
(AirMode-play)
│
▼
GitHub Actions
│
├── Restore
├── Build
├── Test
├── Publish
└── Deploy
│
▼
Azure App Service
(Myfirstw)

Project Structure

AirMode-play
│
├── .github
│ └── workflows
│ └── CI-CD.yml
│
├── Properties
│ └── launchSettings.json
│
├── Program.cs
├── appsettings.json
├── AirMode-play.csproj
│
└── README.md

CI/CD Pipeline
The GitHub Actions pipeline performs:

Restore NuGet packages
Build application
Execute tests
Publish artifacts
Deploy to Azure App Service

GitHub Actions File

Workflow
Workflow file:

.github/workflows/CI-CD.yml
on:
  push:
    branches:
      - main

Local Execution

Running Locally
dotnet restore
dotnet build
dotnet run

Skills Demonstrated

ASP.NET Core Development
GitHub Actions
Continuous Integration
Continuous Deployment
Azure App Service
Git Version Control
Cloud Deployment
