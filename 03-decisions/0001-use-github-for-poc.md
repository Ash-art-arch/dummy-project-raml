# 0001 - Use GitHub for POC Storage

**Status:** Accepted
**Date:** 2024-01-15

## Context
We need a centralized store for project docs for the POC. SharePoint is the
eventual target but adds auth/setup complexity.

## Decision
Use a private GitHub repo for the POC. Docs are Markdown (AI-friendly),
the Contents API is simple, and auth is a single PAT.

## Consequences
- Fast to start, low cost
- Clean text for the AI layer (no PDF/Word extraction)
- Must swap to SharePoint later — mitigated by the MuleSoft abstraction (see 0002)
