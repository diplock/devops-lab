# Kubernetes Lab

This directory documents the Kubernetes cluster deployed in the DevOps lab.

The cluster is built using K3s running on Alpine Linux virtual machines.

## Cluster Architecture

Control Plane
- Alpine Linux VM running K3s

Worker Node
- Alpine Linux VM

## Monitoring Stack

The cluster monitoring stack includes:

- Prometheus
- Grafana
- Node Exporter

These tools collect and visualize system metrics from Kubernetes nodes.

## Directory Structure

cluster-setup/
Instructions for installing the K3s cluster.

manifests/
Kubernetes deployment YAML files.

monitoring/
Monitoring stack documentation.

docs/
Architecture documentation.
