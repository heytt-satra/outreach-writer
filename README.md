# Outreach Writer

A prompt that writes high-converting cold emails, LinkedIn DMs, and connection notes.

Based on principles from $100M Offers and $100M Leads by Alex Hormozi.

The output sounds like a real person wrote it. No marketing fluff. No em dashes. Plain English. Specific details.

---

## What it writes

- **Cold emails** with a subject line, pain-first body, proof, and one CTA
- **LinkedIn connection notes** (300 character limit)
- **LinkedIn DMs** (sent 1-2 days after connection)
- **Job hunting outreach** that positions you broader than one role

## What makes it different

- Opens with an observation about the recipient, not a compliment
- Names the exact pain they live with before mentioning you once
- Uses specific names and numbers, not vague claims
- One ask at the end, lowest friction possible
- Never uses em dashes

---

## Use it on any platform

### ChatGPT / GPT-4
1. Open a new chat
2. Paste the contents of `prompt.md` as your first message, prefixed with `System instructions:`
3. Or use it as a Custom GPT system prompt in the GPT Builder

### Claude (claude.ai)
1. Open a new conversation
2. Paste the contents of `prompt.md` at the start of your message
3. Or add it as a custom instruction in Settings > Custom Instructions

### Cursor / Codex
1. Copy the contents of `prompt.md`
2. Paste it into your system prompt or `AGENTS.md` / `.cursorrules` file
3. Or pass it as `--system-prompt` in the CLI

### Claude Code (Claude CLI)
Use the native skill format in the `claude-code/` folder. See `platforms/claude.md` for setup.

---

## Quick start

Tell the AI:
- What you have built and what skills you have (with numbers if possible)
- Who you are writing to (name, company, role)
- One specific thing you noticed about them
- What format you need (cold email, DM, or connection note)

The AI will ask for anything missing before writing.

---

## Files

| File | Purpose |
|------|---------|
| `prompt.md` | Universal system prompt, works on any AI platform |
| `platforms/chatgpt.md` | ChatGPT and Custom GPT setup |
| `platforms/claude.md` | Claude.ai and Claude Code setup |
| `platforms/cursor.md` | Cursor and Codex setup |
| `claude-code/SKILL.md` | Native Claude Code skill |
