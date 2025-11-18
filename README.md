Gen Therapist – AI CBT Chatbot

A mental-health support chatbot built using Gemini AI, n8n workflows, Telegram Bot API, Google Sheets, and SerpAPI to provide safe, evidence-based Cognitive Behavioral Therapy (CBT)–inspired guidance.

🌟 Project Overview

Gen Therapist is an AI-powered chatbot designed to offer preliminary CBT-based emotional support.
It helps users with:

Stress management

Negative thought reframing

Daily journaling

Mood tracking

Guided CBT-style conversations

This project demonstrates how AI + Automation + Chat Interfaces can make mental-health support more accessible.

⚙️ Tech Stack
Component	Technology Used
Workflow Automation	n8n
AI Model	Google Gemini API
User Interface	Telegram Bot
Data Storage	Google Sheets API
External Search	SerpAPI
Memory Handling	Simple Memory Node (n8n)
Trigger	Telegram Trigger / Webhook
🧠 Key Features

CBT-based emotional support

Real-time Telegram conversation

Mood tracking and journaling

Empathetic and safe AI responses

External fact searches via SerpAPI

Workflow automation for message processing

Short-term memory for conversational continuity

🏗️ System Architecture
Telegram → n8n Webhook → Gemini AI → Memory / Sheets → Telegram Response

Workflow Steps:

User sends message to Telegram bot

n8n Webhook receives the message

Workflow triggers Gemini AI to generate CBT-based replies

SerpAPI used when user asks for definitions/explanations

Mood/journal data saved into Google Sheets

Processed response sent back to the user

📁 Project Structure
/GenTherapist
│
├── workflows/
│   ├── main-workflow.json
│   └── crisis-handler.json
│
├── assets/
│   ├── screenshots/
│   └── diagrams/
│
├── docs/
│   ├── report.pdf
│   ├── presentation.pptx
│   └── references.txt
│
├── README.md
└── .env.example

🚀 How to Set Up the Project
1. Install n8n
npm install n8n -g
n8n start

2. Create a Telegram Bot

Open @BotFather on Telegram

Run /newbot

Save your BOT_TOKEN

3. Set Up APIs

Create an .env file and add:

TELEGRAM_BOT_TOKEN=xxxx
GEMINI_API_KEY=xxxx
SERPAPI_KEY=xxxx
GOOGLE_SHEETS_ID=xxxx

4. Import n8n Workflow

Open n8n

Import the workflow JSON file

Add your API keys into nodes

5. Connect Webhook

Copy n8n Webhook URL

Paste into Telegram using:

https://api.telegram.org/bot<token>/setWebhook?url=<your_n8n_webhook_url>

6. Start Chatting

Your bot is now live and ready to interact.

🧪 Testing

The system was tested for:

Functional accuracy

Integration between modules

Response safety

Latency and performance

User experience

Gemini AI generated empathetic, safe, and structured CBT outputs in all major test scenarios.

📊 Results

Reliable real-time responses
Accurate CBT-style guidance
Smooth integration via n8n
Successful data logging in Sheets
High user satisfaction in testing

🛠️ Future Scope

Multilingual support
Voice-based conversations
Mobile app version
Long-term personalized memory
Advanced emotional detection
Wearable device integration
Crisis-response automation
Therapist dashboard



👩‍💻 Developed By

Prachi Aggarwal
B.Tech (Artificial Intelligence)
Session: 2022-2026
