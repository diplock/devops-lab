# Kubernetes Monitoring Stack

This directory documents the monitoring stack used in the DevOps lab Kubernetes cluster.

## Components

The monitoring system consists of:

- Prometheus (metrics collection)
- Node Exporter (node metrics)
- Grafana (visualization dashboards)

## Architecture

Kubernetes Nodes
        |
        | metrics
        v
Node Exporter
        |
        v
Prometheus Server
        |
        v
Grafana Dashboards

## Prometheus

Prometheus collects metrics from different targets using a pull model.

Example scrape target configuration:

scrape_configs:

job_name: "node-exporter"
static_configs:

targets: ["192.168.122.14:9100"]

Metrics are stored in the Prometheus time-series database.

Access Prometheus UI:

http://SERVER_IP:9090

## Node Exporter

Node Exporter exposes Linux system metrics including:

- CPU usage
- Memory usage
- Disk usage
- Network statistics

Metrics endpoint:

http://SERVER_IP:9100/metrics

## Grafana

Grafana connects to Prometheus as a data source and visualizes metrics using dashboards.

Typical dashboards include:

- Node resource usage
- Kubernetes cluster metrics
- Container monitoring

Default Grafana access:

http://SERVER_IP:3000

## Monitoring Goals

The monitoring system helps to:

- Observe cluster health
- Detect performance issues
- Track system resource utilization
- Trigger alerts for failures
