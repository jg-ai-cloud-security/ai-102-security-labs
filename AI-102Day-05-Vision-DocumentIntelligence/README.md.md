# ai-102-security-labs



\# AI-102 Day 2 — Language Service Hardening



\## Overview

This lab demonstrates deployment and security hardening of Azure AI Language for SOC use cases including phishing analysis and ticket triage.



\## Resources Deployed

\- Service: Azure AI Language

\- Name: ai102-language-jg-lab-001

\- Region: UK South

\- Tier: F0/S0

\- Resource Group: rg-ai102-day2-jg



\## Security Controls Implemented

\- Microsoft Entra ID RBAC (Cognitive Services User)

\- API keys avoided in apps; stored in Key Vault (recommended)

\- Diagnostic logs sent to Log Analytics

\- Managed Identity planned for calling workload

\- Network hardening planned via Private Endpoint



\## SOC Use Case

Inbound emails are processed by a Logic App using Managed Identity. Azure AI Language classifies sentiment, detects phishing indicators and flags malicious content. Logs are streamed to Sentinel for alerting.



\## Architecture

User → Logic App (MI) → Azure AI Language → Log Analytics → Sentinel → Analyst



\## Evidence

Screenshots:

\- Overview

\- IAM role assignment

\- Diagnostic settings

\- Networking

\- Keys blade (masked)



\## Lessons Learned



\- RBAC is preferred over embedding keys.

\- Managed Identity simplifies credential management.

\- Diagnostics enable SOC detection.

\- Private endpoints reduce exposure.





