# Using Outreach Writer in Cursor or with Codex

## Option 1: Add to .cursorrules

Create a `.cursorrules` file in your project root and paste the contents of `prompt.md` into it.

Cursor will apply these instructions automatically when you use AI features in that project.

## Option 2: Add to AGENTS.md

Create an `AGENTS.md` file in your project root with the contents of `prompt.md`.

This works with OpenAI Codex CLI and other agent frameworks that read AGENTS.md.

## Option 3: Use as a system prompt in the CLI

```bash
# OpenAI Codex CLI
codex --system-prompt "$(cat prompt.md)" "Write a cold email to..."

# Or with the OpenAI API directly
curl https://api.openai.com/v1/chat/completions \
  -H "Authorization: Bearer $OPENAI_API_KEY" \
  -d "{\"model\": \"gpt-4o\", \"messages\": [{\"role\": \"system\", \"content\": \"$(cat prompt.md)\"}, {\"role\": \"user\", \"content\": \"Write a cold email to...\"}]}"
```

## Option 4: Cursor Chat

Open Cursor Chat (Cmd+L or Ctrl+L), paste the prompt.md contents first, then describe what you need.
