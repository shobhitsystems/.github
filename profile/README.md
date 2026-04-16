# Shobhit Systems

> Production-ready GCP infrastructure modules for startups — opinionated, modular, and built to scale.

We build Terraform modules that give early-stage teams a solid cloud foundation on Google Cloud Platform, so you spend time shipping features, not fighting infrastructure.

---

## Repositories

### 🏗️ [gcp-startup-stack](https://github.com/shobhit-systems/gcp-startup-stack)
The core infrastructure stack for startups launching on GCP. Provisions Cloud Run services, Cloud SQL, Artifact Registry, VPC networking, and IAM — all wired up and production-ready from day one.

**Includes:** Cloud Run · Cloud SQL · Artifact Registry · VPC · IAM

---

### 🔐 [gcp-iam-baseline](https://github.com/shobhit-systems/gcp-iam-baseline)
Terraform module for setting up a secure IAM baseline on GCP. Enforces least-privilege access, defines service account conventions, and gives your team a consistent, auditable permissions model from the start.

**Includes:** Service Accounts · IAM Roles & Bindings · Least-privilege policies

---

### 🚀 [gcp-artifact-registry-cicd](https://github.com/shobhit-systems/gcp-artifact-registry-cicd)
Provisions GCP Artifact Registry and Cloud Build triggers via Terraform. Every push automatically builds and stores a fresh container image — no manual `docker push` ever again.

**Includes:** Artifact Registry · Cloud Build Triggers · Automated image pipeline

---

## How the modules fit together

```
gcp-iam-baseline          →   sets up secure service accounts & roles
      ↓
gcp-startup-stack         →   provisions Cloud Run, Cloud SQL, VPC using those roles
      ↓
gcp-artifact-registry-cicd →  builds & pushes images via Cloud Build on every push
```

Use all three together for a complete, production-grade GCP setup, or adopt each module independently based on your needs.

---

## Getting started

Each repository contains its own `README.md` with usage instructions, input variables, and example configurations. Clone the repo that fits your need and follow the setup guide inside.

**Prerequisites across all modules:**
- [Terraform](https://developer.hashicorp.com/terraform/install) >= 1.3
- [gcloud CLI](https://cloud.google.com/sdk/docs/install) authenticated with a GCP project
- A GCP project with billing enabled

---

## Philosophy

- **Opinionated by default** — sensible defaults that follow GCP best practices, easy to override
- **Modular** — use one module or all three; no hard dependencies unless noted
- **Startup-first** — minimal complexity, fast to bootstrap, easy to hand off to a growing team

---

*Maintained by [Shobhit Systems](https://shobhitsystems.com/)*
