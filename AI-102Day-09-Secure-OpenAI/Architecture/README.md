\# AI-102 Day 9 — Secure Azure OpenAI Deployment



> Private Endpoint + Private DNS + Monitoring + Cost Governance







\## Architecture





Day 9 Architecture](Architecture/AI102-Day09-Architecture.png)









\## What This Architecture Demonstrates



This design follows Azure Well-Architected Framework principles for security, operational excellence, and cost optimization.





\### Network Isolation



Azure OpenAI is deployed inside a Virtual Network and accessed through a Private Endpoint using Azure Private Link. Public network access is disabled to prevent internet exposure.





\### Private DNS Resolution



The Private DNS Zone (privatelink.openai.azure.com) ensures internal name resolution to the private endpoint IP address instead of the public endpoint.







\### Identity \& Access Control

Managed Identity and RBAC enforce least-privilege access and eliminate hard-coded secrets.



\### Monitoring \& Auditability

Diagnostic logs are routed to Log Analytics, enabling KQL queries and security investigations.



\### Alerting \& Cost Governance

Azure Monitor alerts detect abnormal behavior, while budget alerts protect against unexpected AI workload costs.



