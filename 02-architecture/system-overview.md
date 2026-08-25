# System Overview

## High-Level Architecture
## Components
| Layer | Responsibility |
|-------|----------------|
| Portal UI | Browse folders, view docs, chat |
| MuleSoft | Clean API; holds GitHub token; formats responses |
| GitHub | Stores docs (later: SharePoint) |
| AI (RAG) | Semantic search + Q&A with citations |

## Key Principle
The portal only talks to MuleSoft. Swapping GitHub → SharePoint changes only
the MuleSoft connector — nothing else. See [Decision 0002](../03-decisions/0002-mulesoft-as-integration-layer.md).

See also: [Integrations](./integrations.md), [Data Flow](./data-flow.md)
