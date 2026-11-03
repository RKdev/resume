# James Keys

**Platform / DevOps Engineer**

Johnson City, TN (open to remote) · [keys@novelbusiness.llc](mailto:keys@novelbusiness.llc) · [linkedin.com/in/james-keys-6a926570](https://www.linkedin.com/in/james-keys-6a926570) · [github.com/RKdev](https://github.com/RKdev)

## Summary

Platform and infrastructure engineer with 20 years in technology, from server racks to cloud-native platforms. Spent eight years as the one-person ops function at a healthcare video-interpreting startup: bootstrapped its Kubernetes platform on GCP, ran production through a private-cluster rebuild, a SOC 2 effort and a four-cluster fleet, and built its ELT data platform. Writes the code too, mainly backend services in Go. Lately building AI-assisted engineering workflows with Claude Code.

## Skills

- **Platform:** Kubernetes (GKE), Docker, Helm, NGINX ingress, cert-manager, Prometheus, Grafana, Linux
- **Google Cloud:** GKE, Cloud SQL, L7 load balancing, Cloud Armor, Identity-Aware Proxy, Compute Engine
- **Data:** Airbyte, BigQuery, dbt, PostgreSQL, Redis, SQL
- **Languages:** Go, Bash, SQL, JavaScript (Vue), PowerShell
- **Security & compliance:** SOC 2 infrastructure controls, WAF and rate limiting, zero-trust access (IAP)
- **AI-assisted engineering:** Claude Code, multi-agent development workflows
- **Earlier stack:** Windows Server, virtual desktop infrastructure, Crestron and BiAmp AV systems

## Experience

### Healthcare video-interpreting startup · Remote · Jun 2018 – Sep 2026

**Senior Infrastructure Engineer** · Apr 2022 – Sep 2026

- Created and ran three non-production GKE clusters alongside production, each with its own Cloud SQL instance; one became a pre-production environment that replaced staging, refreshed with scrubbed production data and used by about 10 developers and 3–4 QA testers.
- Delivered the infrastructure side of a company-wide SOC 2 effort, consolidating per-app ingresses into one GCP L7 load balancer with Cloud Armor WAF rules and rate limiting, and ran the annual backup-and-restore test used as audit evidence.
- Took a Go AI gateway for LLM and speech providers into production on GKE from another team's Helm setup, then traced a production-only failure of real-time sessions to the load balancer's 30-second WebSocket cutoff and gave WebSockets a dedicated 60-minute backend.
- Put self-hosted Airbyte behind Identity-Aware Proxy so the data engineering team could manage its own pipelines instead of routing every change through ops.
- Tightened data freshness alerting after a hung sync froze reports for a weekend, adding a 12-hour no-new-data test; the alerts caught later stalls.
- Took on an ERP integration spanning several systems new to the team, run with an AI orchestration workflow: one planning agent directing multiple Claude Code agents.

**Software Engineer** · Jun 2018 – Apr 2022

- Bootstrapped the company's container platform on Google Kubernetes Engine as a contractor, from first commit to production in about six weeks; its ops repo stayed in use through 2026.
- Designed a git-driven ops workflow that cut developer setup to three tools (git, git-crypt, Docker), so any engineer could connect to an environment and deploy.
- Rebuilt production Kubernetes on a private GKE cluster with Helm and Prometheus monitoring in about two weeks of hands-on work, and moved live traffic between clusters behind DNS with no downtime.
- Built the platform's telephony layer in Go on Vonage APIs (Tokbox SIP, Nexmo Voice), delivered in four client-driven phases; it grew into a core, heavily used part of the platform.
- Replaced manual reporting with a self-hosted ELT stack (Airbyte, BigQuery, dbt), choosing Airbyte over Singer, Meltano and Fivetran, and was sole dbt author for its first eight months.

### The University of Texas at Austin · Austin, TX · Jul 2008 – Jun 2018

**Systems Administrator** · Jul 2013 – Jun 2018

- Moved university computer labs from disk imaging to virtual desktops running on the existing lab hardware.
- Engineered Crestron DigitalMedia AV systems for classrooms and labs, including BiAmp audio programming and Crestron SIMPL+ modules.
- Administered Windows, macOS and Linux server environments: Active Directory and Group Policy, DNS and DHCP, patch management, rack servers and tape backup; automated routine work with PowerShell, Bash and VBScript.
- Advised management on technology options and ran RFPs, vendor negotiations, purchasing and inventory.

**Desktop Support Specialist** · Jul 2008 – Jul 2013

- Managed university computer labs end to end, from unboxing and setup to keeping machines running for students.
- Deployed lab-wide images with multicast imaging, including dual-boot images on Mac hardware, and troubleshot Crestron classroom AV systems.

## Education & Certifications

- **A.A.S., Computer and Network Maintenance**, Lee College, Baytown, TX · 2005 · GPA 3.96, Honor Society (Cisco networking curriculum; internship at ExxonMobil's global network operations center)
- **CompTIA A+** and **CompTIA Network+**
