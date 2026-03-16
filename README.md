# 🤖 n8n + Gemini AI Automation

This repository contains an automated workflow built in [n8n](https://n8n.io/) that integrates with the **Google Gemini API** to process data and generate AI-driven insights.

## 🚀 Overview
This project uses n8n to connect various data sources (like Google Sheets, Webhooks, or HTTP requests) to the Gemini 1.5 Flash model. It is designed to automate repetitive thinking tasks, such as content summarization, data categorization, or automated responses.

## 📦 Features
* **AI Engine:** Powered by Google Gemini (1.5 Flash/Pro).
* **Error Handling:** Includes retry logic for API rate limits (`429` errors).
* **Version Control:** Workflow logic is stored as JSON for easy deployment.

## 🛠️ Setup Instructions

### 1. Import the Workflow
1.  Copy the content of the `workflow.json` file in this repo.
2.  Open your n8n instance.
3.  Press `Ctrl + V` on the canvas to import the nodes.

### 2. Configure Credentials
To get this working, you need to set up your Google Gemini API key:
1.  Go to [Google AI Studio](https://aistudio.google.com/).
2.  Create a **new API Key** in a new project.
3.  In n8n, create a new "Google Gemini" credential and paste your key.

### 3. Environment Variables
If you are running this via Docker, ensure your `.env` file allows for external API calls.

## 📂 File Structure
* `workflow.json`: The raw n8n workflow export.
* `README.md`: This documentation.

## ⚠️ Security Note
**Never commit your actual API keys or credentials to GitHub.** This repository only contains the workflow logic. Ensure your n8n credentials remain private.

---
*Created with ❤️ using n8n and Gemini.*
