---
name: write-email
description: Write a weekly Insights @ Spike email from start to finish. Use this skill whenever the user says /write-email, wants to write a Thursday email, wants to write an Insights @ Spike email, or wants to create content for the weekly email series. Guides through category selection, blog reading, angle suggestion, body writing, and subject/CTA finalization — all in one structured flow.
---

# Write Email — Insights @ Spike

You're writing a weekly email for the Insights @ Spike series. Follow this process exactly, one step at a time. Do not skip ahead.

## Step 1 — Ask for category

Read `category.md` to get the available categories. Ask the user which category they'd like to write from and list the options.

## Step 2 — Read all blogs in that category

Fetch and read every blog URL listed under the chosen category in `category.md`. Do all fetches in parallel.

## Step 3 — Filter used angles

Read `angles-log.md`. Note every angle already used under both the Drafts and Sent sections. These cannot be reused. The same blog or concept can still be used — but only with a different angle.

## Step 4 — Suggest ideas

From the remaining angles across the blogs you read, identify the ones with the strongest day-to-day on-call engineer angle — things engineers feel in the moment (getting paged for a system they don't own, not being able to commit to weekend plans, sleeping lighter on quiet on-call nights). Structural or management-level concepts perform worse.

Present 3–5 ideas. For each, state the blog it comes from, the specific angle, and why it's day-to-day relevant.

If no day-to-day angle exists across all blogs in the category, tell the user and ask them to choose a different category.

Wait for the user to pick one before continuing.

## Step 5 — Read rules.md

Read `rules.md` fully before writing a single word of the email. Pay close attention to:
- Format limits (body: 130–150 words, paragraphs: 1–2 sentences max)
- Hard no's (no em dashes, no colons in body, no banned words)
- Writing style (medium-length sentences — not fragments, not run-ons)
- Paragraph flow rule (every paragraph must connect to the previous one by picking up the last word, phrase, or idea)
- The reference email benchmark at the bottom of rules.md

## Step 6 — Write the email body

Follow the structure in `template.md`. Build the body around the concept the user picked.

Run every check in the self-check section of `rules.md` before sharing. Fix anything that fails before presenting the body.

## Step 7 — Share body with user

Present the body only. Wait for the user to approve or request changes. Iterate until the body is locked.

## Step 8 — Subject + preview + CTA

Once the body is locked, present both together in the same message:
- 5 subject-preview pairs
- 5 CTA options

Wait for the user to pick one subject-preview pair and one CTA before continuing.

## Step 9 — Full email

Present the complete email using the skeleton from `template.md`, including:
- Subject and preview at the top
- Fixed intro section
- Body
- CTA button with UTM link (swap the blog slug in the CTA URL)
- Fixed closing section
- Blog page link with UTM

UTM structure is defined in `template.md`.

## Step 10 — Update angles-log.md

Add a new entry under the **Drafts** section of `angles-log.md` with:
- Blog URL
- Angle used (one concise paragraph)
- Subject used
- Date (today's date)

When the user later confirms the email has been sent, move the entry from Drafts to Sent.
