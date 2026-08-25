# Integrations

| Integration | Purpose | Auth | Status |
|-------------|---------|------|--------|
| MuleSoft ↔ GitHub | Read docs | Fine-grained PAT (Contents:Read) | Active (POC) |
| MuleSoft ↔ SharePoint | Read docs | Azure AD app | Planned |
| Portal ↔ MuleSoft | Serve content | API key | Active |
| AI ↔ Claude API | Answer questions | API key | Planned |

## Notes
- GitHub PAT is stored in MuleSoft secure properties, never in the frontend.
- SharePoint connector will replace the GitHub connector behind the same API contract.
