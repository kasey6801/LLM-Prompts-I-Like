# LLM Prompts I Like

**LLM Prompts I Like** is a personal prompt library built inside Claude Code. It lets you save, version, and publish your favorite LLM prompts as structured Markdown files to a public GitHub repository. Two custom slash commands — `/capture-prompt` and `/create-prompt` — guide you through collecting metadata (intended use, original prompt, tool used, modified prompt, and version) before writing and auto-pushing each file to GitHub. The result is a searchable, version-controlled archive of prompts you can reuse across any AI tool.

## File Naming Convention

`YYYY-MM-DD_short-slug.md`

Example: `2026-04-16_creative-brainstorming.md`

## Prompt File Format

Each prompt file uses the following frontmatter:

```markdown
---
title: "Prompt Title"
date: YYYY-MM-DD
tags: [tag1, tag2]
---

Prompt content here...
```

## How Prompts Are Added

- **Capture mode**: Tell Claude "capture this prompt" after writing a prompt you want to save.
- **Create mode**: Ask Claude to "create a prompt for [topic]" and refine it interactively before saving.

After each save, the file is committed and pushed to this repository automatically.
