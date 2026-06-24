<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0078D4,100:1B3A57&height=170&section=header&text=Fr%C3%A9d%C3%A9ric%20LEROY&fontSize=42&fontColor=ffffff&desc=Azure%20Cloud%20%26%20Database%20Automation&descSize=18&descAlignY=72" width="100%" />

![MCT](https://img.shields.io/badge/MCT-Certified_Trainer-5E5E5E?style=flat-square&logo=microsoft&logoColor=white)
![AZ-305](https://img.shields.io/badge/AZ--305-Solutions_Architect_Expert-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![AZ-104](https://img.shields.io/badge/AZ--104-Administrator_Associate-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![DP-300](https://img.shields.io/badge/DP--300-Database_Administrator_Associate-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![SC-300](https://img.shields.io/badge/SC--300-Identity_%26_Access-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-Cloud_Practitioner-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)

</div>

### Hi, I'm Frédéric 👋

I design and run **production Azure infrastructure** and **database platforms** — with a focus on
**automation** (Terraform + Ansible), **security by design**, and **Oracle → PostgreSQL migrations**.
I open-source what I can; the rest is built the same way, privately.

---

### What I'm building

**🧱 AethronOps v3** — *IaC stack catalogue (personal project)*
- YAML-driven generation of **10 App Service / Container Apps stacks** coupled to PostgreSQL, Azure SQL,
  Cosmos DB, MySQL and MongoDB — on **Azure Verified Modules** (pinned versions).
- **Security by design**: Key Vault, Managed Identity, Private Endpoints, Backup Vault; a per-stack
  `SECURITY-POSTURE` document aligned to **CAF / MCSB / NIS2 / GDPR / WAF**.
- Automated **build & validate** pipeline: Python, Terraform 1.9+, Checkov, preflight scripts.

**🗄️ db-platform** — *multi-engine database automation on Azure (personal project)*
- 3-layer model: **Packer** (image) + **Terraform** (infra) + **Ansible** (config).
- **Oracle 19c** — install, CIS hardening, tuning, RMAN, **Data Guard** (broker + Fast-Start Failover,
  validated live), golden-image factory, self-verification.
- **SQL Server** — validated end-to-end: **Always On AG** with **DNN listener**, **TDE**, hardening
  (18 Ansible roles, 3 infra stacks).
- **PostgreSQL 17** — dual-distro (EL9 + Ubuntu), **Patroni** + streaming HA, **pgBackRest**, air-gapped
  install — validated on real Azure.
- **Oracle → PostgreSQL migration** — a toolkit (ora2pg + oracle_fdw) with a read-only pre-migration
  risk analyzer, **proven end-to-end on real Azure**.
- Runs from a **CI runner inside the VNet**: OIDC / Managed Identity, remote Terraform state, secrets in
  Key Vault, GitHub Actions.

---

### 📦 Open-source

- **[azure-terraform-avm-secure-stacks](https://github.com/f-leroy/azure-terraform-avm-secure-stacks)** — 9 production-validated Azure Terraform stacks (App Service / Container Apps × PostgreSQL / SQL / Cosmos / Mongo + a shared platform baseline), apply-validated on real Azure. Apache 2.0.
- **[azure-identity-admin-handbook](https://github.com/f-leroy/azure-identity-admin-handbook)** — Production patterns for Microsoft Entra ID: Conditional Access, PIM, AiTM / token-theft / consent-phishing runbooks, hardening checklist, Graph PowerShell, KQL.
- **[azure-infrastructure-guide](https://github.com/f-leroy/azure-infrastructure-guide)** — Breaking changes, compliance frameworks, Terraform best practices for production Azure.
- **[awesome-az-305-francais](https://github.com/f-leroy/awesome-az-305-francais)** 🇫🇷 — Ressources françaises pour la certification AZ-305.

---

### 🛠️ Tech

`Terraform` · `Ansible` · `Packer` · `Azure` · `Oracle 19c` · `SQL Server` · `PostgreSQL` · `MySQL` ·
`CosmosDB` · `Python` · `GitHub Actions (OIDC)` · `Key Vault` · `Docker`

<sub>Open to **Azure infrastructure, database automation and Oracle→PostgreSQL migration** work.</sub>
