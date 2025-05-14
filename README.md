# Traefik Airlines: Microservices Demo with Kubernetes and Traefik

## Overview

Traefik Airlines is a comprehensive microservices demo application showcasing modern cloud-native architecture using Kubernetes and Traefik as the edge router. This repository demonstrates best practices for building, deploying, and managing a distributed airline management system.

## Architecture

The application is composed of several microservices:
- **Customers Service**: Manages customer information
- **Employees Service**: Handles employee-related operations
- **Flights Service**: Manages flight scheduling and information
- **Tickets Service**: Handles ticket booking and management

## Project Structure

```
traefik-airlines/
├── customers/
├── employees/
├── flights/
└── tickets/
```

Each service directory contains:
- `kustomization.yaml`: Kubernetes resource configuration
- `route.yaml`: Traefik routing configuration

## Getting Started

### Deployment

1. Apply Traefik configuration
2. Deploy each microservice using Kustomize

```bash
kubectl apply -k customers/
kubectl apply -k employees/
kubectl apply -k flights/
kubectl apply -k tickets/
```
