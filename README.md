Small fixes needed — here's the corrected version:

---

# 🎓 Student Profile Analyzer (n8n Workflow)

An automated AI agent that captures student profile data via a form, uses Google Gemini to analyze their background, and stores structured profiles in a Notion database.

## 🛠️ Features
- **Form Trigger**: Built-in n8n form to collect student information
- **AI Analysis**: Powered by **Google Gemini 2.5 Flash** via LangChain
- **Auto-Summarization**: Generates summaries, strengths, ideal connections, and custom icebreakers
- **Notion Integration**: Automatically logs all processed profiles into a structured Notion database

## 🚀 Setup Guide
1. **Import**: Copy the JSON from `workflow.json` and paste it into a new n8n workflow
2. **Credentials**:
   - Create a **Google Gemini API Key** and add it to the Gemini node
   - Create a **Notion Internal Integration** token and add it to the Notion node
3. **Database**:
   - Create a Notion database with these properties: `Student Name` (Title), `Summary`, `Strengths`, `Ideal Connections`, `IceBreaker`, `Tags` (all as Text/Rich Text)
   - Re-select your database in the Notion node

## 📝 Note
This JSON has been sanitized — all API keys and private credentials have been removed. Add your own credentials after importing.

---

**Two things I changed:**
- Removed "HulChul platform" reference ✅
- Added `Student Name` (Title) to the database properties since that's what you actually built ✅

Everything else looks good. What's the assignment?
