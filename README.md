# Cloud DevOps Pipeline Project

## Project Overview
This project simulates a real world engineering workflow: taking a local application, containerizing it, automating its testing and delivery, and monitoring its health—all using industry-standard tools.

## The Architecture
The infrastructure is built in four layers:
*   **Containerization (Docker):** Packaging the application and its environment so it runs identically on any machine.
*   **Continuous Integration & Deployment (GitHub Actions):** An automated pipeline that builds, tests, and prepares the application for deployment every time code is pushed.
*   **Infrastructure as Code (Terraform):** Defining and provisioning the underlying infrastructure via code rather than manual configuration.
*   **Observability (Prometheus & Grafana):** A telemetry system to collect performance metrics and visualize system health to catch errors before they cause downtime.

## Current Learning Roadmap & Progress
- [ ] **Phase 1: Environment & Terminal Basics** (Setting up local tools, mastering the CLI, and understanding Git version control)
- [ ] **Phase 2: Containerization** (Writing Dockerfiles and orchestrating services locally)
- [ ] **Phase 3: CI/CD Automation** (Building GitHub Actions workflows)
- [ ] **Phase 4: Infrastructure as Code** (Learning Terraform configuration locally)
- [ ] **Phase 5: Observability** (Setting up metric scraping and dashboards)

---
*Note: This repository serves as a live portfolio documenting my daily engineering progress, architectural choices, and troubleshooting milestones.*
