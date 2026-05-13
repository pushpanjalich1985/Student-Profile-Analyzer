# 🎓 Student Profile Analyzer (n8n Workflow)

A automated networking assistant for the **HulChul** platform. This workflow captures student profile data via a form, uses AI to analyze their background, and stores structured networking suggestions in a Notion database.

## 🛠️ Features
- **Smart Forms**: Integrated n8n form trigger for user input.
- **AI Analysis**: Powered by **Google Gemini 2.5 Flash** via LangChain.
- **Auto-Summarization**: Generates 2-sentence summaries, strengths, and custom icebreakers.
- **Notion Integration**: Automatically logs all processed profiles into a structured database.

## 🚀 Setup Guide
1. **Import**: Copy the JSON code from `workflow.json` and paste it into a new n8n workflow.
2. **Credentials**:
   - Create a **Google Gemini API Key** and add it to the Gemini node.
   - Create a **Notion Internal Integration** and add the token to the Notion node.
3. **Database**: 
   - Create a Notion database with these properties: `Summary`, `Strengths`, `Ideal connections`, `IceBreaker`, and `Tags` (all as Text/Rich Text).
   - In n8n, re-select your database in the Notion node.

## 📝 Technical Note
This JSON file has been sanitized. All unique instance IDs and private webhook identifiers have been removed for security.
