# Placementbot

Automated **agentic workflow** built with **n8n**, **Telegram Bot**, and **LLM integration** to extract structured placement deadlines from emails and send real-time automated reminders. :contentReference[oaicite:1]{index=1}

---

## Overview

Placementbot keeps track of incoming placement notification and reminds you beofre deadline without any human intervention. It:

- Parses structured info from incoming placement emails.
- Detects deadlines and key metadata.  
- Sends Telegram alerts as reminders.   
- Runs as an n8n workflow for repeatable automation.


---

## 🧠 Workflow Architecture

> The core automation is defined in an n8n workflow JSON (`workflow.json`).  
> It listens for incoming triggers, extracts data using LLM logic, and sends Telegram notifications.

### 🖼️ Workflow Preview

> Replace these with actual screenshots from your `screenshots` folder:

![Workflow — Import view](screenshots/workflow.png)  
*Import view of the n8n workflow showing node layout.*

![Workflow — Data extraction](screenshots/workflow-data-nodes.png)  
*Nodes that handle parsing and structured extraction.*

---

## 💬 Sample Incoming Message

Show how a valid placement email looks before processing:

![Incoming message example](screenshots/incoming-message.png)  
*Example of a raw placement email that the workflow ingests.*

---

## 🛠️ Built With

| Technology | Purpose |
|------------|---------|
| **n8n** | Workflow automation engine |
| **Telegram Bot API** | Sending notifications |
| **Gemini / LLM Node** | Structured data extraction |
| **Webhook Triggers** | Listens for incoming emails |

---

## 📥 Getting Started

### 🔧 Prerequisites

- n8n instance (cloud or self-hosted)
- Telegram bot token (via BotFather)
- Endpoint for email webhook events

### 🧩 Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/aswinajith/placementbot.git
   cd placementbot

