# Awesome-Cloud-Migration-Management

# Awesome-Cloud-Migration-Management

**Top Cloud Migration Management (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Migration Assessment, Workload Mobility, Dependency Mapping & Open Migration Tooling*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Migration Management**. These tools enable organizations to discover on-premises workloads, assess cloud readiness, plan migration waves, and execute cutovers with minimal downtime—from fully managed hyperscaler migration hubs with AI-driven automation to open-source assessment frameworks and migration orchestration tools that give teams control over their migration lifecycle.



**Examples** include AWS Migration Hub (now AWS Transform), Azure Migrate, Google Cloud Migration Center, RiverMeadow, Carbonite Migrate, Flexera One, Turbonomic, CAST Highlight, and Atlassian Cloud Migration Assistant (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted migration assessment, workload planning, and open migration infrastructure. **Critical note**: The open-source cloud migration landscape is nascent—**Cloud Migration MCP Server** is the most structured open-source assessment and wave-planning tool, but it is a CLI/MCP utility rather than a full platform. **CloudHop** and **Skyferry** address data movement rather than migration management. No open-source project matches Azure Migrate's end-to-end discovery-to-execution pipeline or Carbonite Migrate's block-level replication at scale.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global cloud migration services and software ecosystem is estimated between **$300B to $400B+** (with specialized core software and orchestration tools accounting for ~$15B–$40B, expanding at a ~23–28% CAGR driven by generative AI infrastructure demands and hybrid cloud deployments). The market is **moderately fragmented yet tiered**: underlying migration hubs and hypervisor cutovers are concentrated around hyperscalers (AWS, Microsoft, Google), enterprise implementations are led by global systems integrators (GSIs), and specialized assessment, code refactoring, and multi-cloud mobility segments remain distributed across independent software vendors (ISVs).

## SaaS/Hosted Platforms

| Company / Product | Company Size (Market Cap / Valuation / Revenue) | Pricing (Specific Starting Tiers) | Free Tier / Trial Limits | Key Capabilities & Migration Focus |
| :--- | :--- | :--- | :--- | :--- |
| **[Azure Migrate](https://azure.microsoft.com/en-us/products/azure-migrate)** (Microsoft) | ~$3.1T Market Cap (~$245B Ann. Rev.) | **Free core tool** (Discovery, assessment, & TCO planning are $0.00; target cloud infrastructure billed separately, e.g. Azure VMs from ~$0.0104/hr) | **Free forever**: Full discovery, dependency analysis, and assessment; includes $200 Azure credit for 30 days for target infra testing | Hyperscaler discovery and migration platform for VMware, Hyper-V, physical servers, and SQL databases to Azure. |
| **[AWS Transform](https://aws.amazon.com/transform/)** (Amazon AWS) | ~$2.2T Market Cap (~$600B+ Ann. Rev.) | **$0.035 / active agent minute** for custom code modernization; assessments & workload agents are $0.00 platform fee; target infra billed at standard AWS rates | **Free tier**: 50,000 agent minutes/mo free for AWS-managed .NET transformations; free assessments and workload planning; $0 platform fee for MGN | Agentic AI-powered modernization and migration platform superseding AWS Migration Hub; automates code refactoring and workload migration. |
| **[Google Cloud Migration Center](https://cloud.google.com/migration-center)** (Alphabet) | ~$2.1T Market Cap (~$350B Ann. Rev.) | **Free core tool** (Asset discovery, cost estimation, & planning are $0.00; target GCP compute billed separately, e.g. e2-micro instances) | **Free forever**: Full asset discovery, TCO assessment, & planning; includes 90-day free trial with $300 GCP credits for execution testing | Centralized discovery, assessment, and migration hub for lifting and modernizing workloads into Google Cloud. |
| **[IBM Turbonomic](https://www.ibm.com/products/turbonomic)** (IBM) | ~$215B Market Cap (~$62B Ann. Rev.) | **$37,000 / year** baseline subscription for up to 200 managed virtual servers (approx. ~$22–$25/VM/month) | **30-day free trial**: Full access for cloud and on-prem workload resource modeling and migration planning; no credit card required | Application Resource Management (ARM) providing multi-cloud migration planning, right-sizing, and reserved instance cost modeling. |
| **[Atlassian Cloud Migration Assistant](https://www.atlassian.com/)** (Atlassian) | ~$52B Market Cap (~$5.2B Ann. Rev.) | **Free tool included** with Atlassian Cloud plans (Jira Cloud Standard starts at **$8.15 / user / month**) | **Free forever plan**: Up to 10 users and 2 GB storage; or **60-day to 12-month free Cloud Migration Trial** matching existing Data Center tier | Native migration utility (JCMA/CCMA) for migrating Jira, Confluence, and app data from on-premises Data Center to Atlassian Cloud. |
| **[Carbonite Migrate](https://www.carbonite.com/cloud-migration/)** (OpenText) | ~$7.8B Market Cap (~$5.2B Ann. Rev.) | **$500 / server node** starting license (Standard 60-day migration window; volume pricing and multi-packs available) | **Proof of Concept / Eval**: Custom evaluation license provisioned by sales (typically 30 to 60-day validity window per target node) | Byte-level, real-time replication migration engine enabling near-zero downtime cutovers across physical, virtual, and multi-cloud environments. |
| **[Flexera One Cloud Migration Planning](https://www.flexera.com/solutions/cloud-cost/cloud-migration-planning)** (Flexera / Thoma Bravo) | ~$2.8B Valuation (~$290M+ Ann. Rev.) | **$13,000 / year** starting annual scoped contract (FinOps modules scale at ~1–5% of managed cloud spend, or ~$50,000/yr for $1M spend) | **Custom Demo & Trial**: Guided sandbox and custom trial tenant access via sales request; no perpetual self-serve free tier | Workload placement, dependency mapping, multi-cloud cost modeling, and 6R strategy scoring. |
| **[CAST Highlight](https://www.castsoftware.com/products/highlight)** (Bridgepoint Group) | ~$150M (€139M) Valuation (~$50M+ Ann. Rev.) | **$6,800 / year** for a single named application (Complete Insights); portfolio Cloud Insights edition starts at **$30,800 / year** | **14-day free trial**: Access to pre-loaded sample application portfolio and code scanning engine for cloud blocker detection | Static source code intelligence engine scanning 50+ languages for cloud migration blockers, container readiness, and 5R disposition. |
| **[RiverMeadow](https://www.rivermeadow.com/)** | ~$50M–$100M Valuation (~$6M–$8M Ann. Rev.) | **$250 / workload instance** baseline migration fee (or bundled fixed-fee packages starting around ~$3,900 on AWS/Azure Marketplaces) | **Proof of Concept**: 30-day guided evaluation pilot with 5–10 workload migration entitlements upon sales consultation | Multi-cloud workload mobility and automated modernization platform providing pre-flight assurance, OS upgrades, and cutover automation. |

## Open-Source GitHub Projects



- **[Cloud Migration MCP Server](https://github.com/chrishorne74/cloud-migration-mcp)**

  **MCP server for cloud migration assessment and planning** (license per repo) — **the most structured open-source tool for migration strategy and wave planning** found in this research . **Features**: **7 Rs Strategy Engine**—recommends Rehost, Replatform, Repurchase, Refactor, Retire, Retain, or Relocate based on workload attributes. **Migration Assessment**—scores workloads 0–100 across 10 weighted criteria (business criticality, technical complexity, vendor support, cloud readiness, cost, age, SaaS availability, data sensitivity, documentation, compliance). **30+ built-in guardrails** across Dependency, Security, Compliance, Data, Architecture, Operations, and Cost categories—editable at runtime. **Candidate Scoring & Ranking**—rank up to 50 workloads. **Wave Planning**—group workloads into sequenced migration waves respecting dependencies. **Cost Estimation**—ROM (±50%) with cloud annual cost, one-time migration cost, 1/3-year savings, and ROI break-even. **Draw.io Diagrams**—generates migration architecture diagrams using native AWS/Azure/GCP shapes . **Tech stack**: MCP server. **Deploy**: Self-hosted MCP server; accessible via Claude Desktop, Cursor, or other MCP clients. **Trade-off**: **Assessment and planning only**—does not execute migrations or connect to cloud APIs for discovery. Requires manual workload input. **Best for**: architects and migration leads wanting structured 7R assessment, guardrail checking, and wave planning—especially those already using AI assistants via MCP.



- **[CloudHop](https://github.com/ozymandiashh/cloudhop)**

  **Free, open-source GUI for cloud-to-cloud file transfers** (MIT) — **the most user-friendly open-source tool for bulk data migration between cloud storage providers** . **Features**: **Wraps rclone** in a visual interface for 70+ cloud storage providers; live dashboard with speed charts, ETA, and file counts; pause, resume, and schedule transfers; copy, sync, or two-way bisync modes; **files route directly between clouds through your local connection**—never through external servers; no accounts, no tracking . **Tech stack**: Python, pywebview, vanilla JS, rclone. **Deploy**: `pip install cloudhop`; native installers for Mac/Windows; Docker . **Trade-off**: **File transfer only**—not workload migration, infrastructure assessment, or dependency mapping. Local machine must stay online during transfers. **Best for**: teams needing to move data between cloud storage providers (OneDrive to Google Drive, S3 to Azure Blob) without paid per-GB services or rclone CLI complexity.



- **[Skyferry](https://github.com/cubetribe/skyferry)**

  **Patient, verified, resumable Google Drive migration tool** (license per repo) — **the most rigorous open-source tool for large-scale Drive-to-Drive migrations** . **Features**: **Unit-based migration**—folders split above size threshold; state machine from PLANNED through DONE with side states for FAILED and NEEDS_ATTENTION; **MD5 verification** at local and remote stages; **crash-proof** with resumable downloads and uploads; **push alerts** via ntfy and healthchecks.io; bandwidth scheduling (e.g., `08:00,20M 23:00,off`); append-only audit trail; systemd service for unattended operation . **Tech stack**: Python, rclone, Linux. **Deploy**: Dedicated Linux server with buffer disk; systemd user service. **Trade-off**: **Google Drive-specific**—not a general cloud migration tool. Requires a Linux server with sufficient buffer disk. **Best for**: organizations migrating large Google Drive estates (hundreds of GB to TB) needing verification and resumability—especially when network reliability is a concern.



### Additional Strong Open-Source Options



- **xmigrate** — Cloud migration tool for on-premises data and infrastructure (Python, ~43 stars). **Note**: Minimal documentation available; last activity ~11 months ago per metadata . **Best for**: exploration only—not production-ready without significant validation.

- **Accenture SWAO** — AI-accelerated cloud workload compliance assessment (Community Edition binaries). Scans code for sovereign risk factors, compliance mapping (GDPR/HIPAA/PCI), and migration recommendations via CLI, TUI, or MCP server . **Note**: **Source not yet published**—binaries only; licensed tiers for full features. **Best for**: organizations needing compliance-focused workload assessment, not general migration management.



**Frameworks for building custom systems**: Combine **Cloud Migration MCP Server** for 7R assessment and wave planning with **CloudHop** for bulk data transfer between storage providers and **Skyferry** for verified large-scale Drive migrations—creating a lightweight open-source migration toolkit. **None of these match Azure Migrate's end-to-end discovery-to-execution pipeline or Carbonite Migrate's block-level replication**; those require commercial platforms or hyperscaler tooling.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Cloud migration platforms handling infrastructure credentials and data must comply with data protection regulations (GDPR, CCPA, etc.) and implement appropriate access controls during migration.

- **The "hyperscaler migration hub" vs. "workload mobility" vs. "assessment/planning" vs. "data transfer" distinction is critical.** **AWS Transform, Azure Migrate, and Google Cloud Migration Center** are **hyperscaler hubs**—they provide discovery, assessment, and execution within their cloud ecosystem. **RiverMeadow and Carbonite Migrate** are **workload mobility**—they replicate and cut over servers with minimal downtime. **Flexera One and CAST Highlight** are **assessment/planning**—they analyze cost and code readiness but do not execute migrations. **Cloud Migration MCP Server** is **assessment/planning**—it scores workloads and plans waves but does not migrate. **CloudHop and Skyferry** are **data transfer**—they move files between storage providers, not workloads. **Choose based on whether you need to decide, plan, migrate, or move data.**

- **AWS Migration Hub is closed to new customers.** Do not start new projects there—**AWS Transform** is the successor with AI-driven automation and all Migration Hub capabilities . Existing projects continue to function, but new planning should use Transform.

- **Azure Migrate's assessment is free**—discovery, readiness assessment, cost estimation, and dependency analysis cost nothing; you pay only for Azure resources consumed . **This is the most generous assessment offering among hyperscalers** and worth evaluating even if you ultimately migrate elsewhere.

- **CloudEndure Migrate is discontinued.** AWS Application Migration Service (MGN) is the recommended lift-and-shift service . **Do not evaluate CloudEndure as a current option**—references in older documentation are outdated.

- **Cloud Migration MCP Server is the most structured open-source migration planning tool**—it codifies the 7 Rs, guardrails, and wave planning in a way that can be invoked by AI assistants . **The trade-off**: it is assessment and planning only—no discovery, no execution. **For teams wanting a rigorous planning framework they can run locally, it is the best open-source option.**

- **CloudHop and Skyferry solve different problems.** CloudHop is for **cloud-to-cloud file transfers** (OneDrive to Google Drive) with a GUI. Skyferry is for **Google Drive-to-Drive migrations** with verification and resumability . **Neither is a workload migration tool.**

- **Pricing opacity varies.** Azure Migrate assessment is free . Google Cloud Migration Center is free for assessment with $300 credits. RiverMeadow, Carbonite, Flexera, Turbonomic, and CAST Highlight require sales contact. AWS Transform is consumption-based. **Validate with direct vendor conversations against your migration scope and downtime tolerance.**

- Self-hosted open-source solutions require proper setup, credentials for cloud storage APIs, and ongoing maintenance. **Migration tools handle production data and infrastructure credentials**—ensure your deployment meets your organization's security standards before initiating cutovers.



---



**Made for migration architects, cloud engineers, and organizations building transparent cloud migration management solutions.**

Let's make Cloud Migration Management more open, data-driven, and cutover-safe.
