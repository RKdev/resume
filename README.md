# James Keys

**Platform / DevOps Engineer**

Johnson City, TN (open to remote) · [keys@novelbusiness.llc](mailto:keys@novelbusiness.llc) · [linkedin.com/in/james-keys-6a926570](https://www.linkedin.com/in/james-keys-6a926570) · [github.com/RKdev](https://github.com/RKdev)

## Summary

Platform and infrastructure engineer with 20 years in technology, from server racks to cloud-native platforms. Spent eight years as the one-person ops function at a healthcare technology startup (HIPAA, SOC 2): bootstrapped and ran its Kubernetes platform on GCP, built and ran its ELT data platform, and wrote the Go services behind its telephony, payments and billing, including a NetSuite integration for roughly 2,000 clients. Lately building AI-assisted engineering workflows with Claude Code.

## Skills

- **Platform:** Kubernetes (GKE), Docker, Helm, NGINX ingress, cert-manager, Prometheus, Grafana, Linux
- **Google Cloud:** GKE, Cloud SQL, L7 load balancing, Cloud Armor, Identity-Aware Proxy, Compute Engine
- **Data:** Airbyte, BigQuery, dbt, Dagster, PostgreSQL, Redis, SQL, Looker Studio
- **Payments & billing:** Stripe (payments and invoicing), Braintree/PayPal, usage-based billing, NetSuite ERP integration
- **Languages:** Go, Python, Bash, SQL, JavaScript (Vue), PowerShell
- **Security & compliance:** SOC 2 infrastructure controls, HIPAA (self-hosted internal tools), WAF and rate limiting, zero-trust access (IAP)
- **AI-assisted engineering:** Claude Code, multi-agent development workflows
- **Earlier stack:** Windows Server, virtual desktop infrastructure, Crestron and BiAmp AV systems

## Experience

### Jeenie, Inc. · On-demand video interpreting platform for healthcare · Remote · Jun 2018 – Sep 2026

**Senior Infrastructure Engineer (Platform / DevOps / SRE / Data Platform)** · Apr 2022 – Sep 2026

- Created and ran three non-production GKE clusters alongside production, each with its own Cloud SQL instance, handling deploys, upgrades and troubleshooting across the fleet; one became a pre-production environment that replaced staging, refreshed with scrubbed production data and used by about 10 developers and 3–4 QA testers.
- Delivered the infrastructure side of a company-wide SOC 2 effort, consolidating per-app ingresses into one GCP L7 load balancer with Cloud Armor WAF rules and rate limiting, and ran the annual backup-and-restore test used as audit evidence.
- Moved the company's Retool internal-tools platform to a HIPAA-compliant self-hosted deployment on GKE so it could serve larger healthcare providers, with git-versioned apps and a per-environment instance; built its billing and finance tools.
- Built a three-layer, ERP-agnostic integration (dbt/BigQuery, Python/Dagster) that moved billing for roughly 2,000 clients onto NetSuite in about seven weeks from first commit to production invoicing, with idempotent writes, verify-after-write, dead-letter handling and reconciliation tests; run with a planning agent directing multiple Claude Code agents.
- Ran monthly billing (Go, Stripe) for more than five years across roughly 2,000 clients, verifying each 2–5 day cycle and catching most billing errors before invoices went out.
- Took a Go AI gateway for LLM and speech providers into production on GKE from another team's Helm setup, then traced a production-only failure of real-time sessions to the load balancer's 30-second WebSocket cutoff and gave WebSockets a dedicated 60-minute backend.
- Ran the company's Airbyte ELT pipeline, which fed finance, leadership and operations reporting, through 2026, moving new connectors to a Helm deploy on GKE, putting Airbyte behind Identity-Aware Proxy so the data team could manage its own pipelines, and adding a 12-hour no-new-calls freshness test after a hung sync froze reports for a weekend.

**Software Engineer (DevOps / Backend, Go / Data Engineering)** · Jun 2018 – Apr 2022

- Bootstrapped the company's container platform on Google Kubernetes Engine as a contractor, from first commit to production in about six weeks; its ops repo stayed in use through 2026.
- Designed a git-driven ops workflow that cut developer setup to three tools (git, git-crypt, Docker), so any engineer could connect to an environment and deploy.
- Rebuilt production Kubernetes on a private GKE cluster with Helm and Prometheus monitoring in about two weeks of hands-on work, and moved live traffic between clusters behind DNS with no downtime.
- Built the platform's telephony layer in Go on Vonage APIs (Tokbox SIP, Nexmo Voice), connecting it to hospital, state-agency and call-center phone systems in four client-driven phases; phone and rollover grew to an estimated quarter or more of platform usage by 2026.
- Added PayPal alongside Stripe by integrating Braintree's GraphQL API from Go (live in about three weeks, in production for more than six years), and built prepaid minute packages and overage billing full-stack in Go and Vue.
- Replaced a hand-run morning report with a Go pipeline refreshing leadership's usage and revenue sheet every 15 minutes, the data source for board, investor and quarterly reporting.
- Replaced manual reporting with a self-hosted ELT stack (Airbyte, BigQuery, dbt), choosing Airbyte over Singer, Meltano and Fivetran, and built the dbt financial model that moved the company to accrual accounting ahead of its Series A, signed off by an outside accounting firm.

### The University of Texas at Austin · Austin, TX · Jul 2008 – Jun 2018

**Systems Administrator (Systems Engineer / IT Infrastructure)** · Jul 2013 – Jun 2018

- Moved university computer labs from disk imaging to virtual desktops running on the existing lab hardware.
- Engineered Crestron DigitalMedia AV systems for classrooms and labs, including BiAmp audio programming and Crestron SIMPL+ modules.
- Administered Windows, macOS and Linux server environments: Active Directory and Group Policy, DNS and DHCP, patch management, rack servers and tape backup; automated routine work with PowerShell, Bash and VBScript.
- Advised management on technology options and ran RFPs, vendor negotiations, purchasing and inventory.

**Desktop Support Specialist** · Jul 2008 – Jul 2013

- Managed university computer labs end to end, from unboxing and setup to keeping machines running for students.
- Deployed lab-wide images with multicast imaging, including dual-boot images on Mac hardware, and troubleshot Crestron classroom AV systems.

## Education & Certifications

- **A.A.S., Computer Maintenance Technology**, Lee College, Baytown, TX · 2005 · Graduated with Honor, Phi Theta Kappa (Cisco networking curriculum)
- **Internship:** ExxonMobil Global Operations Center (Lee College capstone) · May–Jul 2004 · Monitored and troubleshot global network circuits, worked with engineers to resolve site outages, and monitored daily backups of worldwide servers
- **Certificates:** Networking Maintenance Technology and Computer Maintenance Technology, Lee College · 2004
- **CompTIA A+** and **CompTIA Network+**
