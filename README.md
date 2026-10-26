# Cloud DevOps Pipeline

![Status](https://img.shields.io/badge/status-in%20progress-orange)
![Started](https://img.shields.io/badge/started-October%202026-blue)

An end-to-end DevOps project: a small multi-service application with a fully automated build, test, deploy, and monitoring pipeline around it. Everything is version-controlled, repeatable, and documented.

> **Status:** In progress. Sections marked *(planned)* are not built yet. The roadmap below tracks what is complete.

---

## Pipeline Overview

```
Code push ──► GitHub Actions ──► Docker image ──► Deploy target ──► Prometheus ──► Grafana
              (lint, test,       (built and       (provisioned     (collects      (dashboards
               build)             published)       by Terraform)    metrics)       and alerts)
```

## Architecture

| Layer | Tool | Purpose |
|---|---|---|
| Containerization | Docker, Docker Compose | Package each service with its dependencies so it runs identically on any machine |
| CI/CD | GitHub Actions | Automatically lint, test, build, and publish images on every push |
| Infrastructure as Code | Terraform | Define and provision infrastructure from code instead of manual setup |
| Observability | Prometheus, Grafana | Collect metrics, visualize system health, and alert before failures occur |

## Tech Stack

- **Version control:** Git, GitHub
- **Containers:** Docker, Docker Compose
- **Automation:** GitHub Actions
- **Infrastructure:** Terraform
- **Monitoring:** Prometheus, Grafana
- **Cloud provider:** AWS *(optional, pending free-tier verification)*

## Roadmap

- [ ] **Phase 1: Environment and fundamentals** (local tooling, terminal, Git workflow)
- [ ] **Phase 2: Containerization** (Dockerfiles, multi-service setup with Docker Compose)
- [ ] **Phase 3: CI/CD** (GitHub Actions workflows for lint, test, build, publish)
- [ ] **Phase 4: Infrastructure as Code** (Terraform configuration, validated locally first)
- [ ] **Phase 5: Observability** (metric scraping, Grafana dashboards, alert rules)

## Planned Repository Structure *(planned)*

```
.
├── app/                  # application services and Dockerfiles
├── docker-compose.yml    # local multi-service environment
├── .github/workflows/    # CI/CD pipelines
├── terraform/            # infrastructure definitions
├── monitoring/           # Prometheus config, Grafana dashboards
└── docs/                 # learning log and architecture notes
```

## Documentation

A troubleshooting and learning log will be kept in `docs/`, recording what broke, why it broke, and how it was fixed.

## Getting Started *(planned)*

Setup and run instructions will be added once Phase 2 is complete.

---

*Sample application: to be selected in Phase 2.*
