# Experiment 08 – Kubernetes and Docker Integration

## 1. Check Software Installations

```powershell
docker --version
docker ps
kubectl version --client
kubectl get nodes
```

## 2. Start Docker Desktop

1. Open Docker Desktop.
2. Wait until Docker Engine is running.
3. Make sure Kubernetes is enabled and running.
4. Open VS Code → Terminal → New Terminal.

## 3. Open the Project

1. Open the GitHub repository.
2. Click Code → Download ZIP.
3. Extract the ZIP file.
4. Create a folder using the name given by your faculty.
5. Open the extracted project folder in VS Code.
6. Open Terminal → New Terminal.

## 4. Check Project Files

```powershell
dir
```

Check that these files are available:

- Dockerfile
- index.html
- deployment.yaml
- service.yaml

## 5. Build Docker Image

```powershell
docker build -t varsha0510/kubernetes-docker-task:v1 .
```

Expected output:

```text
Successfully built
Successfully tagged varsha0510/kubernetes-docker-task:v1
```

## 6. Login to Docker Hub

```powershell
docker login
```

Enter your Docker Hub username and password when prompted.

## 7. Push Docker Image to Docker Hub

```powershell
docker push varsha0510/kubernetes-docker-task:v1
```

This makes the image available for Kubernetes to pull.

## 8. Verify Docker Image

```powershell
docker images
```

Check that the image is available:

```text
varsha0510/kubernetes-docker-task
```

## 
