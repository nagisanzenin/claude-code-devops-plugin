# DevOps Plugin for Claude Code

Full DevOps pipeline generator for production-grade deployments. Generates a `DevOps-Suite/` folder with Terraform modules, CI/CD pipelines, container orchestration, monitoring dashboards, and security configs for AWS, GCP, and Azure.

## Features

- Terraform IaC with multi-cloud modules and environment separation
- CI/CD pipelines (GitHub Actions, GitLab CI) with blue-green/canary deployments
- Docker multi-stage builds and Kubernetes manifests (Kustomize + Helm)
- Prometheus/Grafana monitoring with SLO-based alerting and runbooks
- Security scanning (SAST, dependency audit, container scan, IaC scan)
- Secrets management, IAM policies, compliance checklists
- Incident response playbooks and post-mortem templates

## Installation

### Via Marketplace
```
/plugin marketplace add nagisanzenin/nagisanzenin-plugins
/plugin install devops@nagisanzenin
```

### Load Directly
```
claude --plugin-dir /path/to/devops-plugin
```

## Usage

Trigger with phrases like:
- "Set up CI/CD for this project"
- "Create Terraform infrastructure"
- "Deploy to Kubernetes"
- "Set up monitoring and alerting"
- "DevOps pipeline for production"

The skill runs a 6-phase pipeline: Assessment → IaC → CI/CD → Containers → Monitoring → Security

## License

MIT
