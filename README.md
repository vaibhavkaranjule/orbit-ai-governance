# ORBIT - Intelligent Delivery Governance

> AI-powered project artefact intelligence for complex multi-scope delivery programmes

[![Capgemini–Microsoft Agentic Industry Hackathon 2026](https://img.shields.io/badge/Capgemini%E2%80%93Microsoft%20Agentic%20Industry%20Hackathon%202026-BRING%20YOUR%20CLIENT-0096C7?style=flat-square)](https://github.com/vaibhavkaranjule/orbit-ai-governance)
[![Client: Capgemini](https://img.shields.io/badge/Client-Capgemini-1E3A5F?style=flat-square)](https://www.capgemini.com)
[![Cross-Sector](https://img.shields.io/badge/Applicable-Any%20Sector%20%7C%20Any%20Client-00B4D8?style=flat-square)]()
[![Azure AI](https://img.shields.io/badge/Azure%20AI%20Foundry-GPT--4o-0078D4?style=flat-square&logo=microsoftazure)](https://azure.microsoft.com/en-us/products/ai-foundry/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)

---

## The Problem

In complex delivery programmes, governance fails silently. Commitments made in meetings go untracked. Risk signals are buried in email chains and documents. Programme Managers spend 30–40% of their time reconstructing status instead of acting on it.

**This is not a process problem. It is an information architecture problem.**

ORBIT is built to solve it.

---

## What ORBIT Does

ORBIT (Operational Risk & Business Intelligence Tracker) is an AI-powered governance assistant that continuously ingests project artefacts, extracts commitment and risk intelligence using Azure AI Foundry GPT-4o, and presents Programme Managers with a real-time governance dashboard - with zero manual input required.

| Capability | Description |
|---|---|
| **Artefact Ingestion** | Auto-ingest emails, Teams messages, documents, and tickets via Microsoft Graph API |
| **Commitment Extraction** | GPT-4o identifies owners, due dates, dependencies, and risk signals in natural language |
| **Governance Dashboard** | Real-time health score across all delivery scopes — one view, zero manual effort |
| **Proactive Alerts** | Azure Event Grid triggers escalation before deadlines or SLA thresholds are missed |
| **Natural Language Query** | Copilot Studio bot answers "What is overdue this week?" directly in Teams |

---

## Origin · Target · Applicability

| | |
|---|---|
| **Inspired by** | Real challenges in multi-scope enterprise delivery programmes |
| **Primary deployment target** | **Capgemini** delivery organisation |
| **Cross-sector applicable** | Any organisation managing complex multi-scope delivery — professional services, banking, energy, public sector, manufacturing |

**The illustrative scenario:**
- **>€150K/month** in delivery value at risk across 5 concurrent scopes\*
- A governance breakdown left **800+ commitment artefacts** untracked\*
- Resolved the backlog in **6 weeks without tooling** - preventing an estimated **€40–60K in impact**\*
- No system existed to surface this early or detect the gap proactively

ORBIT is built to make that scenario impossible — for Capgemini, and for any delivery programme.

> *\*Figures are illustrative, based on representative programme characteristics.*

---

## Architecture

```
┌──────────────────┐   ┌──────────────────────┐   ┌─────────────────┐   ┌──────────────────┐
│   DATA SOURCES   │──▶│   INGESTION LAYER    │──▶│   AGENT LAYER   │──▶│  OUTPUT LAYER    │
│                  │   │                      │   │                 │   │                  │
│ MS Teams         │   │ Microsoft Graph API  │   │ Azure AI Foundry│   │ Power BI         │
│ Outlook          │   │ Azure Document       │   │ (GPT-4o)        │   │ Governance Dash  │
│ SharePoint       │   │ Intelligence         │   │                 │   │                  │
│ Azure DevOps     │   │                      │   │ Azure Event Grid│   │ Copilot Studio   │
└──────────────────┘   └──────────────────────┘   │ (trigger)       │   │ Teams Bot        │
                                                   └───────┬─────────┘   │                  │
                                                           │             │ Power Automate   │
                                                  ┌────────▼────────┐    │ Alerts           │
                                                  │    STORAGE      │    └──────────────────┘
                                                  │ Azure Cosmos DB │
                                                  │ Azure AI Search │
                                                  └─────────────────┘
```

**Two-agent pipeline: (has multiple agents orchestrating simlar schematics)**
- **Agent 1 : Ingestion & Extraction:** Ingests artefacts, extracts commitments, classifies risk, validates and deduplicates → *Commitments Logged*
- **Agent 2 : Governance & Alert:** Monitors programme health, generates reports, triggers escalations — Programme Manager holds the human decision gate → *Governance Actioned*

**Technology Stack:** Azure AI Foundry · GPT-4o · Microsoft Graph API · Azure Document Intelligence · Azure Cosmos DB · Azure Event Grid · Azure AI Search · Microsoft Fabric · Copilot Studio · Power Automate · Power BI · GitHub

---

## Business Value

| Metric | Target |
|---|---|
| Governance reporting reduction | 80% less manual effort\* |
| PM time recovered | 4–6 hours/week per programme\* |
| Governance gaps surfaced proactively | 65% before escalation\* |
| Risk escalation speed | 50–70% faster\* |
| Break-even | ~5–6 months via PM time savings alone\* |

> *\*Illustrative estimates for demonstration purposes.*

---

## Project Status

**Phase: Semi-Finals Submission** - Capgemini × Microsoft Agentic Industry Hackathon 2026

> Built end-to-end: problem definition, architecture, business case, and submission. Implementation begins April 2026 following environment provisioning.

---

## Team

**Team ORBIT** — Capgemini × Microsoft Agentic Industry Hackathon 2026 · Track: BRING YOUR CLIENT

- **Vaibhav Karanjule** - Delivery Leader & AI Product Development, Capgemini Engineering
  [linkedin.com/in/vaikaranjule](https://www.linkedin.com/in/vaikaranjule)

- **Qi Lutter-Yin** — Capgemini Engineering

---

## Repository Contents

Will upload soon

---

## License

MIT — see [LICENSE](LICENSE)

