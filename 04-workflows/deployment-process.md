# Deployment Process

## MuleSoft
1. Merge to `main`
2. Deploy flow to Anypoint (CloudHub) — sandbox first
3. Verify `/api/folders` returns expected JSON
4. Promote to production

## Portal
1. Merge to `main`
2. Build and deploy to hosting
3. Smoke test: folder listing + chat

## Rollback
Redeploy previous known-good version. See [Troubleshooting](../05-docs/runbooks/troubleshooting.md).
