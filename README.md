# 🐳 Classroom-cicd-kubernetes

## 📌 Prerequisites

Before you start, ensure you have the following installed:

- **Minikube** 🏗️ ([Installation Guide](https://minikube.sigs.k8s.io/docs/start/))
- **kubectl** 🖥️ ([Install kubectl](https://kubernetes.io/docs/tasks/tools/))
- **Docker** 🐳 ([Download Docker](https://www.docker.com/products/docker-desktop))
- **Git** 🌱 ([Download Git](https://git-scm.com/downloads))
- **Helm** ⛵ ([Install Helm](https://helm.sh/docs/intro/install/))

## 🚀 Setup & Deployment

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/WhiteboxHub/classroom-cicd-kubernetes.git
cd classroom-cicd-kubernetes
```

### 2️⃣ Start Minikube
```sh
minikube start
```

### 3️⃣ Enable Minikube Add-ons (Optional)
```sh
minikube addons enable ingress
```

### 4️⃣ Apply Kubernetes Configurations
```sh
kubectl apply -f configmap.yaml
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```

### 5️⃣ Verify Deployments & Services
```sh
kubectl get pods
kubectl get services
```

### 6️⃣ Access Application
```sh
minikube service <your-service-name> --url
```

