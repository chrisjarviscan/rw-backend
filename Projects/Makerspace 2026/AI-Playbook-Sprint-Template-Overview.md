# AI Playbook Sprint: Reusable Program Template

Extracted from the Wells Fargo Foundation pitch deck (March 2026). This document captures the methodology, structure, deliverables, and customizable elements so the sprint can be adapted for other companies (Danaher, etc.) without rebuilding from scratch.

---

## The Core Proposition

Most AI training programs are organized by topic: prompting in Week 1, quality in Week 2, metrics in Week 3. People absorb information, but they leave without a working system. The Playbook Sprint flips the organizing principle. Every week is organized around what each participant is building. AI topics still get covered, but they're woven into the build process rather than driving the sequence.

The end state: participants own a repeatable method for turning any workflow into an AI-powered system, independent of RWI after the sprint ends.

---

## The Central Concept: What Is a Playbook?

A playbook captures someone's expertise, decision-making process, quality standards, edge cases, and voice in a format that AI can reliably execute.

**What a playbook is not:**

- A prompt (single-shot prompts don't encode judgment or standards)
- A tip sheet (tips don't compound and can't be tested against real inputs)
- A template (templates are static; playbooks adapt to each input)

**What a playbook is:** A reusable system that works the way the person works, produces results at the standard they hold, and encodes their process, quality checks, edge cases, voice, and judgment into structured instructions AI can follow, test, and iterate on.

**When pitching:** the playbook concept does the heavy lifting of differentiating RWI's approach from every other AI training vendor. Define it early and define it against things the buyer's teams are probably already doing.

---

## Program Structure

| Parameter | Default Value | Customizable? |
|-----------|--------------|---------------|
| Duration | 7 weeks | Could compress to 5 or extend to 8 depending on session frequency |
| Cohorts | 2 | Scale to client need; more cohorts = more facilitation load |
| Participants per cohort | 25 | Upper bound for meaningful facilitation; 15-20 is easier |
| Live sessions | 14 total (2 per cohort x 7 weeks) | Could add async work or office hours |
| Delivery | Virtual, optional in-person capstone (Week 7) | Fully virtual or hybrid |
| Cohort composition | Mixed (client staff + external partners) | Can be single-org if no partner network exists |
| Funding model | Grant-funded via fiscal sponsor (Global Impact) | Direct contract, grant, or fee-for-service |

---

## Week-by-Week Methodology

### Week 1: Spot Your Workflow

**Driving question:** What recurring workflow eats your time, demands your judgment, and would benefit most from a reliable AI system?

**Session activities:**
- Teach what a playbook is and how it differs from a prompt or template
- Walk through 3 real playbook examples (customize examples to client's industry)
- Participants map their work against selection criteria: frequency, judgment required, time consumed, quality breakdowns

**AI topics woven in:** AI capabilities and limitations, prompting fundamentals, task-level vs. system-level AI use

**Deliverable:** Workflow candidate identified + one-paragraph scope statement

**Facilitation notes:** The selection criteria matter. A good playbook candidate is something the person does repeatedly, where they apply real judgment, and where quality inconsistency has visible consequences. Bad candidates: one-off tasks, purely creative work with no repeatable structure, tasks requiring zero judgment.

---

### Week 2: Map Your Process

**Driving question:** What decisions do you actually make inside this workflow? What standards live in your head but have never been written down?

**Session activities:**
- Externalize tacit expertise: decompose workflow into inputs, decisions, quality checks, edge cases
- Structured process-mapping exercise with facilitator feedback in real time
- Define what "good" looks like before building anything

**AI topics woven in:** Quality and accuracy standards, success criteria, authentic voice vs. generic AI output

**Deliverable:** Completed process map capturing all inputs, decision points, quality standards, failure modes

**Facilitation notes:** This is the hardest week for participants. Most people have never articulated their own process at this level of granularity. The facilitator's job is to ask the questions that surface the unstated rules ("What do you check before you hit send?" "When do you override the standard process?" "What would make you reject this output?").

---

### Week 3: Build Your First Draft

**Driving question:** Can you translate your process map into a format that AI can execute reliably?

**Session activities:**
- Translate process map into a working playbook: structured markdown, system instructions, reference docs
- Encode judgment, quality standards, and voice into reusable instructions
- [CLIENT-SPECIFIC] Bridge workflow introduced if client has a restricted AI environment (e.g., WF uses CoPilot; Danaher may have similar enterprise AI constraints)

**AI topics woven in:** System-level prompting, data handling, tool-agnostic principles across whatever AI tools the client uses

**Deliverable:** Working first draft tested on one real input from actual work

**Facilitation notes:** The bridge workflow is client-specific. For Wells Fargo, this was about safely moving between CoPilot and external AI tools. For Danaher or other companies, map their AI environment first: What tools are approved? What data can leave the corporate network? What anonymization is required? This becomes part of Week 3 content.

---

### Week 4: Test It and Break It

**Driving question:** Where does your playbook fail, and what does that failure teach you about your own process?

**Session activities:**
- Run playbook against 3 different real inputs, surfacing different failure modes
- Structured testing protocol: compare output to manual standard, log every deviation
- Classify failures: wrong output, generic output, missing context, tone mismatch, factual error

**AI topics woven in:** Quality control and accuracy, human-in-the-loop editing, correcting AI output, preserving voice

**Deliverable:** Failure log + revised Playbook v2 addressing critical failures

**Facilitation notes:** The failure classification taxonomy is reusable across clients. The five categories (wrong output, generic output, missing context, tone mismatch, factual error) cover most AI failure modes in professional workflows. Participants often discover gaps in their own process during this week, not just gaps in the playbook.

---

### Week 5: Make It Safe

**Driving question:** Your playbook works. But is it responsible? Is it safe to hand to a colleague?

**Session activities:**
- Pressure-test for governance, risk, and data safety
- Anonymization protocols, bias detection, communication risk management
- Create documentation so someone else can use the playbook without the builder present

**AI topics woven in:** Governance, data anonymization, bias awareness, compliance, AI ethics in the client's context

**Deliverable:** Governance layer added + handoff document for colleague use

**Facilitation notes:** This week's content must be customized to the client's compliance environment. Regulated industries (financial services, pharma/biotech like Danaher, healthcare) will need specific guidance on what data can and cannot flow through AI systems. Work with the client's compliance or legal team before the sprint starts to understand their boundaries, then build those constraints into this session.

---

### Week 6: Build #2 and Share

**Driving question:** Can you do it again, faster? Can you learn from what someone else built?

**Session activities:**
- Build a second playbook on a simpler workflow; map in 15 minutes, draft during the live session
- Speed difference between Playbook 1 and 2 is the proof the method works
- Cross-cohort sharing: participants from different roles/orgs present builds to each other

**AI topics woven in:** Workflow design at process level, metrics patterns across cohort, connecting playbooks into systems

**Deliverable:** Working Playbook #2 + documented cross-cohort insights

**Facilitation notes:** The speed compression between Playbook 1 (took 5 weeks) and Playbook 2 (built in a single session) is the single most persuasive proof point for the method. Track the time difference explicitly. For cross-cohort sharing, the value depends on cohort composition. Mixed cohorts (e.g., corporate staff + nonprofit partners, or R&D + commercial teams within Danaher) create richer cross-pollination than homogeneous groups.

---

### Week 7: Ship It and Roadmap

**Driving question:** What did you build, what does it save you, and where do you go from here?

**Session activities:**
- Finalize both playbooks; present to full cohort with time savings and honest boundaries
- Each presentation covers: what it does, what it replaced, the surprising thing learned, what it cannot do
- Identify next 3 playbook candidates; create 90-day implementation roadmap

**AI topics woven in:** Measuring impact, building the case for AI adoption, identifying where AI should not be used

**Deliverable:** 2 finalized playbooks + cohort presentation + 90-day roadmap

**Facilitation notes:** The presentation format ("what it does, what it replaced, the surprising thing, what it cannot do") is a strong structure. The "what it cannot do" element is especially important for executive stakeholders, because it signals that the program teaches responsible adoption, not hype. Optional: make Week 7 in-person as a capstone event. Inviting executive sponsors to the final presentations turns the capstone into an internal showcase.

---

## What Participants Leave With (Standard Across All Clients)

1. **Two working playbooks** built on actual work, tested against real inputs, with governance and documentation
2. **The playbooking method** applicable to any future workflow without RWI involvement
3. **90-day roadmap** with next three builds prioritized and sequenced
4. **[Client-specific] AI bridge workflow** if the client operates in a restricted AI environment
5. **Cross-sector/cross-functional perspective** from building alongside people in different roles

---

## Elements That Must Be Customized Per Client

| Element | What to customize | How to gather |
|---------|-------------------|---------------|
| Playbook examples (Week 1) | Use examples from the client's industry, not CSR/nonprofit examples | Pre-sprint discovery call; ask for 2-3 recurring workflows they'd want to see automated |
| AI tool environment (Week 3) | Map approved tools, data policies, and the bridge workflow | IT/compliance stakeholder interview before sprint design |
| Governance layer (Week 5) | Regulated industries need specific compliance guardrails | Legal/compliance review; build constraints into session materials |
| Cohort composition | Mixed (cross-functional, cross-org) vs. single-team | Depends on client's goals: operational empathy vs. team-specific depth |
| Cross-cohort sharing framing (Week 6) | The "who sees whose work" narrative changes by audience | Design the pairings intentionally based on where operational empathy has the most value |
| Funding/contracting model | Grant-funded, direct contract, internal L&D budget | Client procurement process |
| Closing slide / contact info | Entity, email, branding | RWI vs. RW branding; fiscal sponsor if grant-funded |

---

## The Sales Argument (Portable Across Clients)

The comparison framework from the WF deck translates to any buyer who has done or is considering topic-based AI training:

| Dimension | Topic-Based Training | Playbook Sprint |
|-----------|---------------------|-----------------|
| Organizing principle | AI topics (foundations, quality, metrics) | What each participant is building |
| Weekly deliverable | Learning + practice exercises | A tangible, testable artifact |
| End output | Knowledge + "at least one workflow" | 2 finalized playbooks + method + roadmap |
| Engagement model | Learn, then apply | Build, and learn through building |
| Reusability after sprint | Participants recall what they learned | Participants own a method they can repeat |
| Cross-cohort value | Shared experience | Shared builds with visible operational insight |

**The closer:** "The budget, cohort structure, timeline, and participation model remain identical. This is a curriculum redesign, not a scope change." (Only use this line when pitching against your own prior proposal or a competitor's topic-based program. If there's no incumbent to compare against, lead with the playbook concept directly.)

---

## Open Questions for Template Refinement

These came up during review and don't have answers in the current deck:

1. **Facilitation ratio:** How many facilitators per 25-person cohort during build sessions? The process-mapping and live-feedback components require more support than a lecture format.
2. **Skill-level spread:** How does the facilitation handle participants ranging from "never written a prompt" to "already using AI daily"? The deck is silent on differentiation.
3. **Completion rate:** Is the "2 finalized playbooks" outcome a guarantee or an aspiration? What percentage of participants actually finish both? This needs an honest answer before it becomes a standard deliverable across clients.
4. **Async work between sessions:** The deck describes live sessions but doesn't specify between-session expectations. How much time per week outside of sessions? Is there a Slack/Teams channel? Office hours?
5. **Measurement:** The deck mentions "time savings" in the final presentation but doesn't describe a measurement framework. For companies like Danaher that run on operational metrics, a structured before/after measurement approach would strengthen the offering.
