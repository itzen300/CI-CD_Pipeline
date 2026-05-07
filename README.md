# Cloud Project
#  CI/CD Pipeline for Two-Tier Flask Application

This project demonstrates the implementation of a complete CI/CD (Continuous Integration and Continuous Deployment) pipeline for a two-tier web application using Flask and MySQL. The infrastructure is automated using Jenkins, Docker, and Docker Compose while being deployed on AWS EC2 cloud infrastructure.

The project was created to gain practical exposure to real-world DevOps workflows including source code management, automated deployment pipelines, containerization, infrastructure provisioning, and deployment automation.

#  Project Architecture is :-

```text
Developer
   │
   ▼
GitHub Repository
   │
   ▼
Jenkins Pipeline
   │
   ├── Clone Source Code
   ├── Build Docker Image
   ├── Deploy Containers
   ▼
Docker Compose
   │
   ├── Flask Container
   └── MySQL Container
   ▼
AWS EC2 Instance
```

# ⚙️ Technologies Used

| Technology     | Purpose                    |
| -------------- | -------------------------- |
| Python Flask   | Backend Web Application    |
| MySQL          | Database Layer             |
| GitHub         | Source Code Management     |
| Jenkins        | CI/CD Automation           |
| Docker         | Containerization           |
| Docker Compose | Multi-Container Management |
| AWS EC2        | Cloud Infrastructure       |
| Ubuntu Server  | Operating System           |



##  Source Code Management are :-

The application source code is stored and managed using GitHub. Developers push updated code to the repository, which acts as the centralized source of truth.


## Jenkins Pipeline Automation are :-

Jenkins is used as the automation engine responsible for:

* Pulling latest source code
* Building Docker images
* Deploying application containers
* Automating deployment workflow


# Docker Containerization are :-

Docker is used to package the Flask application and its dependencies into portable containers. This ensures that the application behaves consistently across development and deployment environments.

### Docker Benefits

* Environment consistency
* Application isolation
* Fast deployment
* Simplified dependency management
* Portability across systems


#  Deployment Workflow are :-

The deployment process follows an automated workflow:

1. Developer pushes code to GitHub
2. Jenkins detects repository changes
3. Jenkins pipeline executes automatically
4. Docker image is built
5. Existing containers are stopped
6. Updated containers are deployed
7. Application becomes publicly accessible

This workflow eliminates manual deployment effort and ensures faster delivery cycles.


#  Security Group Configuration :-

The AWS EC2 instance was configured with the following inbound rules:

| Port | Purpose           |
| ---- | ----------------- |
| 22   | SSH Access        |
| 5000 | Flask Application |
| 8080 | Jenkins Dashboard |

Security groups help control inbound and outbound network traffic within the cloud infrastructure.


# My Practical Learning Outcomes :-

This project helped in understanding:

* CI/CD pipeline implementation
* Jenkins automation workflows
* Docker containerization concepts
* Multi-container orchestration
* Cloud deployment using AWS
* Infrastructure provisioning
* Deployment automation
* DevOps workflow management


#  Future Improvements which can be appended are :-

Potential enhancements planned for this project:
* Kubernetes Integration
* Prometheus Monitoring
* Grafana Dashboards
* Docker Registry Integration
* Automated Testing Stages
* Blue-Green Deployment
* Infrastructure as Code (Terraform)
* Security Scanning

* Containerization technologies
* Deployment orchestration

It serves as a strong foundational DevOps project showcasing both theoretical understanding and practical implementation skills in modern infrastructure automation environments.
