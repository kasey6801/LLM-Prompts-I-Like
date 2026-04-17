# Claude Instructions: LLM Prompts I Like

This project captures and stores LLM prompts as markdown files, synced to GitHub.

## Slash Commands

| Command | Description |
|---|---|
| `/capture-prompt` | Interactively capture an existing prompt with full metadata |
| `/create-prompt [topic]` | Draft, refine, and save a new prompt for a given topic |

## Prompt File Format

**Filename**: `YYYY-MM-DD_short-slug_v<version>.md`

**Content**:
```markdown
---
title: "Prompt Title"
version: "1.0"
date: YYYY-MM-DD
tags: [tag1, tag2]
---

## Intended Use
What this prompt is designed to accomplish.

## Original Prompt
The raw, unmodified prompt the user started with.

## Tool Used
The tool or model used to generate/refine the modified prompt (e.g., Claude Sonnet 4.6).

## Modified Prompt
The final, refined version of the prompt.
```

## Fields

- **Title**: Short descriptive name
- **Version**: Semantic version (1.0, 1.1, 2.0). Increment minor for small edits, major for rewrites.
- **Date**: Date the prompt was saved (YYYY-MM-DD)
- **Tags**: 1–3 descriptive tags
- **Intended Use**: One sentence describing what the prompt accomplishes
- **Original Prompt**: The raw user input before any refinement
- **Tool Used**: Model or tool that helped generate/refine the modified prompt
- **Modified Prompt**: The final polished prompt to reuse

## Git Workflow

After writing any prompt file:
```bash
cd /Users/kcharles/ClaudeDev/CC_LLM_Prompts_I_Like
git add <filename>
git commit -m "Add: <title> v<version>"
git push
```

## GitHub Remote
`https://github.com/kasey6801/LLM-Prompts-I-Like`
