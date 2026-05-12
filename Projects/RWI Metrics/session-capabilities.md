# Session Capability Inventory
**Generated:** 2026-03-27 | **Session:** focused-laughing-darwin

---

## 1. MCP Connections — Status

| Service | Status | Notes |
|---------|--------|-------|
| **Outlook Email** (M365) | LIVE | Search, read, filter emails. Working. |
| **Outlook Calendar** (M365) | LIVE | Search events, find availability. Working. |
| **Teams Chat** (M365) | LIVE | Search chat messages, KQL supported. Working. |
| **SharePoint** (M365) | LIVE | Search docs/pages, folder search. Working. |
| **Fathom** | LIVE | List teams, search meetings, get transcripts, meeting details. Teams: RW, RWI, RW-Angela, RWI-Technology Review. |
| **Smartsheet** | LIVE | 8 workspaces visible (RW Marketing, RW Project Management, RWI Projects, Hours Tracking, etc.). Full CRUD on sheets/rows/columns/discussions. |
| **Google Drive** | LIVE | Search and fetch files. Responded (empty result on test query, but authenticated). |
| **Benevity** | LIVE | Nonprofit search and details. Working. |
| **PubMed** | ERROR | Returned server error on test query. May be intermittent. Retry before declaring unavailable. |
| **Notion** | AVAILABLE | Tools loaded (search, find, create-page, create-task, database-query, create-database-row). Not ping-tested but schema loaded. |
| **Claude in Chrome** | AVAILABLE | Browser automation: navigate, read page, form input, screenshots, JS execution, tabs, GIF creator. |
| **Control Chrome** | AVAILABLE | Tab management, JS execution, page content, navigation. |
| **Desktop Commander** | AVAILABLE | File ops, process management, search, PDF writing. |
| **PDF Tools (Fill/Analyze/Extract)** | AVAILABLE | Fill PDFs, extract to CSV, bulk fill, read fields, profiles, validation. |
| **PDF (Anthropic)** | AVAILABLE | Display and read PDFs. |
| **PowerPoint (Anthropic)** | AVAILABLE | Create/open/edit/save presentations, add slides, insert images, export PDF. |
| **Word (Anthropic)** | AVAILABLE | Create/open/edit/save Word docs, format text, replace, export PDF. |
| **Cowork** | AVAILABLE | Present files, request directory, allow file delete. |
| **Scheduled Tasks** | AVAILABLE | Create, list, update scheduled tasks. |
| **MCP Registry** | AVAILABLE | Search for and suggest new MCP connectors. |
| **Plugins Registry** | AVAILABLE | Search and suggest plugin installs. |
| **Session Info** | AVAILABLE | List sessions, read transcripts. |

---

## 2. Installed Plugins

### Remote Plugins (Custom — Chris Jarvis)

| Plugin | ID | Version | Description |
|--------|----|---------|-------------|
| **rwi-team** | plugin_01TCnjphtuwpMX9wnftAURsL | 1.0.0 | RW Institute team plugin. 19 skills for program delivery, research, facilitation, Makerspace. |
| **rw-chris-personal** | plugin_01TguJ7CVYexf7ru3HtPuqpR | 2.0.0 | Chris Jarvis personal plugin. Full skill suite for RW/RWI work, voice, BD pipeline, meta skills. |
| **rw-team** | plugin_01MwHUshjbstuhGWNzsiDhbG | 1.0.0 | RW consulting team plugin. 28 skills for client delivery, proposals, meetings, docs, file management. |

### Local/Cached Plugins (Official)

cowork-plugin-management, claude-code-setup, claude-md-management, code-review, code-simplifier, coderabbit, feature-dev, frontend-design, github, gitlab, greptile, hookify, Notion, pinecone, plugin-dev, pyright-lsp, security-guidance, sentry, slack, supabase, superpowers

---

## 3. Skills Inventory (28 Local + mirrored across 3 remote plugins)

### Document Creation
- **docx** — Create, read, edit Word documents. Branded formatting, TOC, headers, page numbers.
- **pptx** — Create/edit PowerPoint presentations. PptxGenJS-based. Read/parse existing decks.
- **pdf** — PDF manipulation: extract, merge, split, create, fill forms, OCR.
- **xlsx** — Excel spreadsheets: create, edit, formulas, charts, formatting, data analysis.
- **canvas-design** — Visual art creation (.png, .pdf) using design philosophy.
- **web-artifacts-builder** — Multi-component HTML artifacts (React, Tailwind, shadcn/ui).

### Client & Business Development
- **proposal-writer** — Full branded consulting proposals (SOWs, program proposals, renewals). Auto-researches client info.
- **exploration-proposal-generator** — Early-stage exploration proposals post-discovery call. Phased methodology, budget tables, terms.
- **client-research-brief** — Research dossiers on prospects/clients before proposals or calls.
- **client-status-report** — Comprehensive status reports pulling from Outlook, Teams, Fathom, SharePoint. 3-file memory system.
- **outreach-drafter** — Outreach emails/messages in Chris Jarvis voice. Sales, follow-ups, networking.
- **linkedin-prospect-enricher** — Cross-reference prospect lists against LinkedIn Connections CSV.
- **regional-campus-budget** — RWI Regional Campus Budget Forecaster (v5 Excel). Cost multipliers, registration fees, P&L.

### Meeting Intelligence
- **meeting-search** — Search/filter Fathom meeting history by person, company, topic, date.
- **meeting-recap** (rwi-team, rw-chris-personal, rw-team) — Concise meeting recaps from Fathom.
- **meeting-actions** (rwi-team, rw-chris-personal, rw-team) — Extract action items, todos, follow-ups from meetings.
- **meeting-transcript** (rwi-team, rw-chris-personal, rw-team) — Full transcript retrieval and search.
- **weekly-digest** — Comprehensive digest of all meetings from a time period.
- **transcript-to-action** — Process transcripts into structured action items by RW/RWI meeting type (13 types).
- **daily-call-prep** (rwi-team, rw-chris-personal, rw-team) — Prep for today's external meetings. Pulls calendar, Fathom, email, web research.

### Voice & Writing
- **chris-jarvis-voice-v2** — Chris Jarvis writing voice. No em dashes, no fabrication, systems-first thinking.
- **chris-jarvis-voice-v3** (rw-chris-personal) — Updated v3 with strict anti-fabrication and human cadence.
- **ai-syntax-avoidance** — Zero-tolerance detection/elimination of 4 AI writing patterns.

### File & Document Management
- **document-organizer** — Analyze, rename, tag documents based on content. 99.9% title extraction accuracy.
- **file-renamer** — Batch rename/tag files by content analysis and configurable naming conventions.
- **workspace-audit** — Audit working environment across all connected storage. Source-accountability principles.
- **source-accountability** — Rigorous source verification for multi-source research/audits.

### RWI Makerspace (rwi-team plugin only)
- **makerspace-context** — Deep context on RWI Makerspace operating model, lab types, programs.
- **decision-capture** — Log decisions about the Makerspace.
- **revenue-modeling** — Revenue architecture modeling for the Makerspace.
- **rw-knowledge-graph** — Scan RW docs, extract frameworks/models, build interactive mind map.

### Client Updates (rw-chris-personal, rw-team)
- **client-update** — Client status updates using program update template.

### Survey Design (rwi-team, rw-chris-personal, rw-team)
- **survey-design** — Behavioral science-informed survey design, bias reduction, cognitive bias audits.

### Meta / Session Management
- **skill-creator** — Create, modify, optimize skills. Run evals and benchmarks.
- **mcp-builder** — Guide for creating MCP servers (Python FastMCP or Node/TypeScript).
- **session-handoff** — Manage context across long conversations. 3-file external memory system.
- **dashboard-team-onboarding** — Onboard RW team members onto Meeting Intelligence Dashboard.
- **schedule** — Create scheduled tasks (on-demand or interval).
- **rw-brand-guidelines** — RW brand standards: Hero Navy (#0A3454), Hero Orange (#F05927), Roboto, logo rules.

### Slash Commands (rwi-team plugin)
- **/ms-status** — Quick Makerspace program status dashboard.
- **/ms-sync** — Deep scan Outlook/Fathom/transcripts for Makerspace activity.
- **/ms-brief** — Deep brief on any Makerspace program or topic.
- **/ms-update** — Capture decisions, update Makerspace brain file.

---

## 4. CLAUDE.md Custom Instructions (Summary)

All three remote plugins enforce consistent rules:

**Voice rules (strict, no exceptions):**
- No em dashes. Ever.
- No AI transitions: "Indeed," "Moreover," "Furthermore," "Additionally," "That being said," etc.
- No presentative constructions ("Here is [noun] that...")
- No fragment stacking (3+ fragments starting with same word)
- No metadiscursive directives ("pay attention," "notice," "sit with")
- No staccato parallel fragments
- Plain, direct, peer-to-peer prose. Short sentences, active verbs, concrete nouns.

**Questioning protocol:** One question at a time. Always provide selectable options. Never dump lists of open-ended questions.

**Chris-specific preferences (rw-chris-personal):**
- Complete full tasks in one pass
- Constructive pushback over affirmation
- "I'm still marinating" = explore together, don't present finished answers
- Fact-check everything: verify %, name sources, tiered credibility (Gold/Silver/Bronze/Caution)
- URLs: always web-search and verify live
- Neuroscience claims: specify which study/mechanism
- High tolerance for ambiguity and moral complexity

**File system references:**
- ~/Documents/ — iCloud-synced primary working layer
- Realized Worth Dropbox — shared company IP
- ~/Documents/Claude-AI-Config/ — skill registry, memory, preferences
- ~/Documents/Transcripts/ — Fathom transcripts
- ~/Documents/Active-Work/ — current project files
- ~/Documents/RW-Institute/ — RWI research/program files
- ~/Documents/Clients/[company]/ — client work

**RW Team (rw-team) session protocol:** At end of sessions where new facts are learned, run claude-md-management:revise-claude-md to update CLAUDE.md.

---

## 5. Workspace State

**Mounted folder:** `/sessions/focused-laughing-darwin/mnt/RWI Metrics/` (currently empty)
**Uploads folder:** `/sessions/focused-laughing-darwin/mnt/uploads/`
**Auto-memory:** No MEMORY.md found (fresh session)

---

## 6. Known Issues

| Issue | Severity | Action |
|-------|----------|--------|
| PubMed MCP returned server error | Low | Retry on next biomedical research request. May be transient. |
| Google Drive returned empty on test query | Info | Authenticated but no match for "test". Functional. |
| Notion not ping-tested | Info | Schema loaded successfully. Attempt live call on first Notion request. |
