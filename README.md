# Jenkins CI/CD Pipeline

## Project Overview
This project demonstrates a simple CI/CD pipeline using Jenkins, Docker, and GitHub.

## Pipeline Stages

### 1. Build
Jenkins builds a Docker image from the application.

### 2. Test
Jenkins runs the Docker container and verifies the application output.

### 3. Deploy
Jenkins deploys the application by running a Docker container.

## Tools Used
- Jenkins
- Docker
- Git
- GitHub

## Application Output
Hello from Jenkins CI/CD Pipeline

## CI/CD Trigger
Jenkins checks the GitHub repository for new commits using Poll SCM and automatically starts the pipeline when changes are detected.

## Repository
https://github.com/Manoj666333/jenkins-cicd-task
