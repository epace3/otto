---
name: humanizer
description: Rewrite stiff, robotic, or AI-generated text so it sounds like a real human wrote it. Use whenever the user says "humanize this", "make this sound human", "rewrite this to sound like me", or pastes text that reads as AI-generated and asks for a cleanup. Preserves meaning — changes only tone, rhythm, and word choice. Matches the agent's established voice from their profile or custom instructions when available.
---

# Humanizer

## What this skill does

Takes any AI-generated, stiff, or robotic-sounding text and rewrites it so it sounds like a real human wrote it. Matches the agent's established voice (from their profile or custom instructions). Does NOT change meaning — only tone, rhythm, sentence length, and word choice.

## When to use

Trigger on any of the following:

- The user types **"Humanize this:"** followed by pasted text
- The user says **"make this sound human / less AI / more like me"**
- The user pastes a block of text and asks for it to be cleaned up, softened, or rewritten in their voice
- The user complains that something Otto or another assistant produced sounds "robotic," "corporate," "AI-generated," or "stiff"

## How to respond

1. **Identify the source text.** It's whatever the user pasted after the trigger phrase, or the block of text they're referring to in the previous message.

2. **Pull the agent's voice if it exists.** Check for a profile file (`Otto Workspace/my_profile.md` or similar), project custom instructions, or any prior-conversation context about how the agent writes. If you have a voice on file, match it. If not, default to: **warm, direct, conversational.**

3. **Rewrite using these rules.** Do not paraphrase — rewrite. The goal is the same meaning in words a real person would actually say.

### Banned words and phrases (never use in the rewrite)

- leverage, utilize, streamline, game-changer, cutting-edge, seamlessly, robust, comprehensive, foster, enhance, empower, holistic, synergy, unlock, elevate, unparalleled, revolutionize, transformative, innovative, best-in-class, world-class, next-level, paradigm
- "It's important to note that…"
- "It's worth mentioning that…"
- "In today's fast-paced world…"
- "At the end of the day…"
- "I hope this email finds you well"
- "Please don't hesitate to reach out"
- "Feel free to…"
- "Delve into…"
- "Navigate the complexities of…"

### Rewrite rules

- **Shorter sentences.** Break long, clause-stacked sentences into two or three shorter ones. Vary length — some short, some medium. Almost nothing long.
- **Cut hedging.** Remove "it's important to note," "it's worth mentioning," "one could argue," "generally speaking," and similar filler.
- **Real punctuation.** Use em dashes, periods, and question marks the way a person actually would. Don't overuse semicolons or parenthetical asides.
- **Contractions.** Use them. "It is" → "it's." "Do not" → "don't." "You will" → "you'll." Unless the voice on file is formal.
- **Concrete over abstract.** Replace vague nouns (solutions, strategies, approach, framework) with the specific thing being described.
- **Occasional imperfection.** Real writing has small asymmetries — a one-word sentence, a sentence that starts with "And" or "But," a trailing thought. Let those in.
- **Active voice.** Rewrite passive constructions unless passive actually fits.
- **Match the voice on file.** If the agent's profile says "warm and approachable," lean that way. If it says "luxury and elevated," keep a touch more polish but still cut the AI tells.

## Output format

**Output the rewritten version only.** No preface. No explanation. No "Here's the humanized version." No bullet list of changes you made. No commentary.

Just the rewrite — ready for the agent to copy, paste, and send.

If the source text is very long (more than ~500 words), you may break it into the same sections/paragraphs as the original, but still no commentary.

## Example

**Agent pastes:**

> Humanize this: In today's fast-paced real estate market, it is important to leverage cutting-edge marketing strategies to ensure your property stands out. Our comprehensive approach utilizes a seamless blend of digital and traditional channels to foster maximum buyer engagement and empower sellers to achieve optimal outcomes.

**You respond (rewrite only):**

> The market moves fast right now, so your listing has to work harder than it used to. Here's how I market yours: a mix of digital and traditional channels, each one chosen to put the property in front of the exact buyers most likely to act. That's how we get real interest — and real offers — instead of just clicks.
