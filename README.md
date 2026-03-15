<div align="center">

# Building AI-powered inventory automation for retail.

**StockSyncAI** · Invoice OCR pipelines · SaaS infrastructure · Developer tooling

</div>

---

### What I'm shipping

I build backend-heavy systems that automate the tedious parts of running a retail business — supplier invoice processing, multi-source inventory sync, ERP data pipelines. Right now that means:

- **StockSyncAI** — AI inventory sync engine for retail. Imports multi-supplier Excel/CSV templates, normalizes product data with GPT-4o, and commits atomically to PostgreSQL. Handles conflict resolution across suppliers.
- **Invoice OCR Pipeline** — FastAPI service that extracts structured JSON from supplier invoices using Google Vision + GPT-4o. Built for retail and wholesale ops teams replacing manual data entry.
- **OCR Document Toolkit** — Unified Python library wrapping Google Vision, Tesseract, and EasyOCR behind one interface. Adapter pattern. Swappable backends, consistent output.

---

### Signature projects

| Project | What it does |
|---------|-------------|
| [`stocksync-ai`](https://github.com/Natemerkl/stocksync-ai) | Atomic inventory sync engine — multi-supplier, AI normalization, rollback-safe PostgreSQL transactions |
| [`invoice-ocr-pipeline`](https://github.com/Natemerkl/invoice-ocr-pipeline) | FastAPI + Google Vision + GPT-4o → structured invoice JSON. Async job queue, webhook delivery |
| [`ocr-document-toolkit`](https://github.com/Natemerkl/ocr-document-toolkit) | Python CLI + library. Unified adapter over Google Vision / Tesseract / EasyOCR |
| [`saas-infra-kit`](https://github.com/Natemerkl/saas-infra-kit) | Next.js 14 SaaS boilerplate — Supabase auth, Stripe billing, multi-tenancy, RLS, CI/CD |

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

### Architecture principles

- **Atomic or nothing** — if a sync touches 500 rows and row 300 fails, nothing commits. No partial state.
- **Observable** — every job has a status, a log, and a failure reason. Silent failures are bugs.
- **Swappable** — OCR backend, AI model, storage layer. Nothing hardcoded to a vendor.

---

### Currently building
```
[ Active ]  stocksync-ai         — conflict resolution + dry-run diff API
[ Active ]  invoice-ocr-pipeline — async job queue + webhook delivery
[ Soon   ]  pg-sync-utils        — PostgreSQL patterns for SaaS
[ Soon   ]  ai-data-pipeline     — stage-based async document processing
```

---

### Let's talk

Building something in **retail tech**, **SaaS infrastructure**, or **AI document processing**?

[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:YOUR_EMAIL_HERE)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR_LINKEDIN)
[![X](https://img.shields.io/badge/X-000000?style=flat&logo=x&logoColor=white)](https://x.com/YOUR_X_HANDLE)

---

<div align="center">
<sub>Principal Architect · StockSyncAI · Amsterdam</sub>
</div>
```

Scroll to the bottom, click **"Commit changes"**, write the commit message:
```
docs: add profile README with projects and stack
```

Click **Commit changes**.

---

## Step 4 — Set the repo description

This is the one-liner that appears under the repo name everywhere on GitHub.

In your `Natemerkl` repo, look for the **"About"** section on the right side. Click the **gear icon ⚙** next to it.

**Description field — paste this exactly:**
```
GitHub profile · Building AI inventory automation for retail
