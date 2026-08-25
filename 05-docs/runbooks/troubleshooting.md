# Troubleshooting

| Symptom | Likely Cause | Fix |
|---------|-------------|-----|
| Portal shows no folders | MuleSoft API down / wrong URL | Check Anypoint app status, `MULESOFT_API_URL` |
| 401 from MuleSoft | Portal API key invalid | Rotate/verify API key |
| MuleSoft 401 to GitHub | PAT expired or wrong scope | Regenerate PAT (Contents:Read), update secure props |
| Broken doc links | `webUrl` mapping wrong | Check DataWeave transform, repo owner/name |
| AI gives wrong answers | Stale index / poor docs | Re-run ingestion; improve source docs |
