# Online Boutique — Kubernetes Deployment

## Overview

Online Boutique is a cloud-native demonstration application developed by Google Cloud. It is composed of multiple independent microservices that work together to provide an online shopping application.

For this project, I deployed the application locally on a Kubernetes cluster created with Kind and verified the individual services, Pod states, and frontend access.

## Architecture

The application consists of 11 microservices:

- Ad Service
- Cart Service
- Checkout Service
- Currency Service
- Email Service
- Frontend
- Load Generator
- Payment Service
- Product Catalog Service
- Recommendation Service
- Shipping Service

Redis is also used by the Cart Service.

## Environment

- Kubernetes: Kind
- Container runtime: Docker
- Kubernetes client: kubectl
- Cluster name: `boutique`
- Application source: Google Cloud Online Boutique

## Deployment

### 1. Clone the repository

```bash
cd ~/portfolio-projects
git clone https://github.com/fatimahaneef-tech/microservices-demo.git
cd microservices-demo
