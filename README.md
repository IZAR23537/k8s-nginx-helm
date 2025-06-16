# Kubernetes Deployment with Helm: NGINX App

This project demonstrates deploying an NGINX-based web application using Helm charts on a local Minikube cluster.

## Technologies

- Kubernetes (Minikube)
- Helm 3
- NGINX
- NodePort Service

## Project Structure

```
k8s-nginx-helm/
├── charts/
│   └── nginx-app/
│       ├── Chart.yaml
│       ├── values.yaml
│       └── templates/
│           ├── deployment.yaml
│           └── service.yaml
```

## How to Deploy

### 1. Start Minikube

```bash
minikube start
```

### 2. Deploy using Helm

```bash
helm install nginx charts/nginx-app
```

### 3. Access the Service

```bash
minikube service nginx
```

To uninstall:

```bash
helm uninstall nginx
```
