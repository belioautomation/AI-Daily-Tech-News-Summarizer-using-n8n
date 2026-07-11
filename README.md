# 📰 AI Daily Tech News Summarizer using n8n

## 📌 Project Overview

AI Daily Tech News Summarizer is an AI-powered automation workflow built with **n8n**, **Google Gemini AI**, **RSS Feed**, **Google Sheets**, and **Telegram**. It automatically retrieves the latest cybersecurity and technology news, summarizes multiple articles using AI, stores the summaries in Google Sheets, and delivers a daily news digest directly to Telegram.

Built as part of my **30-Day n8n Automation Portfolio**, this project demonstrates AI-powered content summarization, RSS feed processing, workflow automation, and automated reporting.

---

## 🎯 Objectives

* Automate daily technology news collection
* Summarize multiple news articles using AI
* Archive AI-generated summaries
* Deliver daily news digests to Telegram
* Build a portfolio-ready AI automation workflow

---

## 🏗️ Workflow Architecture

```text
Schedule Trigger
        │
        ▼
RSS Feed Read
        │
        ▼
Limit
        │
        ▼
Aggregate
        │
        ▼
Google Gemini (Basic LLM Chain)
        │
        ▼
Google Sheets
        │
        ▼
Telegram
```

---

## ⚙️ Workflow Implementation

### 1. Schedule Trigger

Runs the workflow automatically every day at a scheduled time.

---

### 2. RSS Feed Read

Retrieves the latest cybersecurity and technology news from an RSS feed.

Example source:

```text
https://feeds.feedburner.com/TheHackersNews
```

---

### 3. Limit

Selects the latest news articles (for example, the most recent five) for processing.

---

### 4. Aggregate

Combines article titles and content into a structured format suitable for AI summarization.

---

### 5. Google Gemini (Basic LLM Chain)

Analyzes the collected articles and generates a concise daily news digest by:

* Summarizing each article
* Highlighting key information
* Producing a readable report

---

### 6. Google Sheets

Stores AI-generated summaries for future reference.

Example columns:

| Date | Headlines | Summary |
| ---- | --------- | ------- |

---

### 7. Telegram

Sends the summarized daily news digest directly to Telegram.

Example:

```text
📰 Daily AI & Tech News

1. Oracle Security Flaw Under Active Exploitation

A critical Oracle vulnerability is currently being exploited, allowing attackers to compromise vulnerable systems.

2. Malicious AI Chrome Extension Removed

Microsoft identified and removed a fake AI browser extension that intercepted user searches.

3. WhatsApp Introduces Usernames

WhatsApp is rolling out usernames to improve user privacy without exposing phone numbers.

🤖 Generated automatically with n8n.
```

---

## 🛠️ Technologies Used

* n8n
* Google Gemini AI
* RSS Feed
* Google Sheets API
* Telegram Bot API

---

## 📁 Repository Structure

```text
AI-News-Summarizer/
│
├── README.md
├── workflow.json
│
├── screenshots/
│   ├── workflow.png
│   ├── telegram-output.png
│   └── google-sheets.png
│
└── assets/
```

---

## 📸 Screenshots

Include the following screenshots:

* Complete Workflow
* Google Sheets Output
* Telegram Notification

---

## 🚀 Key Features

* ✅ Scheduled Workflow Automation
* ✅ RSS Feed Processing
* ✅ AI-Powered News Summarization
* ✅ Google Sheets Integration
* ✅ Telegram Notifications
* ✅ Automated Daily News Digest
* ✅ Fully Automated Workflow

---

## 🎓 Lessons Learned

Through this project, I gained experience in:

* Building AI-powered automation workflows
* Integrating RSS feeds with n8n
* Using Google Gemini for text summarization
* Aggregating and processing structured data
* Automating Google Sheets logging
* Delivering AI-generated reports through Telegram

---

## 📈 Impact

This workflow automates the collection and summarization of technology news, helping users stay informed without manually browsing multiple sources. It demonstrates how AI and workflow automation can simplify information gathering and daily reporting.

---

## 📜 License

MIT License

---

## 👨‍💻 Author

**Belio C. Sinangote**

BS Information Technology Student
Cebu Technological University (CTU)

GitHub: [https://github.com/belioautomation](https://github.com/belioautomation)

This project is part of my **30-Day n8n Automation Portfolio**, showcasing practical workflow automation using n8n, AI, APIs, and automation best practices.
