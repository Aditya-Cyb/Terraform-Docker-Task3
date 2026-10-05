# Task 3 – Infrastructure as Code (IaC) with Terraform

## 📌 Objective

The objective of this task is to provision a local Docker container using **Terraform** and understand the basic Infrastructure as Code (IaC) workflow.

Terraform was used to:

- Provision a Docker image
- Create a Docker container
- Verify the deployed container
- Track infrastructure using Terraform state
- Destroy the provisioned infrastructure

---

## 🛠️ Tools and Technologies Used

- **Terraform v1.16.1**
- **Docker v28.3.3**
- **Docker Provider:** `kreuzwerker/docker v4.6.0`
- **Docker Image:** `nginx:latest`
- **Git & GitHub**
- **Git Bash**
- **Windows**

---

## 🏗️ Project Architecture

```text
Terraform
    │
    ▼
Docker Provider
    │
    ├── Pull nginx:latest
    │
    ▼
Docker Container
    │
    └── terraform-nginx
            │
            ▼
     localhost:8080
