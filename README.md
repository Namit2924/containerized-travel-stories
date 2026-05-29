# 🌍 Containerized Travel Stories MERN Application

A full-stack MERN (MongoDB, Express.js, React.js, Node.js) travel story sharing application containerized using Docker and deployed on AWS ECS Fargate with Amazon ECR.

---

# 🚀 Project Overview

This project allows users to:

* Create travel stories
* Upload travel images
* Edit and delete stories
* Search travel memories
* Authenticate users securely using JWT

The application was containerized using Docker and deployed on AWS cloud infrastructure using ECS Fargate.

---

# 🛠️ Tech Stack

## Frontend

* React.js
* Axios
* Tailwind CSS

## Backend

* Node.js
* Express.js
* JWT Authentication

## Database

* MongoDB Atlas

## Cloud & DevOps

* Docker
* Docker Compose
* Amazon ECS Fargate
* Amazon ECR
* AWS CloudWatch
* GitHub

## Media Storage

* Cloudinary

---

# 🏗️ Architecture

```bash
React Frontend
       ↓
Docker Container
       ↓
Amazon ECS Fargate
       ↓
Node.js Backend Container
       ↓
MongoDB Atlas + Cloudinary
```

---

# 📂 Project Structure

```bash
containerized-travel-stories/
│
├── backend/
│   ├── Dockerfile
│   ├── package.json
│   └── index.js
│
├── frontend/
│   └── travel_stories/
│       ├── Dockerfile
│       ├── src/
│       └── package.json
│
├── docker-compose.yml
├── .gitignore
└── README.md
```

---

# ⚙️ Features

* User Authentication using JWT
* CRUD Operations for Travel Stories
* Image Upload using Cloudinary
* Dockerized Frontend & Backend
* Cloud Deployment using AWS ECS
* MongoDB Atlas Integration
* Responsive UI

---

# 🐳 Docker Setup

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/containerized-travel-stories.git
cd containerized-travel-stories
```

---

# Backend Docker Build

```bash
cd backend
docker build -t travel-backend .
```

---

# Frontend Docker Build

```bash
cd frontend/travel_stories
docker build -t travel-frontend .
```

---

# Run Backend Container

```bash
docker run -p 8000:8000 --env-file .env travel-backend
```

---

# Run Frontend Container

```bash
docker run -p 5173:5173 travel-frontend
```

---

# ☁️ AWS Deployment

## Services Used

* Amazon ECS Fargate
* Amazon ECR
* CloudWatch Logs
* MongoDB Atlas

---

# Deployment Workflow

```bash
Docker Build
     ↓
Push Images to Amazon ECR
     ↓
Create ECS Task Definitions
     ↓
Deploy ECS Services
     ↓
Access Public Application
```

---

# 🔐 Environment Variables

Create a `.env` file inside backend folder:

```env
PORT=8000
MONGO_URI=your_mongodb_uri
ACCESS_TOKEN_SECRET=your_secret_key


```

---

# 📸 Application Screenshots

Add your project screenshots inside:

```bash
Output_image/
```

---

# 📈 Learning Outcomes

Through this project, I learned:

* Docker containerization
* AWS ECS Fargate deployment
* Amazon ECR image management
* Cloud-based MERN deployment
* Environment variable security
* CI/CD deployment concepts
* Cloud networking & security groups

---

# 🧑‍💻 Author

## Namit Dhangar

B.Tech Computer Engineering Student
Interested in DevOps, Cloud Computing, MERN Stack, and Cybersecurity.

---

# ⭐ Future Improvements

* CI/CD using GitHub Actions
* HTTPS with Load Balancer
* Domain Integration
* Auto Scaling
* Kubernetes Deployment
* Monitoring Dashboard

---

# 📜 License

This project is for learning and educational purposes.
