# Portal API (MuleSoft) — Contract

Base URL: `https://<your-anypoint-app>/api`

## Endpoints

### List root folders/files
`GET /folders`

### List folder contents
`GET /folders/{path}/children`

### Get file content (for AI ingestion)
`GET /files/content?path={path}`

## Response Shape
```json
{
  "items": [
    {
      "name": "02-architecture",
      "type": "folder",
      "path": "02-architecture",
      "webUrl": "https://github.com/<org>/<repo>/tree/main/02-architecture"
    },
    {
      "name": "system-overview.md",
      "type": "file",
      "path": "02-architecture/system-overview.md",
      "webUrl": "https://github.com/<org>/<repo>/blob/main/02-architecture/system-overview.md"
    }
  ]
}
