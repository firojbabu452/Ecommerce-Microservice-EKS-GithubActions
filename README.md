# DevOps + AIOps Series

> A full end-to-end DevOps project with AIOps integration — so you can connect the dots between how AI is helping automate

---

## Welcome


Welcome to my DevOps + AI series where we build an end-to-end DevOps project with an AIOps integration.

A lot of you have been asking: *"when are you going to share a full DevOps project?"*

Well — here we are.

In this series we will:

- Build microservices locally
- Use Claude and AI tools to assist development
- Deploy everything step by step
- Migrate the system to the cloud on AWS EKS
- Set up a full CI/CD pipeline with GitHub Actions
- Implement GitOps workflows with ArgoCD
- Integrate AIOps capabilities with AWS Bedrock

By the end of this series, you won't just know tools — you'll understand how real DevOps systems are designed and deployed.

---

## Repository Structure

```
DevOps-Practice-Guide/
├── docs/
│   ├── part1-system-design.md     # System design foundations (Part 1)
│   ├── part2-workflow.md          # Full workflow with AIOps (Part 2)
│   └── claude-setup.md            # Claude Code + MCP server setup
├── projects/
│   ├── README.md                  # EKS deployment guide (Part 3)
│   ├── boutique-microservices/    # The application (7 services)
│   ├── Infrastructure/            # Terraform for AWS provisioning
│   └── aiops-assistant/           # Bedrock Agent — Kira (Part 4)
├── gitops/
│   ├── argo-cd.yml                # ArgoCD Application manifest
│   ├── kustomization.yml          # Kustomize entry point
│   └── k8s/                       # All Kubernetes manifests
└── .github/
    └── workflows/ci.yml           # GitHub Actions CI pipeline
```

---

## Series Structure

### Part 1 — System Design Foundations
[`docs/part1-system-design.md`](docs/part1-system-design.md)

We start with system design concepts specifically for cloud and DevOps. This is important whether you're a beginner, intermediate, or senior engineer — because companies don't choose tools randomly. They think about architecture patterns, deployment strategies, scalability, reliability, and cost tradeoffs.

We cover 12 core system design pillars used in modern DevOps architectures, and connect each one directly to something running in this project.

---

### Part 2 — Understanding the Workflow
[`docs/part2-workflow.md`](docs/part2-workflow.md)

Before writing any code or deployment configs, you need to understand how the entire system flows:

- What services we're building and how they communicate
- How the pipeline works
- How code moves from developer → CI → deployment → production → AIOps

This is where the full picture comes together — including how AI fits into the workflow.

---

### Part 3 — DevOps Project Implementation
[`projects/README.md`](projects/README.md)

Then we actually build the project. You'll see:

- Docker containers and Docker Compose
- Kubernetes deployments on EKS
- CI/CD pipelines with GitHub Actions
- GitOps automation with ArgoCD
- Infrastructure provisioning with Terraform
- Observability with Prometheus and Grafana



---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Application | React, Node.js, PostgreSQL |
| Containers | Docker, Docker Compose |
| Orchestration | Kubernetes (AWS EKS) |
| Infrastructure | Terraform |
| CI/CD | GitHub Actions |
| GitOps | ArgoCD + Kustomize |
| Monitoring | Prometheus + Grafana |
| Log Forwarding | AWS Fluent Bit → CloudWatch |
| AIOps | AWS Bedrock Agent (Kira) |
| AI Assistant | Claude Code + MCP Servers |
