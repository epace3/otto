# Otto Lite — Install Guide

Three ways to install Otto Lite, depending on how you use Claude.

---

## Option 1 — Install in Claude Cowork (recommended)

Cowork is the Claude desktop app that runs plugins natively. This is the easiest install.

### Step 1 — Open Cowork

Open Claude Desktop and make sure you're in Cowork mode.

### Step 2 — Go to plugin settings

Click **Customize** (or the plugin icon in the top-right) → **Plugins** → **Browse plugins**.

### Step 3 — Add the Otto Lite marketplace

Click **Add marketplace** and paste the Otto Lite GitHub repo URL:

```
https://github.com/arslvn93/otto-lite
```

(Or drag the Otto Lite `.zip` file into the plugin install area.)

### Step 4 — Install

Find **Otto Lite** in the marketplace listing and click **Install**.

### Step 5 — Start a new chat

Open a new conversation and try any of the trigger phrases:

- *"Humanize this: [paste some stiff text]"*
- *"Research the market for downtown condos, $600K–$800K"*
- *"Write an email to my buyer about the post-showing follow-up"*
- *"Be my listing assistant — new listing at 742 Maple Drive"*
- *"Run my weekly priorities"*

Otto Lite will detect the trigger and load the right skill automatically.

---

## Option 2 — Install in Claude Code

If you use Claude Code (the terminal-based version of Claude), Otto Lite installs as a plugin.

### Step 1 — Clone or download the repo

```bash
git clone https://github.com/arslvn93/otto-lite
```

### Step 2 — Add the marketplace

From any directory where you use Claude Code, run:

```bash
claude plugins add ./otto-lite
```

### Step 3 — Install the plugin

```bash
claude plugins install otto-lite
```

### Step 4 — Trigger a skill

Start Claude Code in any project and use any of the trigger phrases above.

---

## Option 3 — Copy individual skills into a project

If you don't want to install the whole plugin, you can drop any individual skill into a single Claude project as custom instructions.

### Step 1 — Open the skill file

Pick one of the 10 skills from `plugins/otto-lite/skills/` and open its `SKILL.md` file.

### Step 2 — Open your Claude project

In Claude web or Desktop, go to your project → **Project Instructions**.

### Step 3 — Paste the skill

Copy the entire contents of the `SKILL.md` file (including the YAML frontmatter) and paste it into the project instructions.

### Step 4 — Use the trigger

Start a conversation in that project and use the trigger phrase from the skill file. Claude will follow the instructions.

**Note:** this approach only works for one skill at a time per project. For the full 10-skill experience, use Option 1 or Option 2.

---

## Troubleshooting

### "Otto Lite isn't responding to my trigger phrase"

1. Make sure you're in a fresh conversation (sometimes plugins load on the first message of a new chat)
2. Try the exact trigger phrase from the README (e.g., "Humanize this:" with the colon)
3. In Cowork, check **Customize → Plugins** and confirm Otto Lite is enabled

### "The plugin installed but I don't see any skills"

1. In Cowork, uninstall Otto Lite, quit the app completely, reopen, and reinstall
2. Confirm you're running a recent version of Claude Desktop

### "Can I use Otto Lite without installing it as a plugin?"

Yes — see Option 3 above. You can paste any individual `SKILL.md` file into a Claude project's instructions and use that one skill directly.

---

## Next steps

Once Otto Lite is installed, try running through all 10 skills in order — it takes about 20 minutes and gives you a full picture of what's possible.

If you want more — full listing/buyer/under-contract/post-close packages, automatic workspace organization, 30+ pre-loaded templates, and a profile that remembers you everywhere — upgrade to the **full Otto plugin**.

Questions? Email **arslan@salesgenius.co**.
