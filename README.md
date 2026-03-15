<div align="center">

# Shipped a live AI inventory SaaS. Building the open-source infrastructure behind it.

[![StockSyncAI — Live Product](https://img.shields.io/badge/StockSyncAI-Live%20Product-3ECF8E?style=flat&logoColor=white)](https://stocksyncai.com)

</div>

---

### The product — StockSyncAI

**[stocksyncai.com](https://stocksyncai.com)** — AI-powered inventory management built for Ethiopian businesses. Live, priced, and serving 500+ businesses across Ethiopia.

Ethiopian retail runs on spreadsheets. StockSyncAI replaces them with real-time multi-warehouse tracking, AI demand forecasting, OCR receipt scanning with Amharic and Afaan Oromoo support, theft detection, and full local tax compliance — ETR, VAT, WHT — at up to 80% less than international alternatives.

| Plan | Price | Target |
|------|-------|--------|
| Free | ETB 0 | Micro businesses |
| Starter | ETB 499/mo | Small businesses with tax compliance |
| Pro | ETB 1,299/mo | Growing businesses — multi-warehouse, AI features |
| Enterprise | ETB 3,999/mo | Large enterprises — unlimited users, full compliance |

Built from scratch. Designed for low-bandwidth environments, local currency (ETB), local tax rules, and local languages. Not a fork of an international tool — a ground-up system designed around how Ethiopian retail actually works.

---

### Open-source infrastructure extracted from the platform

The hard problems StockSyncAI solved in production are becoming standalone tools:

| Project | What it does |
|---------|-------------|
| [`invoice-ocr-pipeline`](https://github.com/Natemerkl/invoice-ocr-pipeline) | FastAPI service — extracts structured JSON from supplier invoices via OCR + GPT-4o. Async jobs, webhook delivery |
| [`stocksync-engine`](https://github.com/Natemerkl/stocksync-ai) | The sync engine: multi-supplier import, AI product normalization, atomic PostgreSQL transactions, conflict resolution |
| [`ocr-document-toolkit`](https://github.com/Natemerkl/ocr-document-toolkit) | Unified Python CLI + library over Google Vision / Tesseract / EasyOCR — one interface, swappable backends |
| [`saas-infra-kit`](https://github.com/Natemerkl/saas-infra-kit) | Next.js 14 + Supabase SaaS boilerplate — auth, Stripe billing, multi-tenancy, RLS policies, CI/CD |
| [`pg-sync-utils`](https://github.com/Natemerkl/pg-sync-utils) | PostgreSQL patterns for SaaS — audit logs, soft deletes, updated_at triggers, RLS templates |

---

### Stack

**Backend**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)

**Frontend**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black)

**AI / Automation**

![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Vision-4285F4?style=flat&logo=google-cloud&logoColor=white)

**Data**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat&logo=supabase&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)

**Infrastructure**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=github-actions&logoColor=white)

---

### What building a market-specific SaaS teaches you

Shipping StockSyncAI meant solving problems international tools ignore entirely:

- **Localization at the data layer** — ETB currency, Ethiopian tax rules, and Amharic character sets enforced in the database, not patched in the UI
- **Offline-tolerant sync** — unreliable connectivity means sync conflicts are a first-class problem, not an edge case
- **Tax compliance as infrastructure** — ETR, VAT, and WHT rules baked into the transaction model from day one, not bolted on later
- **Multi-language OCR** — scanning receipts in Amharic script required custom preprocessing pipelines beyond standard API calls

These are the real engineering problems the open-source repos above are built to solve.

---

### Currently building

```
[ Shipped ]  stocksyncai.com      — live, 500+ Ethiopian businesses
[ Active  ]  invoice-ocr-pipeline — async job queue + webhook delivery
[ Active  ]  stocksync-engine     — open-source sync engine extraction
[ Soon    ]  pg-sync-utils        — PostgreSQL SaaS patterns
[ Soon    ]  ai-data-pipeline     — stage-based document processing framework
```

---

### Let's talk

Building in **emerging market tech**, **AI document processing**, **SaaS infrastructure**, or **retail automation**?

[![StockSyncAI](https://img.shields.io/badge/Product-stocksyncai.com-3ECF8E?style=flat)](https://stocksyncai.com)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:natemerkl@gmail.com)
[![X](https://img.shields.io/badge/X-000000?style=flat&logo=x&logoColor=white)](https://x.com/natemerkl)

---

<div align="center">
<sub>Founder · StockSyncAI · Shipping from Ethiopia & Amsterdam</sub>
</div>
