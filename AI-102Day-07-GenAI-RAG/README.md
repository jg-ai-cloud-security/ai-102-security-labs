\# AI-102 Day 7 — GenAI RAG (Azure AI Search + Chat + Monitoring)



\## Goal

Build a Retrieval-Augmented Generation (RAG) chat experience that answers questions using enterprise documents indexed in Azure AI Search, returning citations/sources, with monitoring and cost controls enabled.



\## What I built

\- Connected a chat experience (playground/app) to an Azure AI Search index for retrieval.

\- Enabled grounded responses with citations (sources) from retrieved chunks.

\- Enabled diagnostics to Log Analytics and created budget alerts for cost governance.



\## Architecture

\### Diagram 1 — RAG Flow

(Insert PNG in `/diagrams` OR paste a mermaid diagram here)



Example:

\- User question → Azure AI Search retrieves relevant chunks → chunks added to prompt → chat model generates answer + citations.



\### Diagram 2 — Security \& Identity

\- Access controlled via RBAC/Managed Identity (where available).

\- Secrets stored in Key Vault (if keys used).



\### Diagram 3 — Monitoring \& Cost

\- Diagnostics → Log Analytics.

\- Alerts + Budget thresholds.



\## Services used

\- Azure AI Search (index + retrieval)

\- Generative AI chat model (Azure OpenAI / AI Foundry)

\- Embeddings model (for vector retrieval if enabled)

\- Storage account (document source) (if used)

\- Log Analytics Workspace (monitoring)

\- Azure Budgets + Alerts (cost control)

\- Key Vault (optional)



\## Implementation (high level steps)

1\. Prepared / reused Azure AI Search index containing document chunks (and vector fields if enabled).

2\. Deployed chat + embeddings models (recorded deployment names).

3\. Connected chat experience to Azure AI Search as a data source.

4\. Enabled citations and validated responses using test prompts.

5\. Enabled diagnostics for AI + Search to Log Analytics.

6\. Set up a budget and alert thresholds for the resource group.



\## Testing prompts (examples)

\- "Summarise the document and cite sources."

\- "Answer using only the documents. If not found, say you don’t know."

\- "List 3 rules and cite where each is stated."



\## Evidence

Screenshots are stored in `/screenshots`:

\- Model deployments (chat + embeddings)

\- Search index fields (chunk/content field visible)

\- Data connection to Azure AI Search

\- Sample answer showing citations

\- Diagnostics to Log Analytics

\- Budget + alert



\## Notes

See `/notes/day07-daily-summary.md` for:

\- key learnings

\- issues/fixes

\- exam notes



\## Monitoring queries (optional)

If diagnostics were enabled to Log Analytics, see `/kql/day07-monitoring-queries.kql`.



\## Cleanup

\- Deleted: (list what you deleted)

\- Kept: (list what you kept for reuse, e.g., Search/Log Analytics/Storage)



