🚀 Automate Code Deployment Using CI/CD Pipeline
📌 Project Overview

This project demonstrates how to automate the build and deployment process of a Node.js web application using a CI/CD pipeline with GitHub Actions. The pipeline automatically installs dependencies, builds the application, and runs the deployment process whenever changes are pushed to the main branch.

🎯 Objective

To implement Continuous Integration and Continuous Deployment (CI/CD) using GitHub Actions and Docker to streamline the software delivery process and reduce manual intervention.

🛠️ Tools & Technologies Used

Node.js

Express.js

GitHub

GitHub Actions

Docker

DockerHub

⚙️ Workflow Explanation

The CI/CD pipeline performs the following steps automatically:

Triggered when code is pushed to the main branch

Checks out the repository code

Installs project dependencies

Builds the application

Creates a Docker image

Pushes the Docker image to DockerHub
