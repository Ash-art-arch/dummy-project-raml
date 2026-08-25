# Data Flow

## Browsing folders
1. User opens a folder in the portal
2. Portal → `GET /api/folders/{path}/children` (MuleSoft)
3. MuleSoft → GitHub Contents API (with secured PAT)
4. MuleSoft transforms response → clean JSON
5. Portal renders folders/files with hyperlinks

## Asking a question (AI chat)
1. User types a question
2. Question embedded → vector DB search for relevant chunks
3. Chunks + question → Claude
4. Claude answers, citing source docs (links back to GitHub)

![Data Flow](./diagrams/data-flow.png)
