# n8n – AI-Driven Assignment Evaluation & Scoring System

An automated end-to-end workflow built using **n8n** to evaluate student assignment PDFs submitted inside a ZIP file.  
The system extracts text, identifies question–answer pairs, performs AI-based scoring, and delivers a detailed evaluation back to the user—fully automated through Telegram.

<img width="1913" height="928" alt="AI Translator" src="https://github.com/user-attachments/assets/f1c34473-859d-442e-9b31-16e2756788b9" />


---

## 📘 Assignment Evaluation

---

## 🚀 Overview

This workflow allows educators, evaluators, and training institutes to automatically grade assignments submitted in bulk. Students upload a ZIP file via Telegram, and the workflow handles everything from extraction to scoring.

The system uses **Google Gemini / OpenAI models** for evaluation and is fully modular so you can customize scoring logic, feedback style, or output format.

---

## ✨ Key Features

- 📦 **Accepts ZIP files** containing any number of PDFs  
- 🔍 **Auto-extracts PDFs** and converts them to readable text  
- 🧠 **AI-based evaluation** using Gemini Chat or OpenAI  
- 🧪 **Detects Q&A pairs** using prompt-based extraction  
- 📊 **Scores each answer (0–10)** + calculates total score  
- 💬 **Sends evaluation on Telegram** in a clean format  
- 🔁 **Loop processing** for unlimited files  
- ⚡ **Fully automated**, no manual work needed  
- 🛠 **Easy to extend** (Google Sheets, email, DB, etc.)

---

## 🛠 Technologies Used

- **n8n (No-code automation framework)**  
- **Telegram Bot API**  
- **Google Gemini / OpenAI GPT**  
- **ZIP & PDF processing modules**  
- **JavaScript Function nodes** for data parsing  

---

## 📥 Setup Instructions

Follow these steps to run the workflow:

---

### 1️⃣ Import Workflow

1. Download the provided `.json` workflow file  
2. Open **n8n**  
3. Go to **Import → Upload JSON**

---

### 2️⃣ Configure Credentials

#### **Telegram Bot Token**
- Create a bot using **@BotFather**  
- Add the token under **Telegram API credentials**

#### **Gemini / OpenAI API Keys**
Add your key under:
- **HTTP Request credentials**, or
- **OpenAI / Google AI node credentials**

---

### 3️⃣ Enable the Telegram Trigger

After activation, your bot will begin receiving ZIP uploads from users.

---

### 4️⃣ Test the System

Send a ZIP file containing PDFs and receive the full evaluation automatically.
