# Introduction
In modern cloud-based application deployment, containerization and orchestration tools like Docker and Kubernetes are essential for ensuring scalability, portability, and efficient resource management. This lab report outlines the process of deploying a Maven web application on Google Cloud Platform (GCP) using Google Kubernetes Engine (GKE), highlighting the integration of Docker for containerization and Kubernetes for orchestration. 

# GitHub Repository
https://github.com/jb-cheng/BinaryCalculatorGCPApp

# Video
[Omitted from GitHub]

# Discussion
[Omitted from GitHub]


# Design

See `.yaml` files.


# Deployment Instructions
```
docker build -t northamerica-northeast2-docker.pkg.dev/axial-diagram-451822-g1/sofe3980u/binarycalculatorwebapp .
```

```
docker push northamerica-northeast2-docker.pkg.dev/axial-diagram-451822-g1/sofe3980u/binarycalculatorwebapp
```

```
kubectl create -f binarycalculatorwebapp-deploy.yaml
```

```
kubectl create -f binarycalculatorwebapp-service.yaml
```