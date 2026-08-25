# 0002 - MuleSoft as the Integration Layer

**Status:** Accepted
**Date:** 2024-01-15

## Context
Storage will change (GitHub now, SharePoint later). We don't want to rewrite
the portal each time. We also don't want secrets in the frontend.

## Decision
Place MuleSoft between the portal and storage. It exposes one clean API and
holds the storage credentials server-side.

## Consequences
- Portal only calls one stable API
- Swapping GitHub → SharePoint = change the Mule connector only
- GitHub PAT stays secured in MuleSoft
- Adds Anypoint dependency and some setup effort
