# Observability Stack

This project sets up a complete observability stack on a local Kubernetes cluster using Kind. It provides a comprehensive monitoring, logging, and tracing solution for your applications.

## Overview

The stack includes the following components:
- **Prometheus**: Metrics collection and storage
- **Grafana**: Visualization and dashboarding
- **Loki**: Log aggregation and storage
- **Alloy**: OpenTelemetry collector for metrics and traces
- **Tempo**: Distributed tracing backend
- **ArgoCD**: GitOps
- **Github Actions**: Pipeline for testing terraform changes

## Prerequisites

Before you begin, ensure you have the following tools installed:
- [Terraform](https://www.terraform.io/downloads.html) (11.0.3 or later)
- [Atmos](https://atmos.tools) (latest version)
- [Kind](https://kind.sigs.k8s.io/docs/user/quick-start/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [Docker](https://docs.docker.com/get-docker/)

## Installation

1. Clone this repository
2. Install the Pre-requisites
2. Run the following commands:
   ```bash
   # Initialize Project
   atmos deploy 


## Components

### Prometheus
- Collects and stores metrics as time series data
- Provides a powerful query language (PromQL)
- Supports service discovery and scraping

### Grafana
- Creates, explores, and shares dashboards
- Supports multiple data sources
- Rich visualization options

### Loki
- Log aggregation system
- Prometheus-inspired query language (LogQL)
- Efficient log storage and retrieval

### Alloy
- OpenTelemetry collector
- Handles metrics and traces
- Configurable pipelines

### Tempo
- Distributed tracing backend
- Supports multiple trace protocols
- Integrates with Grafana for visualization

## Accessing the Stack

Once deployed, you can access the components at:
- Grafana: http://localhost:3000
- Prometheus: http://localhost:9090
- Loki: http://localhost:3100
- Tempo: http://localhost:3200

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
