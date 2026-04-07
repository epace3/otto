---
name: weekly-priorities
description: Run a real estate agent's weekly priorities review — gap analysis against annual goal, time allocation recommendation, top 3 priorities for the week, prospecting recommendation, and the one thing they're avoiding. Use when the user says "run my weekly priorities", "what should I focus on this week", or triggers their Monday morning priority review. Designed to run every Monday and produce a clean scannable summary, not a wall of text.
---

# Weekly Priorities Workflow

## What this workflow does

Runs a real estate agent's weekly priorities review. Ideally triggered every Monday morning. Takes the agent's current goal data, pipeline, and calendar, and produces a **scannable weekly plan** that answers:

1. How far behind or ahead are they vs. their annual target?
2. How should they split their time this week?
3. What are the top 3 things that matter most?
4. Who should they be calling?
5. What are they avoiding that needs to be done?

Not a wall of text. Not a motivational speech. A clean, honest, useful plan.

## When to use

Trigger on:

- **"Run my weekly priorities"**
- **"It's Monday — run my priorities"**
- **"What should I focus on this week?"** (when invoked in EA mode)
- **"Weekly priorities"**
- Any variant where the agent is asking for a weekly planning session

This workflow is owned by the `executive-assistant` skill — the EA is the trigger, this workflow is the execution.

---

## Step 1 — Intake

Ask for (or confirm from memory if already on file):

1. **Annual deal goal and income target** — the number they're driving to this year
2. **Deals closed YTD** — how many are in the bank
3. **This week's specific focus** — any listing appointments, showings, closings, deals in conditions, buyer consults already scheduled
4. **Current challenges** — what's feeling hard, stuck, or heavy right now
5. **This week's calendar** — the agent can paste it in, or describe the shape of the week

If the agent already has a profile or goal data in memory from prior sessions, restate it and ask them to confirm or update. Don't make them re-enter the whole thing every Monday.

Do not proceed to Step 2 until you have at least the annual goal, YTD count, and some version of this week's shape.

---

## Step 2 — Gap Analysis

The honest number.

Calculate:
- **Deals needed per month** to hit the annual target
- **Current pace** (deals closed YTD ÷ months elapsed)
- **Gap** — are they ahead, behind, or on pace, and by how much

Write it as a short, direct paragraph. No cushioning. Example:

> You're 3 deals closed in Q1. Your goal was 20 for the year, which means you need 1.67 deals per month to stay on pace. You're currently running at 1.0 per month. You're not in crisis, but you're 2 deals behind where Q1 should have left you, and that gap compounds if Q2 looks the same. Q2 needs to be 6 deals minimum to get back on pace.

If they're ahead, say that clearly too. Don't over-inflate — just honest numbers. An agent who's told they're ahead when they're not ends the year short.

---

## Step 3 — Time Allocation Recommendation

Based on the gap + this week's calendar, how should they split their time?

Format as **percentages with context**. Percentages alone are useless.

Example:

> **This week's allocation:**
>
> - **45% prospecting** — you're behind pace, and prospecting is the only input that closes the gap. This isn't "if you have time," it's the top priority.
> - **30% active client service** — 3 showings + 1 closing + the Patel price conversation. Non-negotiable.
> - **15% follow-up** — the leads from last week's open house need calls before Wednesday or they go cold.
> - **10% admin and planning** — cap it at this. You tend to let admin swell when prospecting feels hard.

Be specific. Tie every percentage to something concrete from the intake.

---

## Step 4 — Top 3 Priorities

The 3 things that matter most this week. **Specific and actionable.**

Not: *"Do more prospecting."*
Not: *"Focus on pipeline."*

Yes: *"Call the 4 leads from last week's open house by Wednesday. They walked through, they signed in, and they haven't heard from you since. One of them is pre-approved."*

Each priority should answer: **what exactly, by when, and why it matters.** Three priorities. No more. If you can't name three, name two.

---

## Step 5 — Prospecting Recommendation

Based on their pipeline, their gap, and what's in season: **who should they call, what should they say, and why now?**

If they've mentioned specific leads, expired listings, or pipeline contacts in prior sessions or earlier in the conversation, reference them by name. If not, give them a specific category to work (e.g., "expireds from the last 30 days in your farm area — the ones that didn't re-list are actively disappointed in their last agent and open to a conversation right now").

One short paragraph. Specific enough that the agent can walk away and do it in the next 20 minutes.

---

## Step 6 — The One Thing They're Avoiding

The hardest section. Based on everything the agent has told you — the challenges, the calendar, the tone of their messages — **name the one thing that's probably sitting undone because they're avoiding it.**

Examples:
- The seller price conversation they've been dreading
- The difficult call to the client whose deal fell through
- The follow-up with the lead who went cold because they don't know what to say
- The contract amendment they haven't signed because it means admitting a mistake
- The numbers they haven't looked at in 3 weeks because they're behind pace

Be direct. **Not harsh — just honest.** One sentence naming it, one sentence on why it matters, one sentence on what to do about it (or which skill to delegate to — `crucial-conversations` for the hard talk, `email-writer` for the cold follow-up).

If you genuinely can't identify an avoidance pattern, say so. Don't invent one.

---

## Delivery format

**One clean, scannable summary.** Section headers for each of the 6 steps. Short paragraphs and bullets, not walls of text. The whole thing should be readable in under 90 seconds.

**If running inside a plugin environment with file-saving capabilities:** save the weekly priorities document as a dated file (e.g., `weekly-priorities/2026-04-07.md`) and return a clickable `computer://` link so the agent can open it in the preview and reference it throughout the week.

**Close with one line** the agent can take with them into the week — not a motivational quote, not advice, just the single sharpest thing from the review they should keep in their head. Example: *"The 4 open house leads are your week. Everything else is secondary."*

## Tone across the whole output

Direct, honest, warm, protective of their time. You sound like a chief of staff, not a coach. You don't mother them, you don't cheerlead, and you don't sugar-coat the gap. You also don't lecture — one honest sentence beats a paragraph.

If the agent is in a hole, say so. If they're crushing it, say that too. The agent trusts this review because it tells them the truth every Monday.
