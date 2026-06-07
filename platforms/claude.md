# Using Outreach Writer on Claude

## Option 1: Paste into any conversation

Copy the contents of `prompt.md` and paste it at the start of your message:

```
[paste prompt.md contents here]

Now help me write a cold email to...
```

## Option 2: Custom Instructions (claude.ai)

1. Go to claude.ai
2. Click your profile and go to Settings
3. Find "Custom Instructions" or "Default instructions"
4. Paste the contents of `prompt.md` there
5. It will be applied automatically to every new conversation

## Option 3: Claude Code Skill (for Claude Code users)

Use the native skill format in the `claude-code/` folder.

1. Copy the `claude-code/SKILL.md` file into your Claude Code skills directory
2. The skill will be available as `/outreach-writer` in Claude Code
3. Claude Code will automatically suggest it when you ask to write outreach

To find your skills directory, run `claude --skills-dir` or check `~/.claude/skills/`.
