# Workflow Documentation

## Trigger

Google Drive Trigger monitors a specific folder for new PDF uploads.

---

## Processing

1. Download PDF
2. Extract text
3. Analyze using AI
4. Generate metadata
5. Format output

---

## Storage

Metadata is stored in a Notion database.

Properties:

- Title
- Summary
- Category
- Tags
- Keywords

---

## Notification

Telegram confirms successful synchronization.

---

## Error Handling

- Invalid PDFs
- Empty documents
- AI failures
- Notion API errors
