# automated-job-outreach-ai
AI-powered job search automation: scraping, scoring, lead discovery &amp; cold outreach using n8n + LLM

---
## 📸 Screenshots
<img width="1710" height="447" alt="image" src="https://github.com/user-attachments/assets/bb787b26-4772-4340-a8c4-d2224bf76e89" />
---


#  AI Job Search Automation (n8n)

An end-to-end job search automation workflow built using n8n that:

* Scrapes job-related data (via Apify / Google Search patterns)
* Extracts candidate/company insights
* Finds relevant LinkedIn profiles
* Scores & filters opportunities
* Generates:

  * Cold emails
  * LinkedIn outreach messages

---

## 🧠 Features

* 🔍 Job scraping (API-based or search-based)
* 👤 LinkedIn profile discovery (Google search pattern)
* 🧹 Data cleaning + enrichment
* 📊 Deduplication & filtering
* ✉️ AI-generated cold emails
* 💬 AI-generated LinkedIn messages
* 📄 Google Sheets integration

---

## ⚙️ Tech Stack

* n8n (workflow automation)
* Apify (job scraping – external service)
* Google Custom Search API
* Google Sheets API
* LLM (for message generation)

---

## 🏗️ Workflow Overview

1. Trigger workflow
2. Generate search queries
3. Fetch LinkedIn profiles via Google API
4. Extract structured data (name, title, bio)
5. Remove duplicates
6. Store in Google Sheets
7. Generate outreach messages

---

## 📦 Setup Instructions

### 1. Import Workflow

* Open n8n
* Go to "Import"
* Upload `workflow/job-agent.json`

### 2. Add Credentials

You must configure:

* Google Sheets OAuth
* Google Custom Search API key
* Apify API (if used)

### 3. Environment Variables

Create `.env` file:

```
GOOGLE_API_KEY=your_key_here
GOOGLE_CX=your_search_engine_id
```

---

## ⚠️ Important Note (Legal & ToS)

Automating scraping and outreach on LinkedIn, Naukri, Indeed, or email can violate platform Terms of Service and privacy laws. Use official APIs or approved tools when possible, throttle requests, and ensure compliance.

---

## 🧪 Example Use Case

Search:
"Software Engineer hiring manager site:linkedin.com/in"

→ Extract hiring managers
→ Generate personalized outreach
→ Store leads in Google Sheets

---



## 🚧 Future Improvements

* Add email verification (Hunter/Snov)
* Add CRM integration
* Add scoring ML model
* Add auto-send email system

---

## 👨‍💻 Author

Built by Haswanth
