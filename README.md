Devops Project# ☕ Azure Java Web App CI/CD

> Build, test, package and deploy a Java Web Application to Azure App Service using Azure DevOps CI/CD Pipelines.

![Java](https://img.shields.io/badge/Java-17-orange)
![Maven](https://img.shields.io/badge/Maven-Build-red)
![Azure](https://img.shields.io/badge/Azure-App%20Service-blue)
![Azure DevOps](https://img.shields.io/badge/Azure%20DevOps-CI%2FCD-blue)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black)
![License](https://img.shields.io/badge/License-MIT-green)

---

# 📖 Project Overview

This project demonstrates a complete Continuous Integration and Continuous Deployment (CI/CD) pipeline for a Java Web Application using **Azure DevOps**.

The pipeline automatically:

- Builds the application using Maven
- Executes JUnit tests
- Packages the application into a WAR file
- Publishes the WAR as a Pipeline Artifact
- Deploys the application to Azure App Service (Linux)

This project forms part of a complete DevOps portfolio alongside the **terraform-azure-webapp** repository, where the Azure infrastructure is provisioned using Terraform.

---

# 🏗️ Architecture Diagram

![Architecture](azure-java-webapp-ci-cd.png)

---

# 🚀 CI/CD Pipeline

The Azure DevOps pipeline consists of two stages.

## Stage 1 – Build

✔ Checkout Source Code

✔ Build using Maven

✔ Run Unit Tests

✔ Generate WAR Package

✔ Publish Pipeline Artifact

---

## Stage 2 – Deploy

✔ Download Pipeline Artifact

✔ Deploy WAR to Azure Linux Web App

✔ Verify Successful Deployment

---

# ☁️ Azure Resources

The application is deployed to the following Azure resources:

- Azure Resource Group
- Azure App Service Plan (Linux)
- Azure Linux Web App
- Azure Resource Manager Service Connection

---

# 📁 Repository Structure

```text
azure-java-webapp-ci-cd
│
├── server/
├── webapp/
├── pom.xml
├── azure-pipelines.yml
├── Dockerfile
├── AzureDockerfile
├── README.md
└── architecture.png
```

---

# ⚙️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Java 17 | Programming Language |
| Maven | Build Tool |
| JUnit | Unit Testing |
| Azure DevOps | CI/CD Pipeline |
| Azure App Service | Application Hosting |
| GitHub | Source Control |
| Linux App Service | Runtime Environment |

---

# 🔄 Pipeline Workflow

```text
Developer
     │
     ▼
GitHub Repository
     │
     ▼
Azure DevOps Pipeline
     │
     ▼
Build
     │
     ▼
Unit Tests
     │
     ▼
Package WAR
     │
     ▼
Publish Pipeline Artifact
     │
     ▼
Deploy
     │
     ▼
Azure App Service (Linux)
     │
     ▼
Running Java Application
```

---

# 📸 Screenshots

## Azure DevOps Pipeline

> *(Add a screenshot of the successful Build and Deploy pipeline here.)*

```
images/pipeline-success.png
```

---

## Azure App Service

> *(Add a screenshot of the Azure Web App Overview page.)*

```
images/azure-webapp.png
```

---

## Running Application

> *(Add a screenshot showing the deployed Java application.)*

```
images/running-application.png
```

---

# ▶️ Running Locally

Clone the repository

```bash
git clone https://github.com/blueberry247/azure-java-webapp-ci-cd.git
```

Navigate to the project

```bash
cd azure-java-webapp-ci-cd
```

Build the application

```bash
mvn clean package
```

Run locally (if supported)

```bash
mvn tomcat7:run
```

---

# ☁️ Azure Deployment

Deployment is fully automated using Azure DevOps.

Every push to the **master** branch automatically:

- Builds the application
- Executes unit tests
- Packages the WAR file
- Publishes the artifact
- Deploys the application to Azure App Service

---

# 📌 Related Project

Infrastructure for this application is provisioned using Terraform.

Repository:

➡️ **terraform-azure-webapp**

This repository contains:

- Azure Resource Group
- Azure App Service Plan
- Azure Linux Web App
- Azure DevOps Infrastructure Pipeline

---

# 👨‍💻 Author

**Mohammed Farooq**

Infrastructure Engineer | Azure | Terraform | Azure DevOps | CI/CD | Java

GitHub:

https://github.com/blueberry247

---

# ⭐ Future Improvements

- Azure Key Vault integration
- Terraform Remote State
- Deployment Slots
- Approval Gates
- SonarQube Code Analysis
- OWASP Dependency Scanning
- Docker Container Deployment
- AKS Deployment
- Monitoring with Azure Application Insights

---

# 📜 License

This project is licensed under the MIT License.
