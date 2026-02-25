# 📩 Gmail Intelligent Automation Workflow (n8n)

An advanced, production-grade **Gmail automation system** built using **n8n**, combining  
Gmail API, Google Sheets API, Twilio WhatsApp notifications, Slack alerts, and the Gemini  
Language Model for classification, summarization, and automated responses.

This workflow intelligently categorizes incoming emails, stores structured information,  
summarizes content, validates recruitment mails, and sends real-time notifications to users.

---

## 🚀 Features

### ✅ **1. Email Categorization (AI-Powered)**
Uses Google's Gemini chat model to classify emails into:
- **Social**
- **Tech**
- **Recruitment**
- **Delivery**
- **Personal**
- **Misc**

### ✅ **2. Recruitment Mail Legitimacy Validator**
- Detects if a recruitment email is from a real company or spam.
- Saves valid opportunities to Google Sheets.
- Sends **Slack & WhatsApp** alerts for high-priority mails.

### ✅ **3. Social & Tech Email Summarization**
- Extracts important information from newsletters.
- Creates clean, human-friendly summaries.
- Automatically logs into Google Sheets.

### ✅ **4. Personal Email Auto-Responder**
If the user is busy:
- Reads the email
- Generates an appropriate reply using Gemini
- Sends the response through Gmail API

### ✅ **5. Delivery Update Handler**
Classifies and extracts tracking details (where possible).

### ✅ **6. Real-Time Notifications**
- WhatsApp (Twilio)
- Slack
- Email fallback (optional)

---

## 🧠 Tech Stack

| Component | Used For |
|----------|----------|
| **n8n** | Workflow automation, orchestration |
| **Gmail API** | Fetching emails & sending replies |
| **Google Sheets API** | Storing summaries & categorized data |
| **Twilio WhatsApp API** | High-priority notifications |
| **Slack API** | Alerts for recruitment & personal mails |
| **Gemini (LLM)** | Classification, summarization, auto-reply |
| **Webhook Triggers / Cron Jobs** | Scheduled email processing |

---


## 📸 Screenshots

Add your screenshots here:

### ✅ Workflow Overview  
<img width="1920" height="1080" alt="Screenshot 2025-11-02 125907" src="https://github.com/user-attachments/assets/5ff4a144-cb77-4bc6-9c0a-67f4bf4c08d2" />


### ✅ AI prompt  
<img width="1920" height="1080" alt="Screenshot 2025-11-02 130026" src="https://github.com/user-attachments/assets/38951432-3e03-4c57-97a9-85af216bed77" />


### ✅ Sheets Output Example  

<img width="1437" height="877" alt="email1" src="https://github.com/user-attachments/assets/0fac17bb-c1b1-4916-b3a8-6328e56cecf1" />



---

## 🎥 Demo Video (Optional)
the workflow in action:




---

## 📥 Importing the Workflow

1. Download the workflow file:  
   **[`workflow.json`](https://github.com/Nothing00980/Gmail-Automation-n8n/blob/main/email-automation%20(2).json)**

2. Open your n8n instance  
3. Go to **Import → From File**  
4. Upload the JSON  
5. Add your own credentials:
   - Gmail OAuth2
   - Google Sheets OAuth2
   - Twilio Auth
   - Slack Bot Token
   - Gemini API Key

6. Activate the workflow ✅

---


*(Ensure you **never** commit these to GitHub.)*

---

## 📑 How It Works (Short Breakdown)

### 1️⃣ Fetch Emails  
Gmail → n8n → Gemini categorization

### 2️⃣ AI Classification  
Gemini decides category + extracts metadata

### 3️⃣ Action Based on Category  
| Category | Action |
|----------|--------|
| **Social** | Summarize + Save to Sheets |
| **Tech** | Summarize + Save to Sheets |
| **Recruitment** | Validate + Save + Notify |
| **Personal** | Auto-respond using Gemini |
| **Delivery** | Extract tracking info |
| **Misc** | Logged for later |

### 4️⃣ Notifications  
Slack + WhatsApp for priority events.

---

## 🛡️ Security Notes

- All API keys removed from workflow.json  
- Replace placeholders with your own environment variables  
- No real data is included  
- Demo-only structure provided for recruiters and developers  

---

## 👨‍💻 Author

**Yuvraj Bhati**  
AI/ML • Automation • Software Development  
GitHub | LinkedIn | Portfolio (optional)

---

## ⭐ Support  
If you like this project, star the repo! It helps visibility 😊





