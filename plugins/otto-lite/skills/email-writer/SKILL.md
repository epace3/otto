---
name: email-writer
description: Write one-off client emails for real estate agents in the agent's established voice. Use when the user says "write an email to [name] about [context]", "draft an email for…", "help me email my client about…", or pastes context and asks for an email. This skill writes a single email — not a sequence. Asks one clarifying question only if context is too thin, then writes. Output includes two subject line options and a warm, concise body with a clear CTA.
---

# Email Writer

## What this skill does

Writes **one-off client emails** in the agent's established voice — the single email the agent needs to send right now. Not a sequence. Not a campaign. Just the one message.

If context is thin, ask **one** clarifying question. Never more. Then write.

## When to use

Trigger on:

- **"Write an email to [name] about [context]"**
- "Draft an email for my [buyer / seller / lead]"
- "Help me email [name] about…"
- "I need to follow up with [name]"
- "Write the condition removal / price change / closing congrats / referral ask email"
- Any variant where the agent wants a single client email drafted

## Before writing

1. **Check the agent's voice.** Read `Otto Workspace/my_profile.md` if it exists, or pull from custom instructions. Load tone, sign-off, and signature block. If no voice is on file, default to **warm, direct, conversational**.

2. **Check whether you have enough context to write something useful.** You need, at minimum:
   - Who the email is to (name or at least role)
   - The purpose (what the agent wants this email to accomplish)
   - Any specific facts the email has to contain (price, date, address, decision, next step)

3. **If context is too thin, ask ONE clarifying question** — the single most important missing piece. Do not ask a list of questions. Do not send a form. One question, then write.

   Example: *"Quick check before I write — is this email going out before or after they've seen the place? That changes the tone."*

4. **If context is sufficient, write immediately.** Don't ask for permission, don't preview, don't outline. Write the email.

## Output format

Return exactly this structure, nothing more:

```
Subject line (option 1): [subject]
Subject line (option 2): [alternate subject]

[Email body]

[Agent sign-off from profile, e.g., "Best, Jessica"]
[Full signature block from profile if on file]
```

Optionally, after the signature, add **one line** as a PS — **only if it adds real value** (a warm personal note, a reminder about a follow-up, a question that re-opens the conversation). If a PS doesn't add anything, omit it entirely. Never force one.

## Rules for the body

- **Match the agent's voice** from profile or custom instructions.
- **Short.** If it can be 5 sentences, don't write 10. If it can be 3 paragraphs, don't write 5.
- **Clear next step.** Every email ends with either a clear CTA (what you want them to do) or an open question (what you need from them). Never end with "let me know if you have questions" or similar filler.
- **Subject lines matter.** Give two genuinely different options — one direct, one softer or more curious. Both under 50 characters when possible.

## Banned phrases (never use)

- "I hope this email finds you well"
- "Please don't hesitate to reach out"
- "Feel free to…"
- "Just wanted to touch base"
- "Circling back"
- "As per our discussion"
- "Kindly…"
- "At your earliest convenience"
- Any of the banned words from the humanizer skill (leverage, utilize, streamline, seamlessly, etc.)

## Pre-loaded email types

The skill should handle any of these cleanly without extra prompting:

1. **First contact / new lead intro** — warm but not pushy, acknowledge how they came in, one specific question to start a conversation.
2. **Post-showing follow-up** — mention one specific thing about the property they saw, ask what stood out, offer the next step.
3. **Condition removal update** — facts first, clear on what's been removed and what's next, reassuring but not gushing.
4. **Price reduction notification (to seller)** — honest, data-first, keeps the seller on your side, names the next milestone.
5. **Post-closing check-in** — warm, no ask (this one is just relationship), optionally plant a seed for future referrals without asking directly.
6. **Referral request** — direct, specific about who you're trying to help, easy to forward, no guilt-tripping.
7. **Condolence / sensitive situation** — short, human, no platitudes, no business mentioned at all unless they raise it.
8. **Negotiation response** — professional, firm, leaves room to keep talking.

## Example

**Agent:** *"Write an email to the Patels about the condition removal on 742 Maple — financing cleared today."*

**You respond:**

```
Subject line (option 1): Financing is cleared on 742 Maple
Subject line (option 2): Good news — one more condition down

Hi Raj and Priya,

Quick update on 742 Maple — the financing condition is officially removed. That leaves us with just the home inspection condition outstanding, and that report is expected by Friday.

Once inspection clears, we're firm. I'll reach out the moment I hear back from the inspector so we can talk through anything that comes up.

Nothing you need to do on your end right now — just wanted you to know where things stand.

Best,
Jessica

Jessica Chen
Executive Homes Realty
416-555-0100 · jessica@ehr.ca
www.jessicachen.ca
```
