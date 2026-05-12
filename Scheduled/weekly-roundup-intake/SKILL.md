---
name: weekly-roundup-intake
description: Run weekly RWI Roundup intake: read PDFs, search Outlook, web research, merge carry-forward, produce draft for Chris to review.
---

You are running the weekly intake for the RWI Roundup newsletter. Follow these instructions exactly.

## Context
The RWI Weekly Roundup is a curated CSR/social impact newsletter published by the RW Institute. Chris Jarvis curates content and sends it via Mailchimp. Your job is Phase 1: intake and draft generation.

## Steps

1. Read the reference files:
   - Read /Users/realizedworth/My Drive (chrisjarvis@realizedworth.com) (1)/INTERNAL/Operations/Work in Progress 2025/2.RWI - WORK IN PROGRESS 2025 copy/3.RWI - SCOPE 1/ROUNDUP/CLAUDE.md for full specs
   - Read /Users/realizedworth/My Drive (chrisjarvis@realizedworth.com) (1)/INTERNAL/Operations/Work in Progress 2025/2.RWI - WORK IN PROGRESS 2025 copy/3.RWI - SCOPE 1/ROUNDUP/_previous_items.json for carry-forward items

2. Find this week's intake folder: list the ROUNDUP directory, look for the most recent Roundup MM.DD.YY/ folder. If no new folder exists, proceed with carry-forward + Outlook + web research only.

3. Read all PDFs in the intake folder using PDF tools. For each, extract: title, hosting org, org URL, dates/location, description, CTA URL. Categorize into: events, surveys, reports, or recordings. Skip spam or non-CSR content.

4. Search Outlook inbox (via Office 365 MCP) for emails from the past 7 days. Search terms: "CSR", "corporate citizenship", "volunteer engagement", "social impact", "nonprofit", "philanthropy", "ESG", "conference", "webinar", "report". Extract relevant items, deduplicate against PDF items.

5. Web research: search for notable CSR events, reports, or resources from the past week. Focus on: Points of Light, Imagine Canada, ACCP, BCCCC, Engage for Good, Volunteer Canada, ALIVE, CECP, Candid, GivingTuesday, IAVE, Volunteer Match, Out and Equal, Do Some Good.

6. Merge carry-forward items from _previous_items.json. Events: keep only if event date is AFTER today. Surveys: keep if still open. Reports/Recordings: keep all. Carry-forward items do NOT get [NEW] tag.

7. Tag [NEW] items: any item NOT in _previous_items.json (by fuzzy title match) gets [NEW].

8. Generate intake summary: save _intake_summary.md in the intake folder with stats, triage table, and each section with full item details.

9. Generate the Mailchimp HTML automatically. Use inline styles only. Follow the item format from CLAUDE.md. Save as ROUNDUP_[YYYY-MM-DD]_MAILCHIMP.html in the ROUNDUP root folder.

10. Notify Chris: summarize total items, new items, carry-forward, dropped, any issues. Provide file path to HTML. Flag verification-needed items.

## Rules
- No em dashes. Use commas or periods.
- Descriptions should be factual, not marketing copy.
- No fabricated data, orgs, or URLs.
- Use Desktop Commander start_process with cat commands to read .md and .json files from Google Drive paths.
- The ROUNDUP root is: /Users/realizedworth/My Drive (chrisjarvis@realizedworth.com) (1)/INTERNAL/Operations/Work in Progress 2025/2.RWI - WORK IN PROGRESS 2025 copy/3.RWI - SCOPE 1/ROUNDUP/