# MyDevOps-App: Dockerized Web Server Project

**A simple web server containerized using Docker, demonstrating containerization, static web hosting, and DevOps fundamentals.**

---

## 🔎 Project Overview  

This repository contains a minimal static web application (HTML) served via a Docker container. The project demonstrates **containerization, Dockerfile configuration, web service deployment, and DevOps best practices**.  

The goal is to showcase practical skills for cloud and DevOps roles.

---

## 🛠 Technologies Used  

- Docker  
- HTML (static web content)  
- Linux / shell commands  
- (Optional) Future deployment to cloud services like AWS EC2 or ECS  

---

## 📦 Build & Run Instructions  

```bash
# 1️⃣ Build Docker image
docker build -t mydevops-app .

# 2️⃣ Run Docker container (maps container port 80 to host port 8080)
docker run -d -p 8080:80 --name webapp mydevops-app

# 3️⃣ Open browser to test
http://localhost:8080
```

---

## 📸 Demo / Output  

![Website Screenshot](screenshorts/demo1.png)  
*(Add more screenshots if needed — place in the `screenshorts` folder)*

When running the container, the static website should display your `index.html` content in the browser at port 8080.

---

## ✅ What this project demonstrates  

- Containerization using Docker  
- Building and running Docker images  
- Static web hosting inside a container  
- Understanding of Dockerfile and container lifecycle  
- Web server setup and port mapping  
- Basics of DevOps workflow for deployment  

---

## 🚀 Future Enhancements  

- Add a dynamic backend (Python / Node.js) inside the container  
- Integrate CI/CD with GitHub Actions for automated builds  
- Deploy to cloud platforms like AWS EC2, ECS, or Kubernetes  
- Enable HTTPS using reverse proxy and SSL certificates  

---

## 📄 License  

MIT License — free to use, modify, and share for learning or demonstration purposes  

---

## 📝 Notes  

- Screenshots are stored in the `screenshorts` folder  
- Ensure Docker is installed locally to build and run the project  
- Port 8080 is used for local access; you can change this in the run command if needed  

