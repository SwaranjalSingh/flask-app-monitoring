# Flask System Monitoring Dashboard

This project is a simple Flask-based system monitoring dashboard that visualizes CPU and memory usage using Plotly gauge charts. You can run it locally, in Docker, or deploy it on Kubernetes using Minikube.

## 🚀 Features

Real-time CPU and memory usage visualization.

Alerts for high resource usage.

Interactive Plotly gauge charts.

Packaged as a Docker container and deployable to Kubernetes.

## 🧰 Tech Stack

Python (Flask, psutil)

Plotly.js (in HTML)

Docker

Kubernetes

Minikube


## 🔧 Run Locally

### 1. Clone the repository
```bash
git clone https://github.com/swaranjalsingh/flask-app-monitoring.git
cd your-repo-name
```
### 2. Install Python dependencies
```bash
pip install -r requirements.txt
```
### 3. Run the Flask app
```bash
python app.py
```
[Visit : http://localhost:5000/]

## 🐳 Run with Docker
### 1. Build the Docker image
```bash
docker build -t swaranjal/my-flask-app:latest .
```
### 2. Run the container
```bash
docker run -d -p 5000:5000 swaranjal/my-flask-app:latest
```

## ☸️ Deploy on Kubernetes with Minikube
### 1. Start Minikube
```bash
minikube start --driver=docker
```
### 2. Apply deployment and service
```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
### 3. Access the app
```bash
minikube service flask-service --url
```
Open the URL in your browser.

## 📁 Project Structure
├── app.py                 
├── Dockerfile             
├── requirements.txt       
├── templates / index.html         
├── deployment.yaml        
└── service.yaml