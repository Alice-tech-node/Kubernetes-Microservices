# Kubernetes Microservices Project (Docker + Kubernetes)
Project Overview

This project demonstrates how to build, containerize, and deploy a microservices-based application using Docker and Kubernetes.

It includes:

A Flask backend API

MongoDB database (optional extension)

Kubernetes deployments and services


# 🧱 Project Structure

k8s-microservices/

 ├── backend/
 
 │    ├── app.py
 
 │    ├── requirements.txt
 
 │    └── Dockerfile
 
 ├── k8s/
 
 │    ├── backend-deployment.yaml
 
 │    ├── backend-service.yaml
 
 │    └── mongo.yaml
 
 └── README.md

 

 # ⚙️ Technologies Used

  Docker

  Kubernetes

  Python (Flask)

  MongoDB

  

# Step 1: Build Docker Image

 Navigate to backend folder: cd backend

 Build image: docker build -t <your-dockerhub-username>/backend:v1 .

 Push to Docker Hub: docker push <your-dockerhub-username>/backend:v1


# Step 2: Deploy to Kubernetes

Apply deployment: kubectl apply -f k8s/backend-deployment.yaml

Apply service: kubectl apply -f k8s/backend-service.yaml

Check resources:    kubectl get pods

                    kubectl get svc


# Step 3: Access the Application

Find NodePort: kubectl get svc backend-service

Access in browser: http://<NODE-IP>:<NODE-PORT>

# Step 4: Deploy MongoDB

kubectl apply -f k8s/mongo.yaml

# 📈 Features

Containerized backend using Docker

Scalable deployment using Kubernetes

Service exposure via NodePort

Modular microservices structure


# 🧠 Key Learnings

How to build and push Docker images

Kubernetes Deployments and Services

Container orchestration basics

Microservices architecture

# 🚀 Future Improvements

Add frontend (React)

Implement CI/CD pipeline

Add Ingress controller

Add monitoring (Prometheus & Grafana)


# 👩‍💻 Author

Alice S.





















