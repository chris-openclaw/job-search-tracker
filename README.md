# Job Search Tracker

An OpenClaw skill that tracks job applications from discovery to offer, flags stale applications, and helps with follow-up emails, cover letters, and interview prep.

## What it does

- **Tracks applications** in a single markdown file with status, contacts, timeline, salary, resume version, and follow-up dates
- **Detects stale applications** and flags anything that needs attention (no response in 7+ days, overdue follow-ups, upcoming interviews)
- **Generates a dashboard** with pipeline counts, recent activity, and actionable next steps
- **Drafts follow-up emails, cover letters, and thank-you notes** using context from your tracker
- **Preps you for interviews** with company research briefs, mock questions, and talking points mapped to the role
- **Integrates with Gmail** to scan for application confirmations and pull recruiter email context
- **Integrates with LinkedIn** to track Easy Apply submissions and research companies/contacts

All integrations are optional. The skill works well with just what you tell it directly.

## Install

```bash
openclaw skill install chris-openclaw/job-search-tracker
```

## Example prompts

- "I just applied to a Product Manager role at Stripe. Track it."
- "What needs attention in my job search?"
- "I have an interview with Notion on Thursday. Prep me."
- "Draft a follow-up email for the Datadog recruiter."
- "Check my email for any new application confirmations."
- "I got rejected from Shopify."

## How it stores data

Everything lives in `applications.md` in your working directory. Each company gets its own section with status, contacts, timeline, notes, and follow-up info. The file is plain markdown, so you can read and edit it yourself anytime.

## License

MIT-0
