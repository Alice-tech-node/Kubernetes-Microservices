# Kubernetes Microservices Project (Docker + Kubernetes)
Project Overview

This project demonstrates how to build, containerize, and deploy a microservices-based application using Docker and Kubernetes.

It includes:

A Flask backend API

MongoDB database (optional extension)

Kubernetes deployments and services

🧱 Project Structure

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

 ⚙️ Technologies Used

Docker

Kubernetes

Python (Flask)

MongoDB

Step 1: Build Docker Image

Navigate to backend folder:cd backend

Build image:docker build -t <your-dockerhub-username>/backend:v1 .

Push to Docker Hub:docker push <your-dockerhub-username>/backend:v1

























