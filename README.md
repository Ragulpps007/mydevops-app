# MyDevOps‑App: Dockerized Web Server Project

**A simple web server containerized using Docker, demonstrating containerization, web hosting, and DevOps fundamentals.**

## 🔎 Project Overview  
This repo contains a minimal static web application (HTML) served via a Docker container. The goal was to practice containerization, Dockerfile configuration, and web service deployment — as a stepping stone for cloud or DevOps‑oriented roles.

## 🛠 Technologies Used  
- Docker  
- HTML (static web content)  
- Linux / shell environment  
- (Optional) Further deploy to AWS / cloud  

## 📦 Build & Run Instructions  

```bash
# Build Docker image  
docker build -t mydevops-app .

# Run container (mapping port 80)  
docker run -d -p 8080:80 --name webapp mydevops-app

# Open browser and visit  
http://localhost:8080
