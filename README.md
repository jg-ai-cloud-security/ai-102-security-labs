# ai-102-security-labs



\# AI-102 — Azure AI Engineer Associate (Security Labs)



This repository documents my \*\*hands-on learning journey\*\* for the \*\*Microsoft AI-102 (Azure AI Engineer Associate)\*\* certification, built with a \*\*security-first / SOC-ready mindset\*\*.



These labs focus on deploying Azure AI solutions the way real customers expect:

\*\*private networking, identity-based access, centralized logging, secure GenAI/RAG patterns, and cost governance\*\*.



\*\*Author:\*\* Jose Garcia  

\*\*Brand:\*\* JG AI Cloud Security



---



\## What You’ll Find Here



\- End-to-end AI-102 labs with \*\*secure deployment patterns\*\*

\- Evidence-driven builds: \*\*screenshots, notes, diagrams, and architecture explanations\*\*

\- Operational thinking: \*\*monitoring, logging, governance, and cleanup discipline\*\*

\- A portfolio-style structure that is easy to review and repeat



---



\## Objectives



\- Build and secure Azure AI solutions (Language, Vision, Document Intelligence, Azure OpenAI, AI Studio)

\- Implement \*\*secure GenAI\*\* patterns (RAG, prompt hardening, safe data access)

\- Enforce least privilege using \*\*Microsoft Entra ID RBAC + Managed Identity\*\*

\- Enable \*\*Diagnostic Settings → Log Analytics\*\* (SOC-ready telemetry foundation)

\- Apply network hardening (Private Endpoints / restricted public access where possible)

\- Apply \*\*cost governance\*\* (budgets, alerts, and resource cleanup)



---



\## Skills Demonstrated



\- Azure AI services deployment \& configuration

\- Secure Azure OpenAI / Azure AI Studio implementation

\- RAG architecture + security hardening

\- Managed Identity, RBAC, Key Vault secret management

\- Diagnostic logs, Log Analytics, basic KQL where relevant

\- Secure networking: VNets, Private Endpoints, firewall/NSG concepts

\- Responsible AI monitoring and governance controls



---



\## Labs Index



> Each folder represents one lab day and includes its own README with: Overview, Resources, Security Controls, Architecture, Evidence, Lessons Learned.



\- \[Day 02 — Language Service Hardening](./AI-102Day-02-Language-Service-Hardening/)

\- \[Day 03 — Core AI Services Security](./AI-102Day-03-Core-AI-Services-Security/)

\- \[Day 04 — Operationalise CLU](./AI-102Day-04-Operationalise-CLU/)

\- \[Day 05 — Vision + Document Intelligence](./AI-102Day-05-Vision-DocumentIntelligence/)

\- \[Day 06 — End-to-End Secure Deployment](./AI-102Day-06-EndToEnd-Secure-Deployment/)

\- \[Day 07 — GenAI RAG](./AI-102Day-07-GenAI-RAG/)

\- \[Day 08 — Secure AI Deployment](./AI-102Day-08-Secure-AI-Deployment/)

\- \[Day 09 — Secure OpenAI](./AI-102Day-09-Secure-OpenAI/)

\- \[Day 10 — Secure GenAI RAG](./AI-102Day-10-Secure-GenAI-RAG/)

\- \[Day 11 — Responsible AI + Monitoring + Governance](./AI-102Day-11-ResponsibleAI-Monitoring-Governance/)

\- \[Day 12 — Exam Readiness Capstone](./AI-102Day-12-Exam-Readiness-Capstone/)



---



\## Security Baseline Used Across This Repo



\- Prefer \*\*RBAC over keys\*\*

\- Use \*\*Managed Identity\*\* for workloads (Logic Apps, Functions, Apps)

\- Use \*\*Key Vault\*\* for secrets (only if keys must exist)

\- Enable \*\*Diagnostic Settings\*\* and route logs to \*\*Log Analytics\*\*

\- Prefer \*\*private networking\*\* (Private Endpoint / VNet integration) where supported

\- Apply \*\*cost controls\*\* (budgets, alerts) + delete resources after evidence capture



---



\## How To Use This Repo



1\. Open the \*\*Labs Index\*\* above and choose a Day folder

2\. Follow the \*\*Day README\*\* and the `/02-Lab-Guide/`

3\. Review `/07-Architecture/` and `/06-Diagrams/` to understand the design decisions

4\. Use `/03-Screenshots/` as evidence of what was built and configured



---



\## Cost Hygiene



To avoid unexpected charges:

\- Use lower-cost tiers where possible (e.g., F0/S0 where available)

\- Set budgets and alerts

\- Delete resources after screenshots/evidence is captured

\- Keep a short “cleanup checklist” at the end of each day’s README



---



\## Disclaimer



This repository is for learning and portfolio demonstration.  

All sensitive values are masked in screenshots. Resource names are examples and may vary per environment.

