<div align="center">

# ☁️ Gaurav Dubey
### Azure Cloud & DevOps Engineer | Terraform | Infrastructure as Code | CI/CD

<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&duration=3000&pause=1000&color=0078D4&center=true&vCenter=true&width=650&lines=Azure+Cloud+%26+DevOps+Engineer;Terraform+%7C+Modular+Infrastructure+as+Code;Automated+CI%2FCD+Pipelines+(DevOps+%26+GitHub);DevSecOps+%7C+Policy-as-Code+%26+Security;Parent-Child+Terraform+Architectures" alt="Animated Typing Banner" />
  </a>
</p>

<p align="center">
  <a href="https://gauravdubey.pages.dev/">
    <img src="https://img.shields.io/badge/Portfolio-8B5CF6?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Portfolio Website" />
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/gauravdubey5">
    <img src="https://img.shields.io/badge/LinkedIn-0078D4?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn Profile" />
  </a>
  &nbsp;
  <a href="https://github.com/gauravdubey5">
    <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Profile" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Status-Open%20to%20Opportunities%20(DevOps%20%7C%20Cloud%20Engineer)-0E8A16?style=flat-square&logo=azuredevops&logoColor=white" alt="Open to Opportunities" />
  &nbsp;
  <img src="https://img.shields.io/badge/Focus-Infrastructure%20as%20Code%20%7C%20CI%2FCD-0078D4?style=flat-square&logo=terraform&logoColor=white" alt="Current Focus" />
</p>

</div>

---

## 🎯 Executive Summary & About Me

I am an early-career **Azure Cloud & DevOps Engineer** with a **B.Tech in Computer Science & Engineering**, focused on architecting resilient, automated, and secure cloud platforms. My engineering practice centers on **declarative Infrastructure as Code (IaC)**, **immutable delivery pipelines**, and **shift-left security governance**.

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                                CORE ENGINEERING PILLARS                                │
├──────────────────────────┬─────────────────────────────┬───────────────────────────────┤
│  ☁️ Cloud Architecture   │  🏗️ Modular Terraform       │  🔄 CI/CD & DevSecOps         │
│  - Azure Virtual Networks│  - Parent-Child Repositories│  - Azure DevOps & GitHub Acts │
│  - Hub-Spoke Topologies  │  - Git Tag Version Pinning  │  - Automated Plan/Apply Gates │
│  - Azure Policy & RBAC   │  - Reusable Child Modules   │  - tfsec, Checkov & TFLint    │
│  - Compute & Storage IaaS│  - Remote State Management  │  - Bash, PowerShell & Linux   │
└──────────────────────────┴─────────────────────────────┴───────────────────────────────┘
```

- **Cloud Infrastructure:** Architecting Microsoft Azure foundations, virtual networking, identity access governance, and resource lifecycle management.
- **Modular Terraform:** Designing decoupled, production-grade Terraform modules featuring clear input/output contracts, immutable Git release tags, and remote state locking.
- **Continuous Delivery:** Engineering multi-stage CI/CD pipelines in Azure DevOps and GitHub Actions with automated code verification and deployment approvals.
- **DevSecOps & Reliability:** Embedding automated security scanning, policy compliance checks, and configuration hygiene into every pull request.

---

## 🛠️ Technical Competency Matrix

<div align="center">

<p align="center">
  <img src="https://skillicons.dev/icons?i=azure,terraform,githubactions,linux,bash,powershell,py,docker,kubernetes,git&theme=dark" alt="Core Technologies" />
</p>

</div>

| Domain | Core Technologies & Tools | Engineering Scope |
| :--- | :--- | :--- |
| **Cloud Platform** | `Microsoft Azure` `Azure Portal` `Azure CLI` | Virtual Networks (VNets), Hub-Spoke Topology, Resource Groups, Subnets, NSGs, Public IPs, NICs, Route Tables, NAT Gateways, Storage Accounts |
| **Infrastructure as Code** | `Terraform` `HCL` `Terraform Cloud` | Parent-Child Architecture, Custom Modules, Remote State Locking, Dependency Injection, Git Tag Versioning |
| **CI/CD & Automation** | `Azure DevOps` `Azure Pipelines` `GitHub Actions` `YAML` | Multi-stage build/release pipelines, Service Principal authentication, automated approval gates, secret management |
| **Operating Systems** | `Linux (Ubuntu / Debian)` `Windows Server` | System administration, package management, service configuration, file permission hardening |
| **Scripting & Tooling** | `Bash` `PowerShell` `Python` `Git` | Infrastructure automation scripts, CLI wrappers, Git workflows, PR reviews |
| **Containers & Orchestration** | `Docker` `Kubernetes (AKS Fundamentals)` | Containerization, Dockerfile optimization, multi-container stacks, cluster basics |
| **DevSecOps & Code Quality** | `tfsec` `Checkov` `TFLint` `terraform fmt` | Static code analysis, security scanning, policy drift prevention, vulnerability mitigation |

---

## 🏛️ Terraform Architecture Showcase: Parent-Child Pattern

A core hallmark of enterprise Infrastructure as Code is decoupling environment orchestration from underlying resource definitions. In my projects, I implement an enterprise **Parent-Child Terraform Architecture** utilizing dedicated Git repositories, semantic version pinning, and explicit output-to-input parameter binding.

### Architecture Topology Diagram

```mermaid
flowchart TD
    subgraph Parent["Root / Parent Repository (Environment Orchestration)"]
        ParentRoot["<b>parent-enterprise-infrastructure</b><br/><i>(Environment State, Providers, Variable Assignments)</i>"]
    end

    subgraph Modules["Decoupled Child Modules (Git Repositories with Version Tags)"]
        direction TB
        RG["📦 <b>Resource Group Module</b><br/><code>git source | tag: v1.0.0</code>"]
        VNET["🌐 <b>Virtual Network Module</b><br/><code>git source | tag: v1.2.0</code>"]
        SUBNET["🔀 <b>Subnet Module</b><br/><code>git source | tag: v1.1.0</code>"]
        NSG["🛡️ <b>Network Security Group Module</b><br/><code>git source | tag: v1.0.1</code>"]
        PIP["📍 <b>Public IP Module</b><br/><code>git source | tag: v1.0.0</code>"]
        NIC["🔌 <b>Network Interface Module</b><br/><code>git source | tag: v1.0.3</code>"]
        RT["🗺️ <b>Route Table Module</b><br/><code>git source | tag: v1.0.0</code>"]
        NAT["⚡ <b>NAT Gateway Module</b><br/><code>git source | tag: v1.0.0</code>"]
    end

    ParentRoot -->|"Calls and Pins v1.0.0"| RG
    ParentRoot -->|"Calls and Pins v1.2.0"| VNET
    ParentRoot -->|"Calls and Pins v1.1.0"| SUBNET
    ParentRoot -->|"Calls and Pins v1.0.1"| NSG
    ParentRoot -->|"Calls and Pins v1.0.0"| PIP
    ParentRoot -->|"Calls and Pins v1.0.3"| NIC
    ParentRoot -->|"Calls and Pins v1.0.0"| RT
    ParentRoot -->|"Calls and Pins v1.0.0"| NAT

    VNET -.->|"rg_name = module.rg.name"| RG
    SUBNET -.->|"vnet_name = module.vnet.name"| VNET
    NSG -.->|"subnet_id = module.subnet.id"| SUBNET
    NIC -.->|"subnet_id and pip_id"| SUBNET
    NIC -.-> PIP
    NAT -.->|"subnet_association"| SUBNET
    RT -.->|"subnet_association"| SUBNET

    classDef parentStyle fill:#0F172A,stroke:#0078D4,stroke-width:2px,color:#F8FAFC;
    classDef moduleStyle fill:#1E293B,stroke:#8B5CF6,stroke-width:1.5px,color:#F8FAFC;
    class ParentRoot parentStyle;
    class RG,VNET,SUBNET,NSG,PIP,NIC,RT,NAT moduleStyle;
```

### Architectural Principles

* **Git-Based Module Sourcing:** Modules are maintained in dedicated repositories or versioned directories, preventing monolithic code drift.
* **Strict Semantic Version Pinning:** Child modules are referenced with immutable Git tags (`?ref=v1.2.0`), guaranteeing reproducible builds across dev, staging, and production environments.
* **Explicit Dependency Mapping:** Downstream modules consume upstream outputs (e.g., `module.rg.name` → `module.vnet.resource_group_name`), ensuring deterministic dependency resolution.
* **Isolated Blast Radiuses:** Changes to individual child modules undergo standalone validation and tagging before adoption by parent root configurations.
* **Automated CI/CD Integration:** Pipelines authenticate via Service Principals or System Access Tokens to clone private module repositories during `terraform init`.

---

## 🚀 Featured Engineering Projects

### 1. Enterprise Azure Landing Zone
**Scalable Cloud Foundation & Hub-Spoke Network Architecture**

An enterprise-ready Azure Landing Zone implementing security baselines, identity controls, and a transit Hub-Spoke network topology managed strictly via Terraform.

* **Hub-Spoke Topology:** Centralized transit network isolating egress firewall and management bastions from application workloads.
* **Governance as Code:** Integration with Azure Policy to enforce regional deployment guardrails and resource tagging.
* **Zero-Trust Network Controls:** Layered Network Security Groups (NSGs) restricting inter-subnet lateral movement.

```mermaid
flowchart LR
    Hub["<b>Hub VNet</b><br/>Firewall and Bastion"] <-->|"Peering"| SpokeApp["<b>Spoke VNet</b><br/>Application Tier"]
    Hub <-->|"Peering"| SpokeData["<b>Spoke VNet</b><br/>Data Tier"]
    SpokeApp -.->|"Egress via Firewall"| Hub
```

- **Tech Stack:** `Azure` `Terraform` `Hub-Spoke VNet` `Azure Policy` `DevSecOps`
- **GitHub Repository:** [Enterprise-Azure-Landing-Zone](https://github.com/gauravdubey5/Enterprise-Azure-Landing-Zone)

---

### 2. Terraform Enterprise Infrastructure
**Modular Parent-Child Infrastructure Orchestration**

A production-grade infrastructure deployment framework demonstrating the clean separation of environment orchestration from reusable child modules.

* **Decoupled Architecture:** Reusable child modules for Resource Groups, VNets, Subnets, NSGs, NICs, and Public IPs.
* **Version-Pinned Releases:** Invocations locked via Git semantic tags to prevent breaking changes and unplanned drift.
* **State Isolation:** Remote backend architecture utilizing Azure Blob Storage with state locking and encryption at rest.
* **Automated Validation:** Pre-commit linting and HCL formatting checks integrated into pipeline triggers.

```
parent-infrastructure/
├── main.tf          # Module calls with ?ref=vX.Y.Z
├── variables.tf     # Environment variables
├── outputs.tf       # Exported resource identifiers
└── terraform.tfvars # Environment values
```

- **Tech Stack:** `Terraform` `Azure RM` `Modular IaC` `Git Tags` `Remote State`
- **GitHub Repository:** [terraform-enterprise-infrastructure](https://github.com/gauravdubey5/terraform-enterprise-infrastructure)

---

### 3. GitHub Actions Pipeline Automation
**End-to-End Infrastructure CI/CD with Shift-Left Security**

An automated multi-stage CI/CD workflow designed to validate, test, scan, and deploy cloud infrastructure with zero manual overhead.

* **Static Analysis:** Automated execution of `terraform fmt -check` and `tflint` on every pull request.
* **Security Scanning:** Shift-left security scans powered by `tfsec` to block misconfigurations before code merges.
* **Speculative Plans:** Automated generation and commenting of `terraform plan` summaries directly on pull requests.
* **Protected Deployments:** Manual environment approval gates required prior to production execution.

```mermaid
flowchart LR
    Push["PR / Push"] --> Lint["fmt and tflint"]
    Lint --> Sec["tfsec Scan"]
    Sec --> Plan["terraform plan"]
    Plan --> Gate{{"Approval Gate"}}
    Gate --> Apply["terraform apply"]
```

- **Tech Stack:** `GitHub Actions` `CI/CD` `YAML` `tfsec` `TFLint` `Automation`
- **GitHub Repository:** [pipeline-using-action](https://github.com/gauravdubey5/pipeline-using-action)

---

### 4. SmartLearn AI – Cloud-Native Platform
**Modern Full-Stack Educational Web Application & Containerization**

A responsive cloud-native learning management platform designed with modular application architecture and containerized deployment readiness.

* **Application Architecture:** Developed with Python, Flask, RESTful endpoints, and modern responsive front-end interfaces.
* **Database & Data Layer:** Relational data schemas optimized for student learning metrics and course tracking.
* **Container Packaging:** Dockerized application image optimized for minimal size and rapid deployment to cloud container instances.
* **Deployment Automation:** Integrated CI/CD workflows for automated build, container packaging, and deployment.

```
SmartLearn-AI/
├── app/             # Application controllers & routes
├── models/          # Relational schemas & database logic
├── static/          # Responsive UI assets & styles
└── Dockerfile       # Container packaging configuration
```

- **Tech Stack:** `Python` `Flask` `Docker` `REST APIs` `Cloud Deployment`
- **GitHub Repository:** [SmartLearn-AI](https://github.com/gauravdubey5/SmartLearn-AI)

---

## 📊 GitHub Analytics & Telemetry

<div align="center">

<table border="0" cellpadding="0" cellspacing="0">
  <tr>
    <td align="center" valign="middle">
      <a href="https://github.com/gauravdubey5">
        <img src="https://github-readme-stats.vercel.app/api?username=gauravdubey5&show_icons=true&theme=radical&hide_border=true&bg_color=0d1117&title_color=0078D4&icon_color=8B5CF6&text_color=c9d1d9" alt="Gaurav's GitHub Stats" />
      </a>
    </td>
    <td align="center" valign="middle">
      <a href="https://github.com/gauravdubey5">
        <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=gauravdubey5&layout=compact&theme=radical&hide_border=true&bg_color=0d1117&title_color=0078D4&text_color=c9d1d9" alt="Top Languages" />
      </a>
    </td>
  </tr>
  <tr>
    <td colspan="2" align="center" valign="middle">
      <br/>
      <a href="https://github.com/gauravdubey5">
        <img src="https://github-readme-streak-stats.herokuapp.com/?user=gauravdubey5&theme=radical&hide_border=true&background=0d1117&ring=0078D4&fire=8B5CF6&currStreakLabel=0078D4" alt="GitHub Streak Stats" />
      </a>
    </td>
  </tr>
</table>

</div>

---

## 🧭 Engineering Focus & Continuous Development

* **Enterprise Kubernetes (AKS):** Exploring production cluster deployment, ingress controllers, Azure CNI networking, and Pod Identity.
* **GitOps & Declarative Delivery:** Deepening knowledge in Git-driven continuous delivery workflows with automated drift correction.
* **Cloud Security & Policy as Code:** Strengthening automated guardrails using Azure Policy, Open Policy Agent (OPA), and Checkov in CI pipelines.
* **Certifications in Progress:** Pursuing continuous Microsoft Cloud certifications (AZ-104: Microsoft Azure Administrator & AZ-400: Microsoft DevOps Solutions).

---

## 🎓 Education & Background

* **Bachelor of Technology (B.Tech)** — Computer Science & Engineering
* **Core Foundation:** Computer Networks, Operating Systems, Cloud Computing, System Architecture, Object-Oriented Programming, and Database Management Systems.

---

## 🤝 Let's Connect & Collaborate

I am actively seeking **DevOps Engineer** and **Azure Cloud Engineer** roles where I can contribute to building resilient, automated cloud infrastructure. Let's discuss cloud architecture, automation, or potential opportunities!

<p align="center">
  <a href="https://www.linkedin.com/in/gauravdubey5">
    <img src="https://img.shields.io/badge/LinkedIn-Gaurav%20Dubey-0078D4?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" />
  </a>
  &nbsp;
  <a href="https://gauravdubey.pages.dev/">
    <img src="https://img.shields.io/badge/Portfolio-gauravdubey.pages.dev-8B5CF6?style=for-the-badge&logo=google-chrome&logoColor=white" alt="Visit Portfolio" />
  </a>
  &nbsp;
  <a href="https://github.com/gauravdubey5">
    <img src="https://img.shields.io/badge/GitHub-gauravdubey5-181717?style=for-the-badge&logo=github&logoColor=white" alt="Explore GitHub" />
  </a>
</p>

<div align="center">
  <sub>Designed with precision for Cloud & DevOps excellence • © 2026 Gaurav Dubey</sub>
</div>
