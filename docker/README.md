# Docker Lab

This directory contains containerization experiments using **:contentReference[oaicite:1]{index=1}**.

## Purpose

Practice container deployment and container-based services that later run on Kubernetes.

## Examples

examples/
Basic container experiments such as running nginx.

compose/
Multi-container setups using Docker Compose.

docs/
Notes and documentation for Docker experiments.

## Example: Run an nginx container

docker run -d -p 8080:80 nginx

Access the container:

http://SERVER_IP:8080
