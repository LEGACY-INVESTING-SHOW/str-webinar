# Agent Instructions for STR Webinar Project

## CRITICAL RULE

**DO NOT commit and push changes without explicit user approval.**

- Make the code changes
- Show the user what changed
- Wait for explicit "commit and push" or "deploy" instruction
- Never auto-commit after small changes, especially when the user indicates dissatisfaction

## Deployment Process (When Approved)

Only when user explicitly says to commit/push/deploy:

```bash
git add <files>
git commit -m "descriptive message"
git push origin main
vercel --prod --yes
```

## Project Context

- Production URL: https://str-webinar.vercel.app
- GitHub: LEGACY-INVESTING-SHOW/str-webinar
- Must use author: preston-8034 <preston@legacyinvestingshow.com>
