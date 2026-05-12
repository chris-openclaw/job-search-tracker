# Job Search Tracker

An OpenClaw skill that tracks job applications from discovery to offer, flags stale applications, and helps with follow-up emails, cover letters, salary negotiation, and interview prep.

**Current version: 1.1.0**

## What's new in 1.1.0

- **Salary Negotiation**: triggers on "got an offer" and runs gap analysis, counter-offer drafting, and pressure-tactic flagging (exploding offers, verbal-only, below-range)
- **Resume Recommender**: matches stored resume variants from a `resumes/` directory against new postings and suggests the best fit
- **Tone Check**: flags desperate, templated, or negative-framing language in user-drafted emails and cover letters before sending

See [CHANGELOG.md](CHANGELOG.md) for the full release history.

## What it does

- **Tracks applications** in a single markdown file with status, contacts, timeline, salary, resume version, and follow-up dates
- **Detects stale applications** and flags anything needing attention (no response in 7+ days, overdue follow-ups, upcoming interviews)
- **Generates a dashboard** with pipeline counts, recent activity, and actionable next steps
- **Drafts follow-up emails, cover letters, and thank-you notes** using context from your tracker
- **Recommends the best resume variant** for each posting (1.1.0)
- **Tone-checks your drafts** for desperate or templated language (1.1.0)
- **Supports salary negotiation** with counter-offer analysis and drafting (1.1.0)
- **Preps you for interviews** with company research briefs, mock questions, and talking points
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
- "Which resume should I send for this posting?"
- "Does this follow-up email sound desperate?"
- "I have an interview with Notion on Thursday. Prep me."
- "Draft a follow-up email for the Datadog recruiter."
- "I got an offer from Linear — help me think through the counter."
- "Check my email for any new application confirmations."
- "I got rejected from Shopify."

## How it stores data

Everything lives in `applications.md` in your working directory. Each company gets its own section with status, contacts, timeline, notes, and follow-up info. The file is plain markdown, so you can read and edit it yourself anytime.

Resume variants live in a sibling `resumes/` directory if you want the recommender feature.
