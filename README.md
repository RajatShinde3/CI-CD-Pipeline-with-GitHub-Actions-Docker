# CI/CD Pipeline with GitHub Actions & Docker 🐳🚀

This project demonstrates how to build a lightweight CI/CD pipeline using **GitHub Actions** and **Docker** to automatically build, test, and manage a containerized Flask application.

## 🛠 Tech Stack

- 🐍 Python (Flask)
- 🐳 Docker & Docker Compose
- ⚙️ GitHub Actions
- 🧪 Basic Testing (pytest)
- 📁 Makefile for simplified commands

---

## 🚀 Features

- ✅ GitHub Actions CI pipeline
- ✅ Dockerized Flask app
- ✅ Multi-stage Docker build
- ✅ Automated testing
- ✅ Linting support
- ✅ Version-controlled commits (30+ commits simulating real DevOps workflows)

---

## 📂 Project Structure

├── app/ # Flask application
│ ├── app.py # Main app logic
│ └── tests/ # Unit tests
├── .github/workflows/ # GitHub Actions CI config
│ └── ci.yml
├── docker-compose.yml # Docker container configuration
├── docker-compose.dev.yml # Dev environment override
├── Makefile # Helper commands
├── README.md # This file
└── LICENSE


---

## ⚙️ CI/CD Workflow (GitHub Actions)

The `ci.yml` file in `.github/workflows/` triggers on:

- Push to `main` branch
- Pull requests to `main`

Workflow steps:

1. **Checkout code**
2. **Build Docker image**
3. **Run lint/test commands**
4. (Optional) Push to container registry or deploy

---

## ▶️ How to Run Locally

### 🔧 Prerequisites
- Docker & Docker Compose
- Git

### 🧪 Run the app locally:
```bash
# Clone the repo
git clone https://github.com/RajatShinde3/CI-CD-Pipeline-with-GitHub-Actions-Docker.git
cd CI-CD-Pipeline-with-GitHub-Actions-Docker

# Run app using Docker Compose
docker-compose up --build
