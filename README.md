# PR-Triage: AI Code Reviewer for Slack/Discord

PR-Triage is an intelligent, collaborative workspace bridge that automates code analysis, bug triaging, and Pull Request (PR) workflows directly inside your team messaging app.

## 🏆 Hackathon Tracks Entered
* **Track 1: Best Business Workflow** – Automates engineering team code reviews and triaging right inside the active chat channel, eliminating browser context-switching.
* **Track 3: Best Core Contribution** *(Optional / Pending)* – Connecting custom open-source adapters back to the core Switch repository.

---

## 💡 The Problem & Solution
Engineering teams lose significant time context-switching between GitHub, terminal windows, and communication hubs. PRs stall waiting for human eyes, and simple code flaws slip through. 

**PR-Triage** brings the AI coding agent directly into your natural conversational flow. Drop a PR link in chat, and your AI agent instantly runs static analysis, generates line-by-line feedback, and executes code updates based on conversational human instructions—all without leaving your chat window.

---

## 🛠️ Architecture & How Switch is Used
**Switch is the central nervous system of this project.** It acts as the secure, bidirectional bridge handling the heavy lifting between our communication layer and the AI execution brain.

1. **Frontend / Communication:** Slack / Discord / Telegram capturing user commands and threaded conversations.
2. **Orchestration Layer (Switch):** Intercepts events from the messaging app, handles state, formats text payloads, and routes requests to the AI coding agent. It then pipes structured markdown reviews back into the correct chat threads.
3. **AI Brain:** Claude Code / Codex digesting repository diffs, analyzing logic, and prepping code commits.

---

## 🚀 Prerequisites
Before setting up, ensure you have the following installed and configured:
* **Node.js** (v18+ recommended)
* A **Switch** account and the Switch CLI installed
* Developer credentials for your messaging app (Slack App Token / Discord Bot Token)
* An API key for your chosen AI Agent (e.g., Anthropic API key for Claude Code)

---

## ⚙️ Installation & Setup Instruction

### 1. Clone the Repository
```bash
git clone https://github.com
cd switch-ai-code-reviewer
```

### 2. Install Dependencies
```bash
npm install express dotenv body-parser axios
```

### 3. Configure Environment Variables
Create a `.env` file in the root directory:
```env
PORT=3000
SWITCH_API_KEY=your_switch_api_key_here
```

### 4. Run the Application
```bash
node index.js
```
# 🚀 LAUNCH DEAL: NOW A NATIVE MCP SERVER FOR CURSOR & CLAUDE CODE!

We just launched on Agensi! You can now run automated PR triages and security audits locally inside your IDE. 

🔥 **7-DAY LAUNCH SALE:** Get it for **$5.09/mo** (Standard $6.00/mo) before the deal expires!
👉 **[GET THE LATEST DEAL ON AGENSI.IO]** *(Paste your live listing link here)*
