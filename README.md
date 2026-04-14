# 👋 Hermann Arnaud Djoko

### DevOps Engineer | AWS Solutions Architect | Platform Engineer
**Québec, Canada 🇨🇦 | Bilingue FR/EN**

[![AWS SAA](https://img.shields.io/badge/AWS-Solutions_Architect_Associate-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://www.credly.com/org/amazon-web-services/badge/aws-certified-solutions-architect-associate)
[![Terraform Associate](https://img.shields.io/badge/HashiCorp-Terraform_Associate-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)](https://www.credly.com/org/hashicorp/badge/hashicorp-certified-terraform-associate-003)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-hermanndjoko-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/hermanndjoko)

---

## 🚀 À propos

Ingénieur DevOps et Architecte Cloud avec **10+ ans d'expérience** en infrastructure IT, cloud AWS/Azure et automatisation.

Je conçois et déploie des plateformes cloud **production-grade** :
- ☁️ **Infrastructure as Code** — Terraform (modules, multi-env, remote state)
- 🔄 **CI/CD** — GitHub Actions (fmt → validate → tflint → checkov → plan)
- 🐳 **Conteneurisation** — Docker + Kubernetes (EKS/AKS) + Helm
- 🔐 **DevSecOps** — Checkov, TFLint, IAM least-privilege, IRSA, KMS
- 💰 **FinOps** — Infracost, cost-controlled deployments, Free Tier optimization

---

## 🛠️ Stack technique

```
Cloud        │ AWS (EKS, Lambda, RDS, VPC, IAM, CloudWatch...)
             │ Azure (AKS, ACR, App Service, Static Web Apps)
─────────────┼──────────────────────────────────────────────
IaC          │ Terraform • Ansible
─────────────┼──────────────────────────────────────────────
CI/CD        │ GitHub Actions • Docker • Kubernetes • Helm
─────────────┼──────────────────────────────────────────────
Langages     │ Python 3 • Bash • HCL
─────────────┼──────────────────────────────────────────────
Sécurité     │ Checkov • TFLint • CodeQL • Trivy • IRSA
─────────────┼──────────────────────────────────────────────
Virtualisation│ VMware vSphere/ESXi • NetApp SAN
─────────────┼──────────────────────────────────────────────
OS           │ Linux (Ubuntu/CentOS/RHEL — 10+ ans)
```

---

## 📂 Projets Portfolio

### 🏗️ [aws-eks-platform-terraform](https://github.com/HermannDj/aws-eks-platform-terraform)
> Plateforme EKS production-grade déployée sur AWS **ca-central-1**

[![CI — PR Checks](https://github.com/HermannDj/aws-eks-platform-terraform/actions/workflows/pr-checks.yml/badge.svg)](https://github.com/HermannDj/aws-eks-platform-terraform/actions/workflows/pr-checks.yml)
[![CI — Post-merge Plan](https://github.com/HermannDj/aws-eks-platform-terraform/actions/workflows/merge-plan.yml/badge.svg)](https://github.com/HermannDj/aws-eks-platform-terraform/actions/workflows/merge-plan.yml)

- **VPC 3-tier** (public/private/database) + NAT Gateway + Flow Logs
- **EKS** managed node groups + **IRSA** (IAM Roles for Service Accounts)
- **RDS PostgreSQL** + **ElastiCache Redis** + **ALB** + **Secrets Manager**
- **CI/CD** : TFLint → Checkov → Infracost → terraform plan (commentaire PR)
- **Multi-env** : dev (déployable ~$0.15/h) / staging / prod
- **ADR** (Architecture Decision Records) inclus

```bash
# Preuve de déploiement réel — ca-central-1
kubectl get nodes
# ip-10-0-35-123... Ready  v1.30.14-eks ✓
# ip-10-0-37-206... Ready  v1.30.14-eks ✓
# ip-10-0-62-187... Ready  v1.30.14-eks ✓
```

---

### ⚡ [aws-serverless-api-terraform](https://github.com/HermannDj/aws-serverless-api-terraform)
> API REST serverless — **$0/mois** sur AWS Free Tier

[![CI — PR Checks](https://github.com/HermannDj/aws-serverless-api-terraform/actions/workflows/pr-checks.yml/badge.svg)](https://github.com/HermannDj/aws-serverless-api-terraform/actions/workflows/pr-checks.yml)
[![AWS Free Tier](https://img.shields.io/badge/AWS-Free_Tier_Safe-FF9900?style=flat&logo=amazonaws)](https://aws.amazon.com/free/)

- **API Gateway** + **Lambda Python 3.12** + **DynamoDB** + **Cognito**
- **36 tests unitaires pytest** — couverture complète, aucun appel AWS réel
- **Multi-env** dev/staging/prod + remote state S3 + DynamoDB lock
- **CI/CD** : fmt → validate → TFLint → Checkov → plan

---

### 🐳 [aks-project](https://github.com/HermannDj/aks-project)
> CI/CD Kubernetes — Docker build → push ACR → deploy AKS

- Pipeline GitHub Actions : build → push Azure Container Registry → deploy kubectl
- Manifests K8s : rolling update, readiness/liveness probes
- App Python/Flask avec endpoint `/healthz`

---

### ☁️ [terraform-infra-azure](https://github.com/HermannDj/terraform-infra-azure)
> IaC Azure — ACR + App Service + CI Terraform

- Terraform : Resource Group, ACR, App Service Plan, App Service
- GitHub Actions : init → fmt → validate → plan → apply

---

### 🔄 [HermannDj-cicd-flask-project](https://github.com/HermannDj/HermannDj-cicd-flask-project)
> CI/CD Flask — tests → build → push → deploy Azure Web App

- Tests pytest + artifacts upload
- Build/push Docker → Azure Container Registry
- CodeQL + scan Trivy + déploiement Azure Web App

---

## 📊 GitHub Stats

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=HermannDj&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=HermannDj&layout=compact&theme=tokyonight&hide_border=true" height="150"/>
</p>

---

## 🏅 Certifications

| Certification | Organisme | Année |
|---|---|---|
| ✅ AWS Certified Solutions Architect – Associate | Amazon Web Services | 2025 |
| ✅ HashiCorp Terraform Associate (003) | HashiCorp | 2024 |
| VMware Technical Solution Professional (VTSP) | VMware | 2016 |
| NetApp Accredited Sales Professional (NASP) | NetApp | 2018 |
| CCNA – Cisco Certified Network Associate | Cisco | 2010 |

---

## 📫 Me contacter

- 💼 **LinkedIn** : [linkedin.com/in/hermanndjoko](https://linkedin.com/in/hermanndjoko)
- 📧 **Email** : harnaud.djoko@gmail.com
- 📍 **Localisation** : Québec, Canada — Remote ✅ | Hybride ✅

---

*Disponible pour missions DevOps / Cloud Architect via placement — Québec, Montréal, Remote Canada*
