
# devsecops-terraform-hardened

Enterprise DevSecOps pipeline with Terraform IaC security scanning,
container hardening, secrets management, SBOM generation, and automated
security gating using GitLab CI and GitHub Actions.

## Branch Convention

| Branch | Purpose |
|---|---|
| `main` | Stable, production-ready |
| `develop` | Integration branch |
| `DSOPS-AI-001` | Baseline pipeline scaffold |
| `DSOPS-AI-002` | IaC security scanning (Checkov) |
| `DSOPS-AI-003` | Secrets management |
| `DSOPS-AI-004` | Container security (Trivy) |
| `DSOPS-AI-005` | Supply chain (SBOM + Cosign) |
| `DSOPS-AI-006` | Pipeline hardening + security gating |

## Structure

app/           # Target microservice application

terraform/     # Infrastructure as Code

docs/          # Security findings, threat model, metrics

.gitlab-ci.yml # GitLab CI pipeline

.github/

workflows/   # GitHub Actions workflows
