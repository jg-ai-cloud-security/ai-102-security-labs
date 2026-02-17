\# AI-102 Day 10 — Secure GenAI RAG (Baseline)



\## Overview

This lab builds a secure baseline for a GenAI Retrieval-Augmented Generation (RAG) architecture on Azure.

The goal is to establish secure foundations (identity, secrets, logging) before adding private networking and full RAG indexing/testing in later days.



\## Objectives

\- Deploy core services required for a secure GenAI RAG baseline

\- Store secrets securely (no hardcoded keys)

\- Use RBAC-ready access approach and least privilege

\- Enable diagnostics and validate logging with KQL

\- Capture evidence and diagrams for portfolio-ready documentation

\- Delete resources after validation to avoid ongoing cost



\## ## Diagrams (Deferred)

Architecture diagrams will be added in a follow-up update.

Evidence screenshots and KQL validation are complete for Day 10.



\## Services Deployed

\- Azure OpenAI (model deployment configured)

\- Azure AI Search

\- Key Vault (RBAC permission model)

\- Log Analytics workspace

\- Diagnostic settings to Log Analytics



\## Security Controls Implemented

\- Secrets stored in Key Vault (no secrets in code/notes)

\- RBAC-based access model (least privilege design)

\- Centralized monitoring enabled via diagnostic settings → Log Analytics



\## Monitoring \& Validation

\- Diagnostic settings enabled for Key Vault, Search, and OpenAI

\- KQL run in Log Analytics to confirm operational visibility (AzureActivity / AzureDiagnostics)



\## Evidence

Screenshots are stored in:

\- `/04-Evidence (screenshots)/`



Optional supporting files:

\- `EvidenceIndex.md` (what each screenshot proves)

\- `ChangeLog.md` (what changed today)



\## Cleanup (Cost Control)

\- All resources deleted after evidence capture to avoid cost.



\## Next Steps (Day 11)

\- Rebuild baseline quickly

\- Implement Private Endpoints + Private DNS for Key Vault / Search / OpenAI

\- Disable public network access (where supported)

\- Capture proof + update diagrams + delete resources again



\## Repo Structure

\- `01-Plan/`

\- `02-Architecture/`

\- `03-Deployment-Steps/`

\- `04-Evidence (screenshots)/`

\- `05-KQL/`

\- `06-Diagrams/`

\- `07-Cleanup/`



