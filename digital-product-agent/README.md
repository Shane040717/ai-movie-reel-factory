# AI Healthcare Growth Agent

Production-ready starter for automating marketing operations for the AI Healthcare Growth Kit.

## Architecture

`Scheduler/Webhook -> Content Planner -> AI Generation -> Safety/QA -> Approval -> Publishing Adapter -> Analytics -> Weekly Optimization`

The system is intentionally approval-first for healthcare content. It does **not** autonomously publish clinical claims without human review.

## Included

- `config/product.json` — product, audience, offers and content pillars
- `prompts/content_agent.md` — master content-generation instructions
- `prompts/qa_agent.md` — safety and quality gate
- `workflows/n8n_daily_content_workflow.json` — importable n8n workflow blueprint
- `data/content_calendar.csv` — starter 30-day queue
- `docs/SETUP.md` — setup and credential instructions
- `docs/OPERATIONS.md` — daily/weekly operating playbook

## Required credentials

Configure your own OpenAI/API credentials and the publishing provider/API accounts you choose. Never commit secrets, refresh tokens, cookies, or webhook credentials.

## Recommended flow

1. Import the n8n workflow.
2. Configure OpenAI and your publishing/scheduling provider.
3. Connect the approval destination (email/Slack/Telegram/etc.).
4. Test with draft-only mode.
5. Review generated healthcare claims.
6. Enable publishing only after QA and approval are confirmed.

## Product

AI Healthcare Growth Kit — 250 AI prompts + 30-day content calendar + healthcare marketing toolkit.

Suggested primary offer: ₹1,999. Agency/commercial tier: ₹4,999.

## Disclaimer

This automation is a marketing/content system, not a medical device or medical advice system. All healthcare content must be reviewed for clinical accuracy, privacy, advertising rules and applicable platform policies before publication.
