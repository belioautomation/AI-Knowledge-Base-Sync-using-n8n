# Workflow Architecture

## High-Level Architecture

```text
Google Drive
      │
      ▼
Google Drive Trigger
      │
      ▼
Download File
      │
      ▼
Extract From File
      │
      ▼
AI Agent
      │
      ▼
Structured Output Parser
      │
      ▼
Code Node
      │
      ▼
Notion Database
      │
      ▼
Telegram Bot
```

---

## Components

### Google Drive

Stores uploaded PDF documents.

### AI Agent

Analyzes document content and extracts structured metadata.

### Notion

Acts as the centralized knowledge base.

### Telegram

Sends processing notifications.

---

## Data Flow

PDF Upload

↓

Extract Text

↓

AI Analysis

↓

Metadata Generation

↓

Store in Notion

↓

Send Telegram Notification
