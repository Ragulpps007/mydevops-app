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

✅ What this project demonstrates

1.Containerization using Docker
2.Static web hosting via HTTP server inside container
3.Understanding of Dockerfile and container lifecycle
4.Basics of web serving, port mapping, and container deployment

🚀 Future Enhancements (Planned)

1.Add a dynamic backend (e.g. Python/Node) inside container
2.Configure deployment via CI/CD pipeline (GitHub Actions)
3.Deploy to cloud (AWS EC2 / ECS / EKS) for real-world exposure
4.Add HTTPS support using reverse proxy + SSL
