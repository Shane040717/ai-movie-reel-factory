# Setup

## 1. n8n
Import `workflows/n8n_daily_content_workflow.json` into n8n.

## 2. Environment / credentials
Configure your OpenAI credential in n8n. Configure your chosen social publishing provider/API credentials separately. Keep credentials in n8n's credential store or environment secrets; never put tokens in workflow JSON.

## 3. Product settings
Edit `config/product.json` for offer price, audience, platforms and cadence.

## 4. Calendar
Import `data/content_calendar.csv` into Google Sheets or another database and connect it to the workflow.

## 5. Approval
Use the approval node as a hard gate. A human should review healthcare claims before a post is published.

## 6. Publishing
Connect the publishing node to the APIs/accounts you actually control. The starter workflow intentionally uses a webhook-style publishing adapter so you can choose a compliant scheduler/provider.

## 7. Test mode
Run the workflow with publishing disabled. Confirm generated JSON, QA output, approval routing and logging. Only then enable your publishing adapter.
