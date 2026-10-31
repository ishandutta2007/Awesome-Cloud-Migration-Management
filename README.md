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
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[AWS Transform](https://aws.amazon.com/transform/)** (formerly **AWS Migration Hub**)
  **AI-powered migration and modernization service** that supersedes Migration Hub. **Migration Hub stopped accepting new customers on November 7, 2025**; AWS Transform launched in May 2025 and provides all Migration Hub capabilities with enhanced AI-driven automation, improved collaboration, and real-time analytics . Existing Migration Hub projects continue to function; new projects should start in AWS Transform. **Pricing**: Quote-only; consumption-based. **Free tier**: AWS Free Tier applies to some usage. **Best for**: AWS-centric organizations planning large-scale migrations—**note**: do not start new Migration Hub projects; use AWS Transform instead.

- **[Azure Migrate](https://azure.microsoft.com/en-us/products/azure-migrate)**
  **Unified migration platform** for discovering, assessing, and migrating workloads to Azure. **Free service** for discovery, assessment, and planning; partner tools may charge for execution . Supports servers (VMware, Hyper-V, physical), databases (SQL Server), web apps, virtual desktops, and large-scale offline data transfer via Azure Data Box. **Business case** feature estimates on-premises vs. Azure TCO and cash flow comparisons . **Pricing**: Free for assessment; pay for Azure resources consumed. **Free tier**: Yes, migration assessment is free. **Best for**: Microsoft-centric organizations wanting a single portal for the full migration journey—**trade-off**: execution tooling is Azure-specific.

- **[Google Cloud Migration Center](https://cloud.google.com/migration-center)**
  **Unified migration platform** for end-to-end migration from on-premises or other clouds to Google Cloud. Provides **cloud spend estimation**, **asset discovery**, and tools for various migration scenarios including **Migrate for VMs** and **Migrate to Containers** for application modernization . **Pricing**: Free for assessment and planning; pay for GCP resources. **Free tier**: $300 credits for new customers. **Best for**: GCP-centric organizations wanting integrated discovery, cost estimation, and migration execution.

- **[RiverMeadow](https://www.rivermeadow.com/)**
  **Workload mobility platform** for multi-cloud and private cloud migrations. Provides **pre-flight assurance** (readiness library, confidence scoring, remediation), **automation and migration extensions** for post-cutover operationalization, **post-flight validation** comparing migrated targets to source baselines, and **portfolio reporting** across migration programs . **Pricing**: Quote-only. **Free tier**: None. **Best for**: enterprises needing governed, evidence-backed migration programs with readiness gates and UAT tracking.

- **[Carbonite Migrate](https://www.carbonite.com/cloud-migration/)** (OpenText)
  **Real-time replication-based migration** for physical, virtual, and cloud workloads with **minimal downtime** (minutes to seconds). Continuous replication keeps a live copy synchronized; cutover can be manual or automated . Supports Windows Server, RHEL, Oracle Linux, SUSE, CentOS, Ubuntu; VMware, Hyper-V, AWS, Azure, Google Cloud . **Pricing**: Quote-only; per-server licensing. **Free tier**: Trial available. **Best for**: organizations needing near-zero downtime cutovers for mission-critical workloads—**note**: CloudEndure Migrate was discontinued; AWS Application Migration Service is the AWS-native alternative.

- **[Flexera One Cloud Migration Planning](https://www.flexera.com/solutions/cloud-cost/cloud-migration-planning)**
  **Migration planning and cost assessment** within Flexera One. Provides **application dependency mapping**, **cloud cost comparisons** across providers, **workload placement** recommendations, and **migration strategy** (rehost, replatform, retire) based on business impact and technical fit . Gartner reviewers note the cost comparison is useful for informed decisions but the initial profile creation is time-consuming . **Pricing**: Quote-only. **Free tier**: None. **Best for**: organizations wanting cost-driven migration decisions and multi-cloud comparison—**trade-off**: reporting customization is limited per reviewers.

- **[IBM Turbonomic](https://www.ibm.com/products/turbonomic)**
  **Application Resource Management (ARM)** with migration planning capabilities. Configures migration plans to AWS or Azure, selecting VMs, regions, and licensing profiles (BYOL, custom OS mapping) . Includes discount settings for RI/SP to model realistic costs. **Pricing**: Quote-only. **Free tier**: None. **Best for**: organizations wanting to model migration costs with existing discount commitments—**note**: Turbonomic is primarily an optimization tool; migration planning is a secondary capability.

- **[CAST Highlight](https://www.castsoftware.com/products/highlight)**
  **Software intelligence platform** for application portfolio assessment. **Scans source code** (50+ languages) to identify **cloud blockers** (persistent file usage, COM components, etc.), **cloud maturity**, **open-source risks**, and **containerization readiness** . Provides **5R disposition recommendations**, migration wave planning, and effort estimates benchmarked against industry peers . **Pricing**: Quote-only. **Free tier**: None. **Best for**: organizations with large application portfolios needing code-level migration assessment—**trade-off**: requires source code access; not a workload discovery tool for infrastructure.

- **[Atlassian Cloud Migration Assistant](https://www.atlassian.com/)**
  **Native migration tool** for moving Jira and Confluence from Data Center to Cloud. Orchestrates data migration via JCMA (Jira Cloud Migration Assistant); app data migration follows Jira data . **Pricing**: Included with Atlassian Cloud subscriptions. **Free tier**: Limited. **Best for**: Atlassian customers migrating to Cloud—**not** a general-purpose cloud migration tool.

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
