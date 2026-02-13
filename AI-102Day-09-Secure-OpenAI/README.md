

AI-102 Day 9 — Secure OpenAI Deployment



Objective

Deploy Azure OpenAI with private networking, monitoring, and cost governance controls.



Architecture





Security Controls Implemented



* Resource Group tagging + budget alerts
* Network restricted (Selected networks / Private Endpoint)
* Private DNS zone integrated
* Diagnostic settings enabled to Log Analytics



Evidence Captured



* AI102-Day09-01-RG-Created.png
* AI102-Day09-02-RG-Tags.png
* AI102-Day09-03-Budget.png
* AI102-Day09-04-OpenAI-Overview.png
* AI102-Day09-05-OpenAI-Networking.png
* AI102-Day09-06-PrivateEndpoint-Created.png
* AI102-Day09-07-PrivateEndpoint-Approved.png
* AI102-Day09-08-PrivateDNS-Zone.png
* AI102-Day09-09-LogAnalytics-Created.png
* AI102-Day09-10-Diagnostics-Enabled.png





KQL / Monitoring Notes



* If Activity logs are empty, enable Subscription Activity Log → Diagnostic settings → send to Log Analytics (Monitor → Activity Log → Diagnostic settings).



Lessons Learned



* Private Endpoint + Private DNS prevents public exposure.
* Diagnostics + Log Analytics provides an audit trail and investigation capability.
* Budgets reduce risk of unexpected spend.



Next



* All resources deleted after validation to prevent additional cost.











