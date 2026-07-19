# 📚 AI Knowledge Base Sync using n8n

Automatically organize, summarize, and sync PDF documents into a searchable Notion knowledge base using AI.

---

# 📖 Overview

Managing documents manually can quickly become time-consuming as files accumulate across cloud storage. Searching through folders, creating summaries, and organizing information often requires repetitive work.

This workflow automates the entire process by monitoring a Google Drive folder for newly uploaded PDF documents. Once detected, AI analyzes the document, extracts key information, generates metadata, and stores everything inside a structured Notion database. A Telegram notification is then sent to confirm successful processing.

This project demonstrates how AI can automate document management and build a centralized knowledge base with minimal human intervention.

---

# ✨ Features

- 📂 Automatic Google Drive monitoring
- 📄 PDF document processing
- 📝 Text extraction from uploaded files
- 🤖 AI-powered document analysis
- 📋 Automatic title generation
- 📑 AI-generated summaries
- 🏷️ Category classification
- 🔖 Automatic tag generation
- 🔑 Keyword extraction
- 📚 Notion Knowledge Base integration
- 📲 Telegram notifications
- ⚡ Fully automated workflow

---

# 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| Automation | n8n |
| AI Model | OpenRouter AI |
| Storage | Google Drive |
| Knowledge Base | Notion |
| Notifications | Telegram |
| Programming | JavaScript |

---

# 🧩 Workflow

```text
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
Code (Format Output)
        │
        ▼
Notion Database
        │
        ▼
Telegram Notification
```

---

# ⚙️ Workflow Steps

### 1. Google Drive Trigger

Monitors a Google Drive folder for newly uploaded PDF documents.

---

### 2. Download File

Downloads the uploaded PDF from Google Drive.

---

### 3. Extract From File

Extracts readable text from the PDF document.

---

### 4. AI Agent

Analyzes the extracted content and generates:

- Title
- Summary
- Category
- Tags
- Keywords

---

### 5. Structured Output Parser

Formats the AI response into structured JSON for downstream processing.

---

### 6. Code Node

Prepares and formats the extracted metadata before sending it to Notion.

---

### 7. Notion

Creates a new page inside the AI Knowledge Base database with the generated metadata.

---

### 8. Telegram

Sends a notification confirming that the document has been successfully processed.

---

# 📊 AI Output Example

```json
{
  "title": "Meeting Notes",
  "summary": "Discussion of the AI Knowledge Base Sync project covering workflow updates, AI integration, issues, blockers, and action items.",
  "category": "Meeting",
  "tags": [
    "n8n",
    "Workflow",
    "Project Updates"
  ],
  "keywords": [
    "AI Knowledge Base",
    "Meeting",
    "Automation"
  ]
}
```

---

# 📚 Notion Database Structure

| Property | Type |
|----------|------|
| Title | Title |
| Summary | Text |
| Category | Select |
| Tags | Multi-select |
| Keywords | Multi-select |

---

# 📂 Repository Structure

```
AI-Knowledge-Base-Sync-using-n8n/
│
├── workflow/
│   └── workflow.json
│
├── screenshots/
│   ├── workflow.png
│   ├── notion-database.png
│   ├── telegram-notification.png
│   └── execution.png
│
├── sample-data/
│   ├── sample-meeting-notes.pdf
│   └── sample-output.json
│
├── docs/
│   ├── architecture.md
│   ├── workflow-documentation.md
│   ├── ai-prompts.md
│   ├── setup-guide.md
│   └── troubleshooting.md
│
├── LICENSE
└── README.md
```

---

# 🚀 Setup

## Prerequisites

- n8n
- Google Drive Account
- Notion Account
- Telegram Bot
- OpenRouter API Key

---

## Required Credentials

- Google Drive OAuth2
- OpenRouter API
- Notion API
- Telegram Bot API

---

# 💼 Skills Demonstrated

- n8n Workflow Automation
- AI Document Processing
- Prompt Engineering
- PDF Text Extraction
- Structured AI Outputs
- JavaScript
- Google Drive Integration
- Notion Integration
- Telegram Automation
- Knowledge Management
- Business Process Automation

---

# 🎯 Use Cases

- Company Knowledge Bases
- Meeting Notes Management
- Internal Documentation
- SOP Repository
- Project Documentation
- Research Paper Organization
- Training Materials
- Technical Documentation
- Personal Knowledge Management

---

# 🔮 Future Improvements

- Duplicate document detection
- OCR support for scanned PDFs
- Semantic document search
- Vector database integration
- RAG (Retrieval-Augmented Generation)
- Multi-language document support
- Automatic document versioning
- AI-powered question answering
- Document approval workflow

---

# 📸 Screenshots

> Add screenshots of:
>
> - Complete Workflow
> - Google Drive Folder
> - AI Agent Configuration
> - Notion Database
> - Telegram Notification
> - Workflow Execution

---

# 👨‍💻 Author

**Belio C. Sinangote**

Building AI-powered workflow automations with **n8n**, APIs, and AI models as part of a **30-Day n8n Automation Challenge**.

