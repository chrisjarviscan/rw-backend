---
name: refresh-rw-dashboard
description: Refresh the RW Meeting Intelligence Dashboard with local transcript files and calendar data, compute action item priorities and cross-meeting dependencies, and update the Priorities and Actions tab. Runs daily at 8:08am.
---

You are refreshing the RW Meeting Intelligence Dashboard with the latest data from local transcript files and Outlook calendar, and computing action item priorities and dependencies.

## Context
The Meeting Intelligence Dashboard is an HTML-based dashboard located at ~/Dev/rw-dashboards/ that visualizes meeting patterns, client engagement frequency, and action item tracking from local Fathom transcript files and Outlook calendar data. The Fathom MCP connector is NOT available. All transcript data comes from local .md files synced nightly by fathom_sync.py.

## Steps

### Phase 1: Data Collection
1. Read the dashboard technical documentation at /Users/realizedworth/Documents/Claude-AI-Config/memory/projects/meeting-intelligence-dashboard.md
2. Request access to the Transcripts folder using request_cowork_directory with path /Users/realizedworth/Documents/Transcripts if not already mounted. Pull latest transcript data by reading .md files from both: (a) /Users/realizedworth/Documents/Transcripts/FathomTranscripts/ (date-prefixed .md files with full transcripts, summaries, and action items), and (b) /Users/realizedworth/Documents/Transcripts/📅 2026/TRANSCRIPTS - ALL 2026/ (.md and .docx files). Use Glob to find files from the last 30 days, then Read each to extract title, date, attendees/speakers, action items, key topics, and summary.
3. Pull latest calendar data: use outlook_calendar_search with query "*" for last 30 days. Cross-reference with transcript data.
4. Process and structure the data per the technical spec.

### Phase 2: Priority Engine
5. Flatten and score all action items (0-100 scale):
   - Org type base: Client=40, Partner=30, Sales=25, Internal=10
   - Staleness: 0-1 days=+30, 2-3=+20, 4-7=+10, 7+=+5
   - Cross-meeting recurrence (3+ meetings): +20
   - Urgency keywords: +10
   - Assign urgency_level: critical (80+), high (60-79), medium (40-59), low (<40)
6. Detect dependencies: high-frequency clients (3+ meetings), bandwidth risks (4+ orgs per assignee), shared deliverables.
7. Build full_action_list grouped by org type, sorted by priority_score.

### Phase 3: File Updates
8. Write priority data to /Users/realizedworth/Dev/rw-dashboards/data/dashboard_data.json with priority_actions section.
9. Update /Users/realizedworth/Dev/rw-dashboards/index.html: inject priority data into window.PRIORITY_DATA.
10. Update other data files per technical spec. Append/merge, never overwrite historical data.
11. Verify: dashboard_data.json has top_priorities with 1+ items, index.html has PRIORITY_DATA, report counts and timestamp.

### Phase 4: Memory Write-Back
12. Read the Meeting Intelligence section of /Users/realizedworth/Documents/Claude-AI-Config/memory/rw-brain.md
13. Compare against today's dashboard findings. Look for:
    - New high-frequency clients (3+ meetings in 30 days not previously noted)
    - Bandwidth risks (assignees with 4+ active orgs not previously noted)
    - Cross-meeting dependencies that have emerged or resolved
    - Clients that have gone quiet (no meetings in 14+ days after prior high frequency)
14. If new patterns are detected, append dated entries to the Meeting Intelligence section:
    `| YYYY-MM-DD | [pattern description] | Dashboard refresh |`
15. If action items have been resolved or are stale (7+ days, no update), note in brain file
16. Update the "Last updated" timestamp in rw-brain.md
17. Report: "Brain file updated with N new patterns" or "No new patterns detected — brain file unchanged"

## Rules
- No fabricated data. Every record traces to a real local transcript file or calendar event.
- Preserve historical data.
- Use ISO 8601 timestamps.
- If local transcripts or Outlook is unavailable, report which source failed. Do NOT attempt to call Fathom MCP tools (search_meetings, list_meetings, get_meeting_details, get_meeting_transcript). They are disconnected.
- Phase 4 is silent — do not prompt user for confirmation on meeting intelligence writes. These are automated observations, not decisions. Do confirm before writing any decision or project update.