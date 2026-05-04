# 🛍️ E-commerce Microservices App  
<img src="https://raw.githubusercontent.com/Walidbadry/Ecommerce-Microservices-React-Node_js/main/terraform/Graphic-01-1024x553.webp" alt="Architecture Diagram" width="1000" height="500">

This project is a **microservices-based e-commerce application** built with **React (frontend), Node.js (backend), and MongoDB**. It is containerized using **Docker** and deployed using **Kubernetes**.  

---

## 📌 Features  
- **Microservices Architecture**: Independent services for **Users, Products, and Orders**.  
- **React Frontend**: A user-friendly UI for interacting with APIs.  
- **API Gateway**: Centralized communication for microservices.  
- **MongoDB Database**: Stores user, product, and order data.  
- **Docker & Kubernetes**: Containerized and orchestrated deployment.  
- **Jenkins CI/CD**: Automates testing, building, and deployment.  

---

## 🏗️ Microservices Overview  
| Service      | Port  | Description |
|-------------|------|-------------|
| **User Service**  | 5003 | Manages users & authentication |
| **Product Service**  | 5001 | Handles product catalog |
| **Order Service**  | 5002 | Manages order processing |
| **Frontend**  | 3000 | React-based UI |
| **API Gateway** | 8080 | Routes requests to microservices |

## 🏗️ ERD digram
<img src="https://github.com/Walidbadry/Ecommerce-Microservices-React-Node_js/blob/main/terraform/images.png" alt="Description" width="500" height = "400">

---

## 🚀 Tech Stack  
- **Frontend:** React, Tailwind CSS  
- **Backend:** Node.js, Express  
- **Database:** MongoDB  
- **DevOps:** Docker, Kubernetes, Jenkins, Nginx  

---

## 🛠️ Installation  

📌 AWS Deployment Architecture
🛠️ AWS Services Used:
✅ EC2 – Hosts Jenkins for CI/CD automation.
✅ EKS (Elastic Kubernetes Service) – Orchestrates microservices.
✅ RDS (Relational Database Service) – Manages the database (e.g., MySQL/PostgreSQL).
✅ ECR (Elastic Container Registry) – Stores Docker images.
✅ S3 – Stores frontend assets and logs.
✅ ALB (Application Load Balancer) – Manages incoming traffic.
✅ Route 53 – Handles domain and DNS.
✅ CloudWatch & Prometheus/Grafana – Monitors logs and performance.
✅ IAM Roles – Manages access control.

📌 Deployment Flow:
1️⃣ Develop & Push Code → GitHub/GitLab
2️⃣ Jenkins CI/CD on AWS EC2

Pulls code

Runs tests, SonarQube analysis

Builds & pushes Docker images to ECR
3️⃣ Deploy to AWS EKS

Kubernetes manages microservices

ALB routes traffic
4️⃣ Monitor & Scale

CloudWatch, Prometheus, Grafana track metrics

Auto Scaling ensures performance
### **1️⃣ Clone the Repository**  
```sh
git clone https://github.com/YOUR-USERNAME/Ecommerce-Microservices.git
cd Ecommerce-Microservices


## 📂 Folder Structure  
```sh
Ecommerce-Microservices/
│── ecommerce-frontend/  # React Frontend
│── product-service/     # Product Microservice
│── order-service/       # Order Microservice
│── user-service/        # User Management Service
│── k8s/                # Kubernetes YAML files
│── Jenkinsfile          # Jenkins pipeline definition
│── README.md            # Project documentation

### **🔹 DevOps & CI/CD**
| Tool | Description |
|------|------------|
| **Jenkins** | Automates CI/CD pipelines for building, testing, and deploying services. |
| **Docker** | Containerizes each microservice to ensure consistency across environments. |
| **Kubernetes** | Manages and orchestrates all microservices. |
| **Helm** | Simplifies Kubernetes deployments using Helm charts. |
| **SonarQube** | Performs code quality and security analysis. |
| **Trivy** | Scans Docker images for vulnerabilities. |
| **Nexus Repository** | Acts as an artifact repository for storing built Docker images. |
| **Prometheus & Grafana** | Monitors system performance and generates real-time dashboards. |

