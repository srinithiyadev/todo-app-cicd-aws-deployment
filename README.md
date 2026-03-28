# Flask To-Do Application with CI/CD Pipeline

## Overview

This project is a Flask-based To-Do web application integrated with an end-to-end CI/CD pipeline. The application allows users to manage tasks with basic CRUD operations. The deployment process is fully automated using Jenkins and Docker, and the application is hosted on AWS EC2.

## Tech Stack

* Backend: Flask (Python)
* Database: SQLite
* CI/CD: Jenkins
* Containerization: Docker
* Cloud Platform: AWS EC2
* Container Registry: DockerHub

## Features

* Add tasks
* Update task status
* Delete tasks
* Persistent storage using SQLite
* Containerized application
* Automated build and deployment pipeline

## CI/CD Workflow

The application follows a continuous integration and continuous deployment pipeline:

1. Code is pushed to GitHub
2. Jenkins triggers the pipeline
3. Docker image is built
4. Image is pushed to DockerHub
5. Jenkins deploys the latest image to AWS EC2
6. Application runs inside a Docker container

## Deployment

The application is deployed on an AWS EC2 instance using Docker.

Live URL:
http://44.201.230.113:5000

## Docker Commands

To build and run locally:

docker build -t todo-app .
docker run -d -p 5000:5000 todo-app

## Key Learnings

* Implemented a complete CI/CD pipeline using Jenkins
* Automated deployment to a cloud environment
* Worked with Docker for containerization
* Managed real-world deployment issues such as permissions, port conflicts, and remote execution

## Author

Srinithiya
