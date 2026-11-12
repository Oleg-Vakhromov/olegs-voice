# olegs-voice

A Claude Code skill that rewrites or drafts business prose (Slack messages, emails, memos, Jira/PR comments, reports, academic papers, news-style articles) so it reads like a specific person wrote it, not an AI assistant. It combines observed writing habits with William Zinsser's *On Writing Well*; where the two conflict, Zinsser wins.

## Install

Clone into your skills folder:

```
git clone https://github.com/Oleg-Vakhromov/olegs-voice ~/.claude/skills/olegs-voice
```

Or into a project: `.claude/skills/olegs-voice`.

## Layout

- `SKILL.md` – the skill: voice rules, tone by audience, anti-AI layer
- `references/zinsser.md` – clarity, simplicity, brevity, humanity
- `references/long_form.md` – news-style and reported articles
- `references/academic_papers.md` – academic writing
- `references/edit_pass.md` – the final edit pass
