<div align="center">

# Nate Merkl

### Solo developer at Suqnet

[Suqnet website](https://suqnet.com) · [Open Suqnet](https://app.suqnet.com/auth) · [iPhone app](https://apps.apple.com/tr/app/suqnet/id6791631997)

</div>

---

## Building Suqnet

[Suqnet](https://suqnet.com) is the inventory, POS, and business-management workspace I am building for Ethiopian shops. It keeps sales, stock, cash, expenses, customer credit, and reports in one place.

The product starts where a lot of shop work already starts: with a photo. A shop owner can photograph a receipt, invoice, or stock list, review the lines, correct anything that is wrong, and then choose whether it becomes inventory, a sale, or an expense. Nothing is saved before that review.

Suqnet runs in the browser, and the [iPhone app](https://apps.apple.com/tr/app/suqnet/id6791631997) is available now. Android is still on the way.

## The work behind it

I build the whole product: the customer-facing interface, the API and data model, document intake, deployment, and the small operational details that decide whether shop software gets used after the first week.

The hard part is rarely putting a model behind an upload button. A receipt is an unreliable document: names are shortened, quantities are ambiguous, supplier formats change, and a clean-looking scan can still return the wrong order. I build the review step and data boundaries around that reality.

My work is strongest where business workflows meet messy documents and imperfect connectivity:

| Area | What I work on |
| --- | --- |
| Document AI and OCR | Receipt and invoice extraction, page structure, review flows, and data that can be traced back to the source document. |
| Inventory and retail systems | Product records, stock movement, sales, cash, expenses, customer credit, staff roles, and reporting. |
| Full-stack product engineering | TypeScript, React, Next.js, Python, FastAPI, PostgreSQL, Supabase, Redis, Docker, and GitHub Actions. |
| Local product constraints | Mobile-first workflows, low-bandwidth use, Ethiopian business context, and decisions that remain understandable to the person running the shop. |

## How I make product decisions

I do not choose infrastructure from a feature checklist. I start with the record that has to stay correct, the person who has to correct it, and the failure that would cost them money.

That is why Suqnet asks for confirmation before a photo changes stock. OCR output needs structure, review, and extracted text that stays tied to the document. The useful question is whether a shop owner can trust the result on a busy day.

## Find me

[Suqnet](https://suqnet.com) · [Web app](https://app.suqnet.com/auth) · [iPhone app](https://apps.apple.com/tr/app/suqnet/id6791631997) · [Email](mailto:natemerkl@gmail.com) · [X](https://x.com/natemerkl)
