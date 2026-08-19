# Autonomous-Multi-Modal-AI-Ecosystem-Messenger-Vision-Enabled
An advanced, production-ready multi-agent automation system built using **n8n**, **OpenAI APIs**, and **Custom JavaScript middleware**, designed to orchestrate complex multi-platform operations via Facebook Messenger.

---

## 🏗️ Architecture Overview
The workflow implements a **Central Orchestrator Agent** pattern that dynamically routes tasks to specialized sub-agents based on the user's intent (Text, Voice, or Image inputs):

1. **Inputs & Multi-Modal Processing:**
   - **Text:** Direct natural language processing.
   - **Voice:** Audio transcription pipeline powered by **OpenAI Whisper API**.
   - **Image:** Visual data interpretation using **OpenAI Vision API**.
2. **Orchestrator Agent:** Manages stateful conversational memory and routes tasks.
3. **Specialized Sub-Agents:**
   - **Web Search Agent:** Retrieves live data (Google Search, Hacker News, Wikipedia).
   - **E-Mail Agent:** Manages Gmail operations (Send, Read, Delete, Reply).
   - **Calendar Agent:** Handles Google Calendar events and conflict-resolution checks.
   - **Social Media Agent:** Automates content publishing (e.g., Twitter/X).
4. **Resilience & Error Mitigation:** Custom JavaScript middleware handling JSON payload sanitization and control character conflict resolution.

---

## 🛠️ Tech Stack
* **Workflow Engine:** n8n
* **AI & LLMs:** OpenAI (GPT-4o, GPT-4o-mini, Whisper, Vision)
* **Vector Database:** Pinecone
* **APIs & Integrations:** Facebook Messenger API, Google Workspace (Gmail, Calendar, Sheets), Telegram Bot API
* **Middleware:** Custom JavaScript

---

## 🚀 How to Import & Run
1. Clone this repository or download the `messenger_multi_agent_workflow.json` file.
2. Open your local or self-hosted **n8n** instance.
3. Create a new workflow, click on the options (three dots) in the top right, and select **Import from File**.
4. Configure your respective credentials (OpenAI API Key, Facebook Messenger Webhook, Google Workspace OAuth, Pinecone).
5. Activate the workflow and test via your Messenger webhook!
