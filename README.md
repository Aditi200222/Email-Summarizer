📬 Email Summarizing Agent using n8n + Gemini AI
A simple automation built with n8n that summarizes daily Gmail messages using Google Gemini AI and saves the summary to your Gmail as a draft. 
Ideal for daily digests, inbox management, and productivity boosts.

🛠️ Features
•	Fetches emails from Gmail every 24 hours using n8n's schedule trigger
•	Limits the number of messages (e.g., top 10) for summarization
•	Aggregates snippets from multiple emails
•	Uses Google Gemini AI to summarize key details:
    	Key information
    	Issues to look out for
    	Action items
    	Learning outcomes
•	Sends the final summary to your Gmail Drafts

🧩 Tools Used
•	n8n (workflow automation)
•	Gmail API (OAuth2 integration)
•	Google Gemini AI (via API key)
•	Aggregator & AI Agent nodes in n8n

⚙️ Workflow Steps
1.	Schedule Trigger (every 24 hours)
2.	Gmail → Get many messages
3.	Aggregator Node → Combine message snippets
4.	AI Agent Node → Summarize the aggregated content
5.	Gmail → Create Draft with the summary

🔐 Requirements
•	n8n account (self-hosted or cloud)
•	Gmail OAuth2 credentials with scopes:
   o	https://www.googleapis.com/auth/gmail.readonly
•	Gemini AI API key (for LLM summaries)

📤 How to Use
•	Clone or import the workflow into your n8n workspace
•	Connect your Gmail and Gemini credentials
•	Customize filters, token limits, or email subjects as needed
•	Activate the workflow to receive daily AI-generated email summaries

📝 License
MIT License

