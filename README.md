# k8s-soc2-compliance
A Kubernetes security and compliance project designed to meet SOC 2 requirements using Kafka, Elasticsearch, and PostgreSQL. This project implements a real-time auditing and monitoring system to track security events, enforce compliance policies, and analyze logs for potential threats.

# Goals

#### Collect & analyze Kubernetes logs for SOC 2 compliance
#### Stream logs to Kafka for scalable processing.
#### Store logs in Elasticsearch (search & dashboards) & PostgreSQL (audit reports).
#### Set up alerts for compliance violations.

# High-Level Architecture

#### Log Collection → API Server Audit Logs, Kubelet Logs, Pod Logs.
#### Kafka → Central log pipeline (kubernetes.api.audit, kubernetes.pods.logs, etc.).
#### Storage →

    Elasticsearch (fast search & dashboards).
    PostgreSQL (structured audit reports).
#### Alerting & Dashboards → Kibana, Grafana, Prometheus.