<div align="center">

# 🍽️ Restaurant AI Assistant

### 🤖 My First AI Automation Project using n8n

An intelligent restaurant assistant powered by **n8n**, **Groq LLM**, and **Google Sheets** that can answer customer queries, check menu availability, and manage restaurant orders using AI Agents.

![n8n](https://img.shields.io/badge/n8n-AI%20Automation-FF6D5A?style=for-the-badge&logo=n8n&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-LLM-orange?style=for-the-badge)
![Google Sheets](https://img.shields.io/badge/Google%20Sheets-Database-34A853?style=for-the-badge&logo=googlesheets)
![AI Agent](https://img.shields.io/badge/AI-Agent-blue?style=for-the-badge)

---

### 🚀 Built as my first hands-on n8n automation project

</div>

---

# 📖 Overview

Restaurant AI Assistant is an **AI-powered chatbot** that interacts with customers and performs restaurant-related tasks using an AI Agent.

Instead of relying on hardcoded responses, the AI Agent intelligently selects the appropriate tool based on the user's request.

It can:

- 🍽️ Check menu availability
- ❓ Answer restaurant FAQs
- 📝 Record customer orders
- 🧠 Remember conversation context
- 📊 Read and update Google Sheets

---

# 🏗️ Workflow Architecture

<p align="center">
<img src="C:\Users\kulje\OneDrive\Pictures\Samsung Gallery\Screenshots\Screenshot 2026-07-25 204537.png" width="900">
</p>

---

# 💬 AI Agent Demo

<p align="center">
<img src="Screenshots/chatbot-demo.png" width="900">
</p>

---

# ✨ Features

### 🤖 AI Agent

- Natural language conversation
- Tool selection using reasoning
- Context-aware responses
- Multi-turn conversations

---

### 📋 Menu Lookup

Reads the **Inventory** sheet and returns:

- Food availability
- Current quantity
- Stock status

Example:

```
User:
Do you have Chicken Thali?

Assistant:
Yes!
Chicken Thali is available.

Current Stock: 15
```

---

### ❓ FAQ Assistant

Retrieves restaurant information directly from Google Sheets.

Supports questions like:

- Opening hours
- Delivery
- Refund policy
- Vegetarian options
- Payment methods

---

### 📝 Order Management

Stores customer orders inside Google Sheets.

Information stored:

- Customer Name
- Food Item
- Quantity
- Order Date
- Status

---

### 🧠 Memory

Uses **Simple Memory** to remember previous messages, enabling more natural conversations.

---

# ⚙️ Tech Stack

| Component | Technology |
|-----------|------------|
| Workflow Automation | n8n |
| AI Model | Groq Chat Model |
| LLM | GPT-OSS-20B |
| Memory | Simple Memory |
| Database | Google Sheets |
| Knowledge Base | Google Sheets |

---

# 📂 Google Sheets Database

## 📦 Inventory

Stores:

- Food Item
- Quantity
- Availability

---

## 📑 Orders

Stores:

- Customer Name
- Food Item
- Quantity Ordered
- Date
- Status

---

## ❓ FAQ

Stores restaurant questions and answers.

---

# 🔄 Workflow Logic

```text
Customer
      │
      ▼
Chat Trigger
      │
      ▼
AI Agent
      │
 ┌────┼──────────────┐
 │    │              │
 ▼    ▼              ▼
Menu FAQ          Order
(Read) (Read)    (Update)
      │
      ▼
Google Sheets
      │
      ▼
Response to User
```

---

# 🚀 Getting Started

## 1. Clone the repository

```bash
git clone https://github.com/Harjotsingh0311/restaurant-ai-agent-n8n.git
```

---

## 2. Import the workflow

Open **n8n**

```
Import Workflow
```

Select

```
workflow.json
```

---

## 3. Configure Credentials

Add your:

- Groq API Key
- Google Sheets OAuth

---

## 4. Connect Google Sheets

Use three sheets:

- Inventory
- Orders
- FAQ

---

## 5. Start Chatting 🎉

Ask things like:

```
Show me today's menu

Do you have Veg Thali?

What are your timings?

Place an order for 2 Veg Thalis.
```

---

# 📁 Repository Structure

```
restaurant-ai-agent-n8n
│
├── workflow.json
├── README.md
├── .gitignore
│
└── Screenshots
    ├── workflow.png
    ├── chatbot-demo.png
    ├── inventory.png
    └── faq.png
```

---

# 🎯 Learning Outcomes

Through this project I learned:

- Building AI Agents using n8n
- Connecting LLMs with external tools
- Tool Calling
- Conversational Memory
- Google Sheets Automation
- Low-code AI workflows
- Workflow orchestration

---

# 🔮 Future Improvements

- 📱 WhatsApp Integration
- 💳 Payment Gateway
- 📧 Email Confirmation
- 📦 Live Inventory Updates
- 🚚 Delivery Tracking
- 🎙️ Voice Ordering
- 📊 Analytics Dashboard
- 🌍 Multi-language Support

---

<div align="center">

## ⭐ If you like this project, consider giving it a star!

Made with ❤️ using **n8n + Groq AI + Google Sheets**

</div>
