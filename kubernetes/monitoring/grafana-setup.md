# Grafana Setup

Grafana is used to visualize metrics collected by Prometheus.

Access URL:

http://SERVER_IP:3000

Default login:

admin / admin

## Adding Prometheus as a Data Source

1. Open Grafana UI
2. Navigate to Settings
3. Select Data Sources
4. Add Prometheus

Prometheus URL:

http://localhost:9090

## Importing Dashboards

Recommended dashboards:

- Node Exporter Dashboard
- Kubernetes Cluster Monitoring
