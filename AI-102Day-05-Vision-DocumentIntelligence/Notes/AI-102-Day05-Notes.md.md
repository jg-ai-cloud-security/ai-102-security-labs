Day 5 — Vision + Document Intelligence (Operationalised)



Goal: Deploy OCR / document extraction workloads with production controls (private networking, monitoring, cost, secrets).



Resources (rg-ai102-day5)



cv-ai102-day5 (Azure AI services multi-service, UK South, Standard)



law-ai102-day5 (Log Analytics Workspace)



vnet-ai102-day5 + snet-pe



pe-cv-ai102-day5 (Private Endpoint)



kv-ai102-day5-\* (Key Vault)



Monitoring



Diagnostic setting diag-ai102-day5-cv → Log Analytics law-ai102-day5



Verified logs using KQL (AzureDiagnostics/search)



Networking



Private Endpoint created + Private DNS integration



Public network access set to Disabled



Cost



Budget created at RG scope (budget-ai102-day5) with alerts



Security



Key Vault created (RBAC model)



Secret stored for AI key (cv-ai102-day5-key1)



RBAC assigned (Secrets Officer / Secrets User as needed)



Evidence



Screenshots stored in 06-Screenshots/



DevOps User Story + tasks updated

