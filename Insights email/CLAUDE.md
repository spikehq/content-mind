# Insights @ Spike — Email Project

This project is for writing the weekly **Insights @ Spike** email series — short, weekly emails on incident management sent every Thursday to on-call engineers and SREs.

## Project files

| File | Purpose |
|------|---------|
| `rules.md` | Writing rules, style guide, banned words, and a reference email benchmark |
| `template.md` | Email structure, fixed sections, and UTM link format |
| `process.md` | Step-by-step process for writing an email |
| `category.md` | Blog URLs organized by topic category |
| `angles-log.md` | All angles used in sent and draft emails — always check before suggesting ideas |
| `.claude/agents/write-email.md` | The `/write-email` skill |

## How to write an email

Use `/write-email`. It guides through the full process from category selection to final email.

## Non-negotiable rules

- Always read `angles-log.md` before suggesting ideas — skip any angle already used in Drafts or Sent. Same blog or concept can be reused, but the angle must be different.
- Always read `rules.md` fully before writing the body.
- Body must be 130–150 words. No exceptions.
- No em dashes anywhere. No colons in the body.
- Every paragraph must connect to the previous one — pick up the last word, phrase, or idea and open the next paragraph with it as a consequence or direct answer.
- Prioritize day-to-day on-call engineer angles. Structural or management-level concepts perform worse.
- Write medium-length sentences. Not fragments, not run-ons.
- Use "incident" not "alert".

## Angles log discipline

- Drafts and Sent angles are both off-limits when suggesting new ideas.
- When an email is approved and finalized, add it to Drafts in `angles-log.md`.
- When the user confirms it has been sent, move it to Sent.
- If a draft is rejected, remove it from the log.
