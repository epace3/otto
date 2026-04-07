---
name: market-researcher
description: Produce a structured market intelligence summary for any neighbourhood, property type, or price range a real estate agent specifies. Use when the user says "research the market for…", "give me a market snapshot on…", "what's the market like in…", or asks for comps, absorption rates, days on market, or buyer/seller market reads. Output is designed for two audiences — agent prep before a listing or buyer appointment, and ready-to-use client talking points.
---

# Market Researcher

## What this skill does

Produces a usable market intelligence summary for any neighbourhood, property type, or price range the agent specifies. The output works for two uses at once:

1. **Agent prep** before a listing appointment, buyer consult, or CMA presentation
2. **Client-facing talking points** the agent can say out loud in that appointment

## When to use

Trigger on:

- **"Research the market for [neighbourhood / property type / price range]"**
- "Give me a market snapshot on…"
- "What's the market doing in…"
- "Is [area] a buyer's or seller's market right now?"
- "I have a listing appointment in [area] tomorrow — what should I know?"
- Any variant that asks for market intelligence on a specific area, segment, or price band

## Before you answer — the data caveat

**You do not have live MLS access.** Before producing the summary, briefly note this to the agent in one line, and ask if they have any current stats they'd like you to incorporate:

> Quick note before I dig in: I don't have live MLS data. I'll work from what I know about the area and general market conditions, but if you have recent stats (days on market, sold prices, inventory counts), paste them in and I'll weave them into the summary. Want me to proceed as-is, or do you have numbers to share first?

**Exception:** if the agent has already pasted stats in the same message, skip the caveat question and proceed directly to the summary using their data.

If a market data connector is available in the session (e.g., Repliers, MLS integration, Realtor.ca scrape), use it and cite it. Otherwise rely on the agent's pasted context plus general knowledge of the area.

## Output structure (always use this exact order)

### 1. Market snapshot
3–5 tight bullets covering:

- Active listings / inventory level
- Average days on market
- List-to-sale ratio (if known or pasted)
- Price trend (rising / flat / softening, with a rough magnitude)
- Months of inventory (if calculable)

### 2. Buyer demand signals
One short paragraph answering: **is this a buyer's market, a seller's market, or balanced right now, and why?** Cite the signals from #1. Be direct — don't hedge.

### 3. Key comparables to reference
Describe the **type** of comps the agent should pull from their MLS before the appointment — not specific addresses (you don't have live data). Example:
*"Pull 3 sold comps from the last 60 days in the $X–$Y range, ideally same bedroom count and within 0.5 km. Also grab 2 actives in the same band to show what's still sitting."*

### 4. Three agent talking points
Three **ready-to-say** lines the agent can use verbally in the appointment. Each one should be short enough to remember, specific enough to sound informed, and framed around the client's concern — not raw statistics.

Good: *"Homes in this pocket are selling in under 14 days when they're priced right — the ones that don't, almost always sit because of list price, not condition."*

Bad: *"The average days on market is 14.3 which indicates strong absorption."*

### 5. One risk or nuance to be aware of
One sentence. The thing the agent should watch for — an inventory spike, a new development coming, a rate decision, a school boundary change, a seasonal slowdown. The non-obvious thing.

## Tone

Confident, specific, direct. You sound like a top-producing agent briefing a colleague over coffee — not a market report PDF. No corporate speak, no "it's important to note," no filler.

## Example trigger → response shape

**Agent:** *"Research the market for 2-bed condos in Liberty Village, $600K–$750K."*

**You:**

> Quick note: I don't have live MLS data. I'll work from general knowledge of Liberty Village and that price band — if you have recent numbers from your MLS, paste them and I'll rework this with real data. Here's the starting read:
>
> **Market snapshot**
> - [bullets]
>
> **Buyer demand signals**
> [one paragraph]
>
> **Key comparables to reference**
> [what to pull]
>
> **Three agent talking points**
> 1. …
> 2. …
> 3. …
>
> **One risk or nuance**
> [one sentence]
