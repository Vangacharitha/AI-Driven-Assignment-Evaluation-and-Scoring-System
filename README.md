n8n – AI-Driven Assignment Evaluation & Scoring System

An automated end-to-end workflow built using n8n to evaluate student assignment PDFs submitted inside a ZIP file. The system extracts text, identifies question–answer pairs, performs AI-based scoring, and delivers a detailed evaluation back to the user—fully automated through Telegram.

<img width="1919" height="927" alt="Assignment evaluation" src="https://github.com/user-attachments/assets/14aa5494-96d4-4334-a45c-7fcad5d828ab" />






🚀 Overview

This workflow allows educators, evaluators, and training institutes to automatically grade assignments submitted in bulk. Students upload a ZIP file via Telegram, and the workflow handles everything from extraction to scoring.

The system uses Google Gemini / OpenAI models for evaluation and is fully modular so you can customize scoring logic, feedback style, or output format.

✨ Key Features

📦 Accepts ZIP files containing any number of PDFs

🔍 Auto-extracts each PDF and converts it to readable text

🧠 AI-based evaluation using Gemini Chat or OpenAI

🧪 Detects Question–Answer pairs using prompt-based extraction

📊 Scores each answer (0–10 scale) + calculates total score

💬 Delivers results on Telegram in a clean, readable format

🔁 Loop processing for unlimited files

⚡ Fully automated workflow, no manual intervention needed

🛠 Easy to extend (export to Google Sheets, send email, store DB, etc.)

🛠 Technologies Used

n8n (No-code automation framework)

Telegram Bot API (User interaction)

Google Gemini Chat Model / OpenAI GPT (AI scoring & feedback)

ZIP & PDF modules for extraction and text processing

JavaScript Function nodes for custom parsing

📥 Setup Instructions

Follow these steps to run the workflow:

1️⃣ Import Workflow

Download the provided .json workflow file

Open n8n

Go to Import → Upload the JSON

2️⃣ Configure Credentials

Telegram Bot Token

Create a bot via @BotFather

Add your token under Telegram API credentials

Gemini/OpenAI API Keys

Add under HTTP Request / OpenAI / Google AI credentials

3️⃣ Enable the Telegram Trigger

After enabling, your bot will start receiving user messages (ZIP uploads).

4️⃣ Test the System

Send a ZIP file containing one or more PDF assignments to your bot.
You will receive:
✔ Extracted Q&A
✔ Score per question
✔ Total score
✔ Final feedback
