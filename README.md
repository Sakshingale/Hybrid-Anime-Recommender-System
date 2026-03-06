# 🎌 Hybrid Anime Recommender System – End-to-End MLOps Pipeline

An **end-to-end Hybrid Anime Recommendation System** that combines **content-based filtering and collaborative filtering** to generate personalized anime recommendations.

This project demonstrates a **production-ready MLOps workflow**, integrating **data versioning, experiment tracking, CI/CD automation, containerization, and Kubernetes deployment**.

The system is designed to showcase **scalable machine learning infrastructure** using modern DevOps and cloud-native technologies.

---

# 🚀 Tech Stack

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-Orchestration-blue)
![Jenkins](https://img.shields.io/badge/Jenkins-CI/CD-red)
![DVC](https://img.shields.io/badge/DVC-Data%20Versioning-orange)
![CometML](https://img.shields.io/badge/CometML-Experiment%20Tracking-blue)
![Flask](https://img.shields.io/badge/Flask-Web%20Application-black)
![GCP](https://img.shields.io/badge/GCP-Cloud%20Platform-yellow)
![License](https://img.shields.io/badge/License-GPL--3.0-green)

---

# 📌 Project Overview

This project implements a **Hybrid Recommendation System** that improves recommendation accuracy by combining two popular approaches:

### 🔹 Content-Based Filtering

Recommends anime based on **similar attributes such as genre, type, and features**.

### 🔹 Collaborative Filtering

Recommends anime based on **user behavior, ratings, and similarities between users**.

The hybrid approach helps overcome limitations of individual methods and produces **more personalized recommendations**.

---

# 🏗 System Architecture

The project follows a **modern MLOps architecture** where machine learning pipelines are automated and deployed through containerized infrastructure.

### Workflow

1. Developer pushes code to **GitHub**
2. **Jenkins CI/CD pipeline** is triggered
3. **DVC** manages dataset and model versioning
4. **Comet-ML** tracks training experiments
5. **Docker** builds container images
6. Images are deployed to **Kubernetes (GKE / Minikube)**
7. **Flask web application** serves recommendations to users

```
Developer
   │
   ▼
GitHub Repository
   │
   ▼
Jenkins CI/CD Pipeline
   │
   ├── DVC Data Pull
   ├── Run ML Pipeline
   ├── Build Docker Image
   └── Deploy to Kubernetes
   │
   ▼
Kubernetes Cluster
   │
   ├── Recommendation API
   ├── Flask Web Application
   └── Model Serving
   │
   ▼
Comet ML Experiment Tracking
```

---

# 🤖 Machine Learning Pipeline

The recommendation model pipeline includes several automated stages.

```
Raw Dataset
   │
   ▼
Data Ingestion
   │
   ▼
Data Preprocessing
   │
   ▼
Feature Engineering
   │
   ▼
Content-Based Filtering Model
   │
   ▼
Collaborative Filtering Model
   │
   ▼
Hybrid Recommendation Model
   │
   ▼
Model Evaluation
   │
   ▼
Experiment Tracking (Comet ML)
   │
   ▼
Model Packaging (Docker)
   │
   ▼
Deployment (Kubernetes)
```

---

# 🔄 CI/CD Pipeline

The **CI/CD pipeline** automates the complete ML workflow.

### Pipeline Stages

* Pull latest code from repository
* Retrieve datasets using **DVC**
* Install dependencies
* Train recommendation models
* Track experiments with **Comet-ML**
* Build Docker container
* Push container image
* Deploy to Kubernetes cluster

This ensures **continuous integration, reproducibility, and scalable deployments**.

---

# 📊 Data Versioning with DVC

**DVC (Data Version Control)** is used to manage datasets and model artifacts.

Benefits:

* Version control for datasets
* Reproducible ML experiments
* Large file tracking outside Git
* Data pipeline automation

---

# 🌐 Web Application

A **Flask-based web interface** allows users to interact with the recommendation system.

Features:

* User input for anime preferences
* Real-time recommendations
* Integration with trained ML models
* REST API for prediction requests

---

# 📁 Project Structure

```
Hybrid-Anime-Recommender-System
│
├── .dvc/                 # Data versioning configuration
├── artifacts/            # Processed datasets and model outputs
├── config/               # Configuration files
├── custom_jenkins/       # Jenkins configuration
├── notebook/             # Data exploration notebooks
├── pipeline/             # ML pipeline scripts
├── src/                  # Model training and recommendation logic
├── static/               # Static assets for Flask app
├── templates/            # HTML templates for UI
├── utils/                # Utility functions
│
├── application.py        # Flask application
├── tester.py             # Testing and prediction scripts
├── Dockerfile            # Docker container configuration
├── Jenkinsfile           # CI/CD pipeline definition
├── deployment.yaml       # Kubernetes deployment configuration
├── requirements.txt      # Python dependencies
└── README.md
```

---

# 🧠 Skills Demonstrated

This project demonstrates practical experience with **real-world MLOps systems**.

* Hybrid **Recommendation System Design**
* **Content-Based & Collaborative Filtering**
* **Data Versioning using DVC**
* **Experiment Tracking with Comet-ML**
* **CI/CD Automation using Jenkins**
* **Docker Containerization**
* **Kubernetes Deployment**
* **Flask API Development**
* **Scalable ML Infrastructure**

---

# 📜 License

This project is licensed under the **GPL-3.0 License**.

