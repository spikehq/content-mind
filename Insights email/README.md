# Insights @ Spike — Weekly Email Series

Short, weekly emails on incident management sent every Thursday to on-call engineers and SREs.

## Prerequisites

- [Claude Code](https://claude.ai/code) installed

## Getting started

```bash
git clone <repo-url>
cd "Thursday email"
claude
```

Then type `/write-email` and follow the prompts.

## How it works

The `/write-email` skill guides you through the full process:

1. Pick a category
2. Claude reads all blogs in that category
3. Claude filters out already-used angles
4. Claude suggests ideas with a day-to-day on-call engineer angle
5. You pick one
6. Claude writes the body
7. You approve or iterate
8. Claude presents subject/preview pairs and CTA options
9. You pick one of each
10. Claude outputs the full email with UTM links

## Project files

| File | What it does |
|------|-------------|
| `rules.md` | Writing rules — format limits, style, banned words, and a reference email |
| `template.md` | Email structure and UTM link format |
| `process.md` | The 10-step writing process |
| `category.md` | Blog URLs organized by category |
| `angles-log.md` | All angles used across sent and draft emails |
| `.claude/agents/write-email.md` | The `/write-email` skill |

## Managing the angles log

`angles-log.md` tracks every angle used so the same idea is never sent twice.

- **Drafts** — finalized emails pending review/send. Angles here are reserved.
- **Sent** — emails that have been sent. Move entries from Drafts to Sent after sending.
- **Rejected drafts** — remove the entry from Drafts entirely.

## Adding a new category

Add a new section to `category.md`:

```markdown
## Category name

- https://spike.sh/blog/post-slug-1/
- https://spike.sh/blog/post-slug-2/
```

## Contributing

When adding new blog posts to a category, add the URL to `category.md` under the relevant section.
