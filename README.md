# 🚀 AI CRM Lead Qualification Workflow using n8n

An AI-powered CRM Lead Qualification workflow built with **n8n**, **Groq Llama 3.3**, **Google Sheets**, **Gmail**, and **Slack**.

This workflow automatically validates incoming business leads, analyzes their quality using AI, assigns a lead score and status, updates the CRM, and notifies the sales team for timely follow-up.

---

## ✨ Features

* 🌐 Webhook-based Lead Intake API
* 🤖 AI-powered Lead Qualification
* 📊 AI Lead Scoring (1–10)
* 🔥 Automatic Lead Status Classification

  * Hot
  * Qualified
  * Warm
  * Nurture
  * Cold
* ⚡ Priority Assignment

  * Critical
  * High
  * Medium
  * Low
  * Ignore
* ⏰ AI Follow-up Recommendation
* 📧 Gmail Notifications
* 📄 Google Sheets CRM Integration
* 🔁 Append or Update Existing Leads
* 🚨 Slack Error Notifications
* ✅ Input Validation
* 📦 Structured JSON API Response

---

# 🛠 Tech Stack

* n8n
* Groq API
* Llama 3.3 70B
* Google Sheets API
* Gmail API
* Slack API
* Webhooks

---

# 📌 Workflow Architecture

```
Webhook
    │
    ▼
Validate Request
    │
    ▼
AI Lead Qualification
    │
    ▼
Lead Score
    │
    ▼
Lead Status
    │
    ▼
Priority Assignment
    │
    ▼
Email Notification
    │
    ▼
Google Sheets CRM
    │
    ▼
Webhook Response
```

---

# 📥 API Endpoint

```
POST /webhook/crm
```

---

# 📤 Sample Request

```json
{
  "name":"John Smith",
  "company":"ABC Technologies",
  "email":"john@abc.com",
  "budget":"15000 USD",
  "requirement":"Need AI automation for sales process."
}
```

---

# 📥 Sample Response

```json
{
  "success": true,
  "lead": {
    "name": "John Smith",
    "company": "ABC Technologies",
    "email": "john@abc.com"
  },
  "ai": {
    "score": 9,
    "status": "Hot",
    "priority": "Critical",
    "reason": "Clear enterprise automation opportunity.",
    "follow_up": "Within 15 Minutes"
  }
}
```

---

# 📊 AI Output

The AI evaluates every lead using:

* Budget
* Company Quality
* Requirement Clarity
* Project Complexity
* Business Value
* Closing Probability
* Decision Maker Intent
* AI / Automation Opportunity

---

# 🔥 Lead Status

| Score | Status      |
| ----- | ----------- |
| 9–10  | 🔥 Hot      |
| 7–8   | ✅ Qualified |
| 5–6   | 🟡 Warm     |
| 3–4   | 🔵 Nurture  |
| 1–2   | ⚫ Cold      |

---

# 📂 Project Structure

```
04.n8n-ai-crm-lead-qualification
│
├── workflow.json
├── api-request.json
├── README.md
├── LICENSE
├── .gitignore
│
├── assets
│   ├── workflow.png
│   └── architecture.png
│
└── screenshots
    ├── webhook-test.png
    ├── gmail-notification.png
    ├── google-sheet.png
    └── workflow-execution.png
```

---

# 🚀 Getting Started

1. Import `workflow.json` into n8n.
2. Configure the required credentials:

   * Groq
   * Gmail
   * Google Sheets
   * Slack
3. Activate the workflow.
4. Send a POST request to the Webhook endpoint.
5. The workflow will automatically:

   * Validate the request
   * Score the lead
   * Classify the lead
   * Send email notifications
   * Update the CRM
   * Return a JSON response

---

# 📸 Screenshots

* Workflow
* API Testing
* Gmail Notification
* Google Sheets CRM
* Workflow Execution

(Add screenshots inside the `screenshots` folder.)

---

# 💡 Use Cases

* AI Agencies
* CRM Automation
* Sales Teams
* Lead Qualification
* AI Automation Businesses
* Marketing Agencies
* SaaS Companies

---

# 📄 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Piyush Kumar**

AI Automation Developer

* GitHub: https://github.com/autonode-x
* LinkedIn: https://www.linkedin.com/in/piyush-ai

---

⭐ If you found this project useful, consider giving it a star.
