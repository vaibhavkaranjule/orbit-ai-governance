# ORBIT — AI-Powered Delivery Governance Tool

> *Automatically extracts commitments from emails and documents, tracks deadlines in real time, and lets your team query project status in plain English via Microsoft Teams.*

Built as a submission for the **Capgemini IDG Hackathon 2026** (March 2026).

---

## The Problem

In large aerospace programmes, critical commitments like deadlines, action items, supplier promises that are buried in hundreds of emails and meeting notes every week. By the time a deadline is missed, it is already too late. Programme managers spend hours manually chasing status instead of resolving issues.

**ORBIT turns that reactive loop into a proactive, automated governance system.**

---

## What It Does

| Step | What Happens |
|------|-------------|
| 1. Email arrives | Power Automate detects it and sends content to Azure AI Foundry (GPT-4o) |
| 2. AI extracts commitments | GPT-4o identifies deadlines, owners, and action items from natural language |
| 3. Data is stored | Extracted commitments are written to a SharePoint List automatically |
| 4. Alerts fire | Power Automate sends proactive Teams alerts 3 days before any deadline |
| 5. Dashboard updates | Power BI dashboard shows live commitment health across the programme |
| 6. Team queries in plain English | Copilot Studio bot answers "What is overdue this week?" directly in Teams |

---

## Architecture
```
Emails / Documents
        ↓
Power Automate (trigger)
        ↓
Azure AI Foundry GPT-4o (commitment extraction)
        ↓
SharePoint List (structured data store)
        ↓
┌───────────────────┬──────────────────────┐
Power BI Dashboard   Copilot Studio Teams Bot
(live governance)    (natural language query)
```

---

## Tech Stack

- **Azure AI Foundry** - GPT-4o for natural language commitment extraction
- **Microsoft Power Automate** - email trigger, AI call, SharePoint write, Teams alert
- **SharePoint Lists** - structured commitment data store
- **Microsoft Power BI** - live governance health dashboard
- **Copilot Studio**- conversational Teams bot for status queries
- **GitHub** - version control and documentation

---

## Repository Contents

| File | Description |
|------|-------------|
| `ORBIT_Architecture_Wireframe.html` | Interactive architecture diagram |
| `ORBIT_Hackathon_Handbook.docx` | Step-by-step build guide |
| `ORBIT_UseCase_Document.docx` | Use case, user stories, and prototype specification |
| `ORBIT_Hackathon_Deck.pptx` | Pitch deck ppt submitted to Capgemini IDG Hackathon 2026 |

---

## Key Results

- Eliminates manual commitment tracking - **zero spreadsheets, zero chasing**
- Proactive deadline alerts - **3-day advance warning** to responsible owners
- Natural language programme status - **instant answers** without opening any system
- Estimated time saving: **5–8 hours/week** per programme manager

---

## About

Built by **Vaibhav Karanjule** - Technical Project Leader at Capgemini Engineering, specialising in aerospace supply chain transformation and AI product development.

- **LinkedIn:** [linkedin.com/in/vaikaranjule](https://linkedin.com/in/vaikaranjule)
- **Background:** 4+ years leading cross-regional teams on Airbus/Satair programmes; originator of AI-driven SDR prediction model (InsightBridge)

---

## License

MIT License - see [LICENSE](LICENSE) for details.
