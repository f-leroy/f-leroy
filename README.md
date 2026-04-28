<table><tr><td width="75%">

### Hey, I'm Frédéric 👋

**Azure Cloud Architect · Microsoft Certified Trainer**

As a trainer and architect on Azure, I know how much time it takes to build production-ready infrastructure the right way. Azure Verified Modules are great, but each one comes with dozens of variables to configure, wire together, and validate. I wanted to help teams skip the repetitive plumbing and go straight to deploying with confidence.

That's why I built **[AethronOps](https://aethronops.com)**.

</td><td width="25%" align="right" valign="top">

<img src="assets/mct-badge.png" width="150" />

</td></tr></table>

---

#### The problem AethronOps solves

Setting up production-ready Azure infrastructure is painful:

- Writing Terraform for a typical stack takes **days to weeks**
- Wiring resources together correctly (networking, identity, monitoring, secrets) is error-prone
- Documenting how each resource maps to industry frameworks (MCSB, CAF, WAF, GDPR, NIS2) is tedious and usually skipped
- Most teams deploy first, then scramble before audits

**AethronOps generates all of this in one ZIP.** You pick a stack, choose your mode (dev free / production paid), and download a complete Terraform project — validated, wired, framework-aligned.

---

#### What makes it different

🏗️ **11 production-ready stacks** — App Service or Container Apps, paired with PostgreSQL / SQL / Cosmos DB / MySQL / MongoDB, plus a shared Platform Baseline (VNet, NAT, NSG, Redis, Private DNS Zones)

⚡ **Built on Azure Verified Modules** — every stack uses Microsoft's official AVM modules. No custom resources, no drift from Azure best practices. Telemetry off, versions pinned.

🔌 **Auto-wired** — networking, identity, monitoring, Key Vault, Private Endpoints, Entra-ID passwordless DB auth, EventGrid expiry alerts... 40 to 60 resources connected end-to-end per stack. Not just modules dropped in a folder — actual working infrastructure.

🔒 **Framework-aligned per stack** — each ZIP includes a `SECURITY-POSTURE.md` mapping ~61 controls to MCSB, CAF, WAF, GDPR/RGPD, NIS2 (with traceability to DORA, CIS, ISO 27001, SOC 2, PCI-DSS). Aligned with — not certified by.

✅ **Validated end-to-end on Azure** — every stack passes `terraform validate`, `terraform plan`, `checkov`. Every workload variant has been deployed and torn down on a real Azure subscription before shipping.

🚫 **Zero access to your environment** — AethronOps never touches your Azure, your repo, or your credentials. You get a ZIP, you deploy it yourself.

---

#### Who it's for

- **CTOs & DSI** who need framework-aligned Azure infrastructure without hiring a Terraform expert
- **Azure consultants** who want to deliver faster with battle-tested templates
- **DevOps engineers** who are tired of reinventing the wheel for every project
- **CISOs & compliance teams** who need audit-prep documentation from day one
- **Startups** who want enterprise-grade security without the enterprise budget

---

#### How it works

```
1. Browse the catalog        → 11 stacks · App Service · Container Apps · 5 databases
2. Pick your mode            → dev (free, MIT) / production (paid, brownfield-ready)
3. Download your ZIP         → complete Terraform project, ready to deploy
4. terraform init && apply   → your infrastructure is live
```

Every production ZIP contains:

```
my-stack/
├── main.tf, app.tf, database.tf, identity.tf, keyvault.tf, monitoring.tf, ...
├── wiring.tf               ← brownfield wiring (3 modes: remote state / VNet ID / lookup by name)
├── finops.tf               ← budget alerts, auto-shutdown, storage lifecycle
├── governance.tf           ← Azure Policy, optional resource locks
├── envs/prod.tfvars        ← enterprise variables, ready to customise
├── .github/workflows/deploy-prod.yml  ← GitHub Actions OIDC pipeline
├── README.md, INSTALL.md, CHANGELOG.md
└── SECURITY-POSTURE.md     ← 61 controls mapped across 4 frameworks
```

---

#### Try it free

🆓 **10 dev stacks open source on GitHub** — MIT licensed, no account needed:

| Stack | Database | Compute |
|-------|---------|---------|
| [app-service-postgresql](https://github.com/Aethronops/aethronops/tree/main/stacks/app-service-postgresql) | PostgreSQL Flexible Server | App Service |
| [app-service-sql](https://github.com/Aethronops/aethronops/tree/main/stacks/app-service-sql) | Azure SQL Database | App Service |
| [app-service-cosmosdb](https://github.com/Aethronops/aethronops/tree/main/stacks/app-service-cosmosdb) | Cosmos DB (NoSQL) | App Service |
| [app-service-mysql](https://github.com/Aethronops/aethronops/tree/main/stacks/app-service-mysql) | MySQL Flexible Server | App Service |
| [app-service-mongodb](https://github.com/Aethronops/aethronops/tree/main/stacks/app-service-mongodb) | DocumentDB (MongoDB vCore) | App Service |
| [container-apps-postgresql](https://github.com/Aethronops/aethronops/tree/main/stacks/container-apps-postgresql) | PostgreSQL Flexible Server | Container Apps |
| [container-apps-sql](https://github.com/Aethronops/aethronops/tree/main/stacks/container-apps-sql) | Azure SQL Database | Container Apps |
| [container-apps-cosmosdb](https://github.com/Aethronops/aethronops/tree/main/stacks/container-apps-cosmosdb) | Cosmos DB (NoSQL) | Container Apps |
| [container-apps-mysql](https://github.com/Aethronops/aethronops/tree/main/stacks/container-apps-mysql) | MySQL Flexible Server | Container Apps |
| [container-apps-mongodb](https://github.com/Aethronops/aethronops/tree/main/stacks/container-apps-mongodb) | DocumentDB (MongoDB vCore) | Container Apps |

**Need the production version?** [aethronops.com/stacks](https://aethronops.com/stacks) — 199 € HT per stack, or 499 € HT for all 11 (one-time, no subscription).

---

#### Certifications

![MCT](https://img.shields.io/badge/MCT-Certified_Trainer-5E5E5E?style=flat&logo=microsoft&logoColor=white)
![Azure Solutions Architect](https://img.shields.io/badge/Azure_Solutions_Architect-Expert-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Azure Administrator](https://img.shields.io/badge/Azure_Administrator-Associate-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Azure DB Admin](https://img.shields.io/badge/Azure_DB_Administrator-Associate-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![Azure AI](https://img.shields.io/badge/Azure_AI-Fundamentals-0078D4?style=flat&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Cloud_Practitioner-FF9900?style=flat&logo=amazonwebservices&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-Certified_Associate-F80000?style=flat&logo=oracle&logoColor=white)

---

#### Tech

`Terraform` · `Azure` · `Python` · `FastAPI` · `Astro` · `React` · `TypeScript` · `Tailwind CSS` · `GitHub Actions` · `Docker` · `SQL Server` · `Oracle` · `PostgreSQL` · `MySQL` · `CosmosDB` · `Redis` · `MongoDB`

---

<p align="center">
  <a href="https://aethronops.com"><strong>aethronops.com</strong></a> · <a href="https://github.com/Aethronops/aethronops">Stack Catalog</a> · <a href="https://aethronops.com/contact/">Contact</a>
</p>
