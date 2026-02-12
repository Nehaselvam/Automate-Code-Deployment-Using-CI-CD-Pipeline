🚀 DevOps Internship Task 1
Automate Code Deployment Using CI/CD Pipeline (GitHub Actions)

📌 Project Overview

This project demonstrates how to automate application deployment using a CI/CD pipeline with GitHub Actions and Docker.

The pipeline automatically builds, tests, containerizes, and pushes a Node.js web application to DockerHub whenever code is pushed to the main branch.

🎯 Objective

The goal of this project is to:

Implement Continuous Integration and Continuous Deployment (CI/CD)

Automate application build and deployment process

Containerize a Node.js application using Docker

Push Docker images to DockerHub automatically

Understand DevOps automation workflow

🛠️ Technologies & Tools Used
Tool	Purpose
Node.js	Backend Web Application
Express.js	Web Server Framework
GitHub	Version Control
GitHub Actions	CI/CD Automation
Docker	Containerization
DockerHub	Image Repository

📂 Project Structure
nodejs-demo-app/
│
├── app.js
├── package.json
├── Dockerfile
├── README.md
│
└── .github/
    └── workflows/
        └── main.yml

⚙️ Application Description

This is a simple Node.js Express web application that returns a greeting message when accessed through the browser.

🚀 CI/CD Workflow Explanation

The GitHub Actions workflow performs the following steps:

1️⃣ Trigger Workflow

The pipeline starts automatically when code is pushed to the main branch.

2️⃣ Install Dependencies

Node.js environment is setup

Project dependencies are installed using npm

3️⃣ Run Tests

Placeholder test step to simulate CI validation

4️⃣ Docker Authentication

Logs into DockerHub using GitHub Secrets

5️⃣ Build Docker Image

Creates a container image of the application

6️⃣ Push Image to DockerHub

Uploads built image to DockerHub repository

🔄 Workflow Diagram
Code Push → GitHub Actions → Install Dependencies → Test → Docker Build → Docker Push → Deployment Ready

🐳 Docker Implementation

Docker is used to package the application with all required dependencies.

Dockerfile Explanation

Uses Node.js base image

Sets working directory

Installs dependencies

Copies application code

Exposes port 3000

Starts server

🔐 GitHub Secrets Configuration

Secrets are used to securely store DockerHub credentials.

Required Secrets
Secret Name	Description
DOCKER_USERNAME	DockerHub Username
DOCKER_PASSWORD	DockerHub Access Token
▶️ How To Run Application Locally
Step 1 — Clone Repository
git clone <YOUR_REPO_LINK>
cd nodejs-demo-app

Step 2 — Install Dependencies
npm install

Step 3 — Start Application
npm start

Step 4 — Open Browser
http://localhost:3000

🐳 Run Application Using Docker
Build Docker Image
docker build -t node-demo .

Run Docker Container
docker run -p 3000:3000 node-demo

📌 GitHub Actions Workflow File

Location:

.github/workflows/main.yml


This file defines the automated CI/CD pipeline.

📈 Learning Outcomes

Through this project, I learned:

Fundamentals of CI/CD pipelines

Automating deployment using GitHub Actions

Containerization using Docker

Secure credential management using GitHub Secrets

DevOps workflow automation

❗ Challenges Faced

Understanding workflow syntax

Configuring Docker authentication

Debugging pipeline errors

✅ Solutions Implemented

Used GitHub Actions documentation

Created DockerHub access tokens

Verified pipeline logs for troubleshooting

🔮 Future Improvements

Add automated test cases

Implement deployment to cloud platforms (AWS / Azure)

Add monitoring and logging

Introduce multi-stage Docker builds
