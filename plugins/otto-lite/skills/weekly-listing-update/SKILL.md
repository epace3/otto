---
name: weekly-listing-update
description: Run a weekly listing update for a real estate agent — summarize showing activity, roll up agent feedback, flag market changes, prep price-reduction talking points if needed, and produce a ready-to-send seller update email. Use when the user says "weekly update — [address]", "run the weekly listing update", or provides a listing address with a week's worth of activity notes. Produces everything in one scannable document.
---

# Weekly Listing Update Workflow

## What this workflow does

Takes a week's worth of activity on an active listing and produces a structured update the agent can use two ways: (1) to prep their own head before talking to the seller, and (2) to send the seller a clean, honest update email.

Includes conditional price reduction prep if the feedback suggests price is the barrier.

## When to use

Trigger on:

- **"Weekly update — [address]"** + any showing notes, agent feedback, or open house notes pasted in
- "Run the weekly listing update for [address]"
- "Give me this week's listing update on [address]"
- Any variant where the agent is asking for a structured weekly review of an active listing

## Before you start — intake

You need the following. If anything is missing, ask for it in one batch before running Step 1:

1. **Property address** and **current list price**
2. **Showing activity this week** — how many showings, any agent feedback captured
3. **Open house notes** (if there was one)
4. **Any market changes** — new comparable listings, new solds, price changes nearby, rate news, anything moving the pricing conversation

Do not proceed until you have at least showing count + feedback (even if the feedback is "none"). The update only works if the data is real.

---

## Step 1 — Intake Confirmation

Repeat back what you have in a short scannable format so the agent can confirm nothing is wrong before you generate the update:

> **Confirming weekly update for 742 Maple Drive:**
>
> - **Current list price:** $1,449,000 (day 12 on market)
> - **Showings this week:** 6 private + 1 open house (14 groups through)
> - **Agent feedback:** 3 said price is too high for the updated comps, 2 said kitchen is a strength but the primary bedroom feels small, 1 said they're still deciding between this and 88 Oak
> - **Open house notes:** steady traffic, 2 signed-in as "just looking," 1 pre-approval in hand from a family with 2 kids
> - **Market changes:** new sold on the same block closed at $1,385K — comparable sq footage, no reno
>
> Everything accurate? I'll run the update.

Wait for confirmation.

---

## Step 2 — Showing Activity Summary

One short paragraph plus 2–3 bullets. Answer:

- **How many showings** and how that compares to a realistic benchmark for this price point / area / week-of-listing
- **Patterns in the feedback** — what buyers are responding to (the wins) and what they're pushing back on (the drags)
- **What the objections are really about** — not the surface complaint, the underlying read ("it's priced at the top of the range and the comps are softening" is the real story behind "too expensive")

Be direct. Do not sugar-coat. A seller who hears honest feedback once in week 2 is a seller who takes a price conversation well in week 4.

---

## Step 3 — Agent Feedback Rollup

**3 bullets max.** The themes, not the quotes. Each bullet names a theme and its implication.

Example:
- **Price sensitivity at this level** — 3 of 6 agents cited pricing vs. the most recent sold. Implication: the ceiling on this house is probably $50K below current list.
- **Primary bedroom perception** — 2 of 6 said the primary feels small relative to the price. Implication: a staging tweak might help, but it won't overcome #1.
- **Competition from 88 Oak** — one direct comparison. Implication: buyers shopping this price in this pocket have one real alternative right now and we need to out-position it.

Be blunt. The agent is going to use this to decide what to do next — they need the truth.

---

## Step 4 — Market Pulse

Any new comparable listings or sales this week that affect positioning. **One sentence** on what each one means for this listing. No more.

Example:
- **New sold: 56 Oak Drive at $1,385K.** Same sq footage, no reno — confirms the upper ceiling of the market is softening. Makes our $1,449K list look 4–5% high to buyers who know the comps.

If no market changes, say so in one line and move on. Don't pad this section.

---

## Step 5 — Price Reduction Prep (conditional)

**Only include this section if the combined evidence from Steps 2–4 suggests price is the barrier.** If it's not, write "Price reduction not indicated this week — feedback is about [the real thing, e.g., staging / exposure / timing]" and skip.

If price IS the barrier, produce talking points for the seller conversation in this order:

1. **Data first.** The 2–3 numbers the seller needs to hear. No opinions yet — just the facts (days on market, comparable sold, feedback patterns, showing count vs. benchmark).
2. **Emotion second.** Acknowledge what they're feeling — attachment to the number they set, frustration with the market, worry that reducing looks like weakness.
3. **Recommendation third.** A specific number or range to reduce to, and the *why* behind it (what that price opens up in terms of comparable buyer pools, search filter thresholds, psychological anchors).
4. **One script line** the agent can use to open the conversation — pulled from the `crucial-conversations` framework (acknowledge, mutual purpose, honest core message).

---

## Step 6 — Seller Update Email

**Ready to send, pending agent review.** Written to the seller from the agent.

Rules:

- **Warm, honest, specific to this week's activity** — not a template.
- **No sugar-coating.** If feedback is bad, say so.
- **No doom.** Bad feedback is not a crisis — it's data. Frame it that way.
- **Professional and clear.** Every email ends with a specific next step or a question the seller needs to answer.
- **Match the agent's voice** from their profile or custom instructions.
- **Never use banned phrases** — no "I hope this email finds you well," no "please don't hesitate," no "just wanted to circle back."

Include **two subject line options** at the top. Include the agent's sign-off and signature block from their profile.

**Present the email to the agent and ask them to review before sending.** Do not mark the workflow complete until the agent has seen the email and approved it (or sent edits).

---

## Final delivery

Return all 6 steps in **one clean scannable document** with section headers. The agent should be able to scroll the whole thing once and then walk into the seller conversation with nothing else in hand.

**If this workflow is running inside a plugin environment with file-saving capabilities:** save the weekly update document and the seller email as separate files in the property's folder (e.g., `742-maple-drive/weekly-updates/{date}/`) and return clickable `computer://` links so the agent can open each in the preview.

**Close with one line** on what the agent should do next — schedule the seller call, send the email, wait for one more showing, etc. Not a paragraph. One line.
