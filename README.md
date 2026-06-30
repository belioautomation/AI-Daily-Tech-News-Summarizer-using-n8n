# AI Daily Tech News Summarizer using n8n

An AI-powered automation workflow built with **n8n** that fetches the latest cybersecurity and technology news from an RSS feed, summarizes it using **Google Gemini**, stores the results in **Google Sheets**, and automatically delivers a daily digest to **Telegram**.

---

## 📌 Overview

This workflow automates the process of staying up to date with technology news by:

* Retrieving the latest articles from an RSS feed.
* Selecting the newest articles.
* Organizing the data into a format suitable for AI.
* Generating concise summaries using Google Gemini.
* Saving summaries for future reference in Google Sheets.
* Sending the summarized news directly to Telegram.

Perfect for developers, cybersecurity enthusiasts, students, and anyone who wants an AI-curated daily news digest.

---

## 🚀 Features

* ⏰ Automatic scheduled execution
* 📰 Retrieves latest tech & cybersecurity news
* 🤖 AI-powered summarization with Google Gemini
* 📊 Stores summaries in Google Sheets
* 📲 Sends formatted news digest to Telegram
* 💯 Fully automated workflow
* 🆓 Uses free services (within available free tiers)

---

## 🛠 Tech Stack

* **n8n**
* **Google Gemini**
* **RSS Feed**
* **Google Sheets API**
* **Telegram Bot API**

---

## 📂 Workflow

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

## ⚙️ Workflow Explanation

### 1. Schedule Trigger

Runs automatically every day at a specified time.

---

### 2. RSS Feed Read

Retrieves the latest articles from:

```
https://feeds.feedburner.com/TheHackersNews
```

---

### 3. Limit

Limits the number of articles processed (e.g., latest 5).

---

### 4. Aggregate

Combines article titles and content into a structured format suitable for AI summarization.

---

### 5. Google Gemini (Basic LLM Chain)

Generates a concise news digest by:

* Summarizing each article
* Highlighting key points# AI-Daily-Tech-News-Summarizer-using-n8n
An AI-powered automation workflow built with n8n that fetches the latest cybersecurity and technology news from an RSS feed, summarizes it using Google Gemini, stores the results in Google Sheets, and automatically delivers a daily digest to Telegram.

* Producing a readable daily report

---

### 6. Google Sheets

Archives the generated summaries.

Example columns:

| Date | Headlines | Summary |
| ---- | --------- | ------- |

---

### 7. Telegram

Sends the AI-generated news digest directly to Telegram.

Example output:

```text
📰 Daily AI & Tech News

1. Oracle Security Flaw Under Active Exploitation

A critical Oracle Payments vulnerability (CVE-2026-46817) is currently being exploited. Attackers can gain unauthorized control of vulnerable Oracle instances.

2. Malicious AI Chrome Extension Removed

Microsoft identified a fake Perplexity AI Chrome extension that intercepted user searches before redirecting them to legitimate websites.

3. WhatsApp Introduces Usernames

WhatsApp has started rolling out usernames to improve privacy by allowing users to connect without sharing phone numbers.

Have a productive day!
```

---

## 📁 Project Structure

```
AI-News-Summarizer/
│
├── README.md
├── workflow.json
└── screenshots/
    ├── workflow.png
    ├── telegram-output.png
    └── google-sheets.png
```

---

## 📸 Screenshots

Include screenshots such as:

* Workflow Editor
* Google Sheets output
* Telegram notification

Example:

```
screenshots/
    workflow.png
    telegram-output.png
    google-sheets.png
```

---

## 💡 Use Cases

* Daily cybersecurity updates
* Technology news digest
* AI-powered content summarization
* Learning n8n automation
* Portfolio project for automation and AI

---

## 🔮 Future Improvements

* Support multiple RSS feeds
* Remove duplicate articles
* Categorize news by topic (AI, Security, Cloud, etc.)
* Generate email newsletters
* Save summaries to Notion
* Publish summaries to Discord or Slack
* Translate summaries into multiple languages

---

## 📚 What I Learned

This project helped me gain practical experience with:

* Workflow automation using n8n
* Integrating RSS feeds
* Prompt engineering with Google Gemini
* Google Sheets automation
* Telegram Bot integration
* Data aggregation and transformation
* Building end-to-end AI-powered workflows

---

## 🏷 Skills Demonstrated

* n8n
* Workflow Automation
* Google Gemini AI
* Google Sheets API
* Telegram Bot API
* RSS Feed Processing
* Prompt Engineering
* Data Transformation
* API Integration
* No-Code / Low-Code Automation

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome. Feel free to fork this repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.

---

# ⭐ If you found this project useful, consider giving it a star!
