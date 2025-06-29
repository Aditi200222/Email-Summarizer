📬 Email Summarizing Agent using n8n & Gemini AI


This project automates the process of reading, summarizing, and drafting Gmail messages using n8n and Google’s Gemini AI. With a simple no-code workflow, it retrieves emails on a daily schedule, summarizes them using an AI agent, and sends the results to your Gmail Drafts folder.

Ideal for busy professionals, founders, researchers, and productivity enthusiasts who want a quick overview of their inbox without reading each message individually.

✨ Features
🔁 Scheduled automation (daily summary at midnight)
📥 Fetches the latest emails from your Gmail inbox.
🧠 AI-powered summarization using Google Gemini
📦 Aggregates multiple emails into one intelligent summary
✉️ Automatically creates a Gmail draft with the summarized output
⚙️ Completely no-code solution using n8n visual workflows

🧰 Tech Stack
•	n8n (Workflow automation)
•	Gmail API (via OAuth2)
•	Google Gemini AI (LLM with API key)
•	Optional: OpenAI or other LLMs can be substituted

🛠 Workflow Overview
Here’s how the automation works:

⏰ Schedule Trigger
 Runs the workflow every 24 hours (midnight by default)
📩 Gmail Node
 Fetches up to 10 recent emails received in the last 24 hours using OAuth2 credentials
🔗 Aggregator Node
 Combines email snippets into one structured input
🤖 AI Agent Node
 Uses Gemini to analyze:
 - Key details
 - Problems/issues raised
 - Action items
 - Learnings or next steps
📝 Gmail Draft Node
 Creates a draft email in your Gmail with the summarized output

🔐 Prerequisites
✅ An n8n cloud or self-hosted instance

✅ Gmail OAuth2 Credentials with the following scopes:
https://www.googleapis.com/auth/gmail.readonly
(or modify/send scope if needed)

✅ Google Gemini API key (or alternative LLM provider)

•	🚀 Getting Started
•	Import the workflow into your n8n account
•	Connect your Gmail credentials using OAuth2
•	Add your Gemini AI credentials (API key)
•	Test the workflow manually to preview results
•	Activate the workflow to run automatically every day

🧪 Example Use Cases
•	Daily email summary digest in your inbox
•	Automatic briefing for newsletters or clients
•	Organizing leads and inquiries for a sales team
•	Summarizing customer feedback or support tickets

📝 License
MIT License – feel free to fork and build on top of this project!
