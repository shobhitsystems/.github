# Shobhit Systems

> We help startups build their infrastructure on Google Cloud — end to end, from day zero to production.

We are a GCP infrastructure partner for early-stage startups. We design, build, and hand over complete cloud infrastructure and CI/CD pipelines on Google Cloud Platform, so your engineering team can focus entirely on the product.

No piecing together tutorials. No months lost on cloud setup. Just a solid, production-grade foundation — built for you.

---

## What we do

- **Infrastructure setup** — VPC, IAM, Cloud Run, Cloud SQL, Artifact Registry, and more, all provisioned via Terraform
- **CI/CD pipelines** — automated build, test, and deploy pipelines using Cloud Build, so every code push flows safely to production
- **Security baseline** — least-privilege IAM, service account conventions, and network policies from day one
- **Handover-ready** — everything is documented, version-controlled, and built to be owned by your team long-term

---

## Open-source modules

These repositories are the Terraform modules we use to build GCP infrastructure for our clients. They are open-sourced so the community can benefit from the same patterns.

### 🏗️ [gcp-startup-stack](https://github.com/shobhit-systems/gcp-startup-stack)
The core infrastructure stack for startups launching on GCP. Provisions Cloud Run, Cloud SQL, Artifact Registry, VPC networking, and IAM — all wired up and production-ready from day one.

`Cloud Run` · `Cloud SQL` · `Artifact Registry` · `VPC` · `IAM`

---

### 🔐 [gcp-iam-baseline](https://github.com/shobhit-systems/gcp-iam-baseline)
A secure IAM baseline for GCP projects. Enforces least-privilege access, defines service account conventions, and gives your team a consistent, auditable permissions model from the start.

`Service Accounts` · `IAM Roles & Bindings` · `Least-privilege policies`

---

### 🚀 [gcp-artifact-registry-cicd](https://github.com/shobhit-systems/gcp-artifact-registry-cicd)
Provisions Artifact Registry and Cloud Build triggers via Terraform. Every push automatically builds and stores a fresh container image — no manual `docker push` ever again.

`Artifact Registry` · `Cloud Build Triggers` · `Automated image pipeline`

---

## How the modules fit together

```
gcp-iam-baseline           →   secure service accounts & roles
        ↓
gcp-startup-stack          →   Cloud Run, Cloud SQL, VPC built on top of those roles
        ↓
gcp-artifact-registry-cicd →   automated image builds & pushes on every code push
```

Together they form a complete, production-grade GCP setup for any startup — or adopt each module independently as needed.

---

## Work with us

If you're a startup that needs a GCP infrastructure partner, we'd love to help. We handle the full setup — infrastructure, CI/CD, security, and documentation — so your team hits the ground running.

📬 Reach out to via [Chat](https://wa.me/917045529476) for free audit.

---

*Built with care by [Shobhit Systems](https://shobhitsystems.com)*
