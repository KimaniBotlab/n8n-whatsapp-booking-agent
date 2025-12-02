# 🤖 AI WhatsApp Booking Agent (n8n + Gemini)

**Built by [Kimani BotLab](https://github.com/kimanibotlab)**

A fully autonomous appointment setting agent that connects WhatsApp to Google Calendar using Large Language Models (LLMs). This workflow replaces manual scheduling by allowing clients to book appointments via natural conversation.


## ⚡ Features
* **Natural Language Processing:** Uses **Google Gemini** to understand intent (e.g., "I need to book next Tuesday afternoon").
* **Real-Time Availability:** Checks **Google Calendar** for conflicts before offering time slots.
* **Smart Timezone Handling:** Converts user's local time (e.g., London) to office time (Nairobi) automatically.
* **Context Awareness:** Remembers conversation history using a memory buffer.
* **Strict Logic:** Enforces a specific data collection flow (Email -> Name -> Phone -> Location).
* **Omnichannel Sync:** Logs all data to **Google Sheets** and sends confirmation emails via **Gmail**.

## 🛠️ Tech Stack
* **Orchestrator:** [n8n](https://n8n.io/)
* **AI Model:** Google Gemini (PaLM)
* **Database:** Google Sheets
* **Scheduling:** Google Calendar
* **Messaging:** WhatsApp (via Twilio)

## 🚀 How to Use
1.  **Import:** Download the `workflow.json` file from this repo.
2.  **Load into n8n:** Open your n8n dashboard > `Import from File`.
3.  **Setup Credentials:** You will need to connect:
    * Google Cloud Console (Calendar, Sheets, Gmail API)
    * Twilio (WhatsApp Sandbox or Business API)
    * Google Gemini API Key
4.  **Activate:** Turn on the workflow and start chatting.

