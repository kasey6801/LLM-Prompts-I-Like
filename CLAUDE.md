# Claude Instructions: LLM Prompts I Like

This project captures and stores LLM prompts as markdown files, synced to GitHub.

## Prompt Capture Workflow

### Capture an existing prompt
When the user says any of: "capture this prompt", "save this prompt", "add this to the collection" — or similar phrasing:
1. Confirm: "Got it — I'll save this as a new prompt file. Here's what I'll capture: [repeat the prompt]"
2. Ask for a short title and any tags if not obvious from context
3. Write the file (see format below)
4. `git add`, `git commit -m "Add: <title>"`, `git push`

### Create a new prompt for a topic
When the user says "create a prompt for [topic]" or "write a prompt about [topic]":
1. Draft the prompt and present it to the user
2. Refine iteratively based on feedback
3. When the user approves ("looks good", "save it", "that's the one"), write the file
4. `git add`, `git commit -m "Add: <title>"`, `git push`

## File Format

**Path**: `/Users/kcharles/ClaudeDev/CC_LLM_Prompts_I_Like/YYYY-MM-DD_short-slug.md`

**Content**:
```markdown
---
title: "Prompt Title"
date: YYYY-MM-DD
tags: [tag1, tag2]
---

The prompt text goes here.
```

## Git Commands

```bash
cd /Users/kcharles/ClaudeDev/CC_LLM_Prompts_I_Like
git add <filename>
git commit -m "Add: <title>"
git push
```

## Notes
- Use today's date for the filename
- Keep slugs lowercase with hyphens
- Tags should be 1-3 descriptive words
- The GitHub remote is: `https://github.com/kasey6801/LLM-Prompts-I-Like`
