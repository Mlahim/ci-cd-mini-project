# Scientific Calculator - CI/CD DevOps Project

## Overview

This project is a Dockerized Scientific Calculator built using HTML, CSS, and JavaScript. The primary goal of this project was not only to create a calculator application but also to demonstrate practical DevOps skills by implementing a complete CI/CD pipeline using GitHub Actions, Docker Hub, and Render.

## Features

* Basic arithmetic operations
* Square root calculation
* Square calculation
* Trigonometric functions (sin, cos)
* Responsive user interface
* Docker containerization
* Automated CI/CD workflow

## Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript

### DevOps

* Git & GitHub
* GitHub Actions
* Docker
* Docker Hub
* Render

## CI Pipeline

The Continuous Integration pipeline performs the following tasks:

1. Triggered on Pull Requests to the main branch.
2. Checks out the repository code.
3. Builds a Docker image.
4. Verifies successful image creation.
5. Pushes the Docker image to Docker Hub.

## CD Pipeline

The Continuous Deployment pipeline performs the following tasks:

1. Triggered on pushes to the main branch.
2. Calls the Render Deploy Hook.
3. Automatically deploys the latest Docker image.
4. Updates the live application without manual intervention.

## Docker

Build the image locally:

```bash
docker build -t calculator .
```

Run the container:

```bash
docker run -d -p 8080:80 calculator
```

## Project Structure

```text
scientific-calculator/
│
├── index.html
├── style.css
├── script.js
│
├── Dockerfile
├── README.md
│
└── .github/
    └── workflows/
        ├── ci.yaml
        └── cd.yaml
```

## DevOps Skills Demonstrated

* Git Branching Strategy
* Pull Request Based Development
* Continuous Integration (CI)
* Continuous Deployment (CD)
* Docker Image Creation
* Docker Registry Integration
* GitHub Actions Automation
* Deployment Automation
* Infrastructure as Code Concepts
* Cloud Deployment on Render

## Learning Outcomes

Through this project, I gained hands-on experience with:

* Building automated CI/CD pipelines
* Managing Docker images and registries
* Working with GitHub Actions workflows
* Deploying containerized applications
* Automating deployments using webhooks
* Implementing DevOps best practices

## Author

Muhammad Mlahim

