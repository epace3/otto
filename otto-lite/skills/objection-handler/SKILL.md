---
name: objection-handler
description: Turn any buyer or seller objection into a structured, confident response the agent can deliver in their own voice. Use when the user says "handle this objection", "how do I respond to…", "the client said…", "I'm getting pushback about…", or pastes an objection and asks for help. Gives the agent the logic and language to respond — not a word-for-word script to read robotically.
---

# Objection Handler

## What this skill does

Takes any buyer or seller objection and produces a structured, confident response **in the agent's tone**. The output is not a script to recite — it's the logic, the opener, the core message, a follow-up question, and the landmines to avoid. The agent uses this to sound natural, not rehearsed.

## When to use

Trigger on:

- **"Handle this objection: [paste]"**
- "How do I respond to a client who says…"
- "I'm getting pushback about [commission / price / timing / credentials]"
- "The seller told me [X] — what do I say?"
- "The buyer said [X] — help me answer"
- Any variant where the agent is asking how to respond to client resistance

## Response structure (always use this exact order)

Produce the response with these five sections, clearly labeled:

### 1. What's really behind this objection
One short paragraph. Name the **emotional driver**, not the surface complaint. Clients rarely object for the reason they say out loud — they object because of fear, past burn, perceived loss of control, or social pressure. Call that out.

Example: *"Your commission is too high" is almost never about the percentage. It's about the client feeling like they're losing control of a big financial decision and looking for something they can push back on. The commission is the lever they can see.*

### 2. How to open your response
The first 1–2 sentences the agent should say. **Acknowledge before you answer.** Never jump straight into rebuttal — it puts the client on the defensive. The opener should make them feel heard, then earn the right to respond.

### 3. The core response
3–5 sentences max. The actual substance. Clear logic, specific language, no filler. Written in a way the agent can say out loud and still sound like themselves — not a memorized pitch.

### 4. A question to ask after
One open-ended question the agent asks the moment they finish the core response. The goal is to keep the conversation moving, not to end it with a mic-drop. Good questions uncover what the client *actually* needs to hear next.

### 5. What NOT to say
2–3 bullets. The specific traps that make this objection worse — things many agents say that damage trust. Be direct.

## Rules

- **Never sound manipulative.** The goal is resolution and trust, not winning. If a response feels like a close-the-deal script, rewrite it.
- **Match the agent's voice** from their profile (`Otto Workspace/my_profile.md` or custom instructions) if available. Otherwise default to warm, direct, confident.
- **Don't hedge.** If the client is wrong about something, say so — kindly but clearly.
- **Don't pile on data.** Stats can support a point, but one specific number beats five vague ones.

## Common objections — treat these as pre-loaded examples

If the agent pastes any of the following, you should already have a strong default angle. Still produce the full 5-section structure.

1. **"Your commission is too high."** → Driver: loss of control over a big financial decision. Core: you're not paying for the transaction, you're paying for everything that happens *around* the transaction — the pricing, the marketing, the negotiation, the risk management. Reframe from cost to value-per-dollar.

2. **"We want to wait until spring."** → Driver: fear of making a wrong move, belief spring is safer. Core: spring isn't automatically better — it's more competitive. List early, less competition, motivated buyers who couldn't wait. Ask what specifically they think spring will solve for them.

3. **"We saw a similar house for less."** → Driver: anchoring on one data point, needing reassurance. Core: "similar" is doing a lot of work there. Walk them through what actually makes two houses comparable (condition, layout, lot, location pocket, finishes) vs. what looks similar on a map.

4. **"We don't need an agent — we can do it ourselves."** → Driver: feeling capable, wanting to save money, past bad experience with an agent. Core: acknowledge they probably *can* — then show them the 3 things that quietly cost FSBOs money (pricing, exposure, negotiation under pressure). No fear-mongering.

5. **"We want to think about it."** → Driver: not enough clarity or comfort to commit yet. Core: respect it, then find out what specifically they need more clarity on. "Think about it" is usually code for "I have one unanswered question and I can't name it yet."

6. **"Another agent offered to do it for less."** → Driver: testing, or genuinely seeing a cheaper option. Core: acknowledge it's a fair thing to compare, then ask what the other agent's plan is. The conversation should move from price to *plan*. Price without a plan is just a discount.

## Output

Return the 5-section structure in plain markdown with clear section headers. No preamble, no closing summary. The agent should be able to scan it once and walk into the conversation.
