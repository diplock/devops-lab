# DevOps Lab

This repository contains my personal DevOps lab used to practice modern infrastructure automation and observability.

## Technologies Practiced

- Ansible automation
- Docker containers
- Kubernetes (K3s)
- Prometheus monitoring
- Grafana dashboards
- Git and GitHub
- CI/CD pipelines (GitHub Actions)
- Infrastructure as Code

## Lab Infrastructure

Control Node:
Ubuntu VM running on KVM virtualization.

Managed Nodes:

- Alpine Linux VM (Kubernetes Control Plane)
- Alpine Linux VM (Kubernetes Worker Node)

## DevOps Components

### Automation

Server configuration using Ansible playbooks located in:

These playbooks automate:

- Nginx installation
- Docker host setup
- Container deployment

### Containerization

Docker is used for container workloads and experimentation.

### Kubernetes

A lightweight Kubernetes cluster is deployed using **:contentReference[oaicite:1]{index=1}**.

### Monitoring Stack

Cluster monitoring implemented using:

- **:contentReference[oaicite:2]{index=2}**
- **:contentReference[oaicite:3]{index=3}**
- **:contentReference[oaicite:4]{index=4}**

Metrics collected include:

- Node CPU usage
- Memory usage
- Network traffic
- Disk IO

### CI/CD

Automation pipelines using **:contentReference[oaicite:5]{index=5}**.

## Lab Goals

This lab is used to practice real-world DevOps engineering skills including:

- Infrastructure automation
- Kubernetes cluster management
- Observability and monitoring
- Troubleshooting distributed systems
- Continuous integration and deployment

## Future Improvements

Planned additions:

- kube-state-metrics
- Alertmanager alerts
- Kubernetes dashboards
- Terraform infrastructure provisioning
