# SK Trading Kubernetes Deployment

This repository contains the SK Trading application deployed on Kubernetes using Docker Desktop.

## Project Files

- `Dockerfile` — Docker image for SK Trading app
- `index.html` — Main page of the app
- `deployment.yaml` — Kubernetes Deployment with resources and HPA
- `components.yaml` — Optional Kubernetes components (services, configmaps, etc.)

## Steps Performed

1. Built Docker image for SK Trading:
   ```bash
   docker build -t sktrading:v1 .
