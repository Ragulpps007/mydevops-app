# MyDevOps-App: Dockerized Web Server Project

**A simple web server containerized using Docker, demonstrating containerization, static web hosting, DevOps fundamentals, and AWS ECS deployment.**

---

## 🔎 Project Overview  

This repository contains a minimal static web application (HTML) served via a Docker container. The project demonstrates **containerization, Dockerfile configuration, web service deployment, and DevOps best practices**, with optional deployment on **AWS ECS**.  

The goal is to showcase practical skills for **cloud, containerization, and DevOps roles**.

---

## 🛠 Technologies Used  

- Docker  
- HTML (static web content)  
- Linux / shell commands  
- AWS ECS (Elastic Container Service)  
- (Optional) Future integration with CI/CD pipelines  

---

## 📦 Build & Run Instructions  

### Local Docker

```bash
# 1️⃣ Build Docker image
docker build -t mydevops-app .

# 2️⃣ Run Docker container (maps container port 80 to host port 8080)
docker run -d -p 8080:80 --name webapp mydevops-app

# 3️⃣ Open browser to test
http://localhost:8080
```

### Deploy on AWS ECS (Optional)

1. Push Docker image to **Amazon ECR** (Elastic Container Registry)  
2. Create **ECS Cluster** using Fargate or EC2 launch type  
3. Define **Task Definition** pointing to your ECR image  
4. Create a **Service** with desired number of tasks  
5. Assign **Security Group** to allow inbound HTTP (80)  
6. Access your application via **Load Balancer** or ECS public endpoint  

---

## ✅ What this project demonstrates  

- Containerization using Docker  
- Building and running Docker images locally  
- Static web hosting inside a container  
- Deployment to **AWS ECS** (cloud container service)  
- Understanding of Dockerfile, container lifecycle, and task definitions  
- Web server setup and port mapping  
- Basics of DevOps workflow for deployment  

---

## 🚀 Future Enhancements  

- Add a dynamic backend (Python / Node.js) inside the container  
- Integrate CI/CD with **GitHub Actions** for automated builds and ECS deployment  
- Enable HTTPS using reverse proxy and SSL certificates  
- Auto-scaling and monitoring using **CloudWatch**  

---

## 📄 License  

MIT License — free to use, modify, and share for learning or demonstration purposes  

---

## 📝 Notes  

- Screenshots are stored in the `screenshort` folder  
- Ensure Docker is installed locally to build and run the project  
- Port 8080 is used for local access; you can change this in the run command if needed  
- ECS deployment requires AWS account with IAM permissions for ECR, ECS, and optionally CloudWatch
