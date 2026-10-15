---
name: write-customer-story
description: "End-to-end workflow for writing a Spike customer story: collect and verify facts, draft the copy in chat for approval, add it to website_astro, prepare images, raise and merge the PR, verify it is live, update Airtable and the Sheet, and draft (never send) the customer update email. Use whenever a customer has agreed to a story and shared their thoughts, or when asked to write, revise, or publish a customer story. Not for the outreach emails themselves (use customer-email)."
---

# Writing a Customer Story

Stories live on spike.sh/customers. The model stories are **RevX, HitPath, Bluem, Stakin and SocialBee**. Read at least RevX, HitPath and Bluem in `src/data/customers.js` before drafting.

## 1. Gather inputs
- The customer's own words: their email or a call transcript. This is the only source for quotes.
- Their role and company facts. Read the **customer's own website (About page)** for how they describe themselves. LinkedIn is often stale: Perplex's LinkedIn said "internet marketing, 11-50" while their site said "digital agency, 80+ experts". If a site blocks fetching, open it in the browser.
- Headshot (square) and logo.

**Hard gate: do not start the story until every key input is in hand.** Do not draft copy, write a card quote, or touch the repo while anything below is missing. As soon as the skill starts, check this list, then send the user ONE message that lists what you already have and asks for everything still missing. Wait for their answer. Only then move to section 2.

Key inputs (all required):
1. The customer's verbatim words (email or transcript).
2. Person's name and exact role/title, and the company name.
3. Team size bracket (for example 11-50, 51-200).
4. Industry label.
5. Location.
6. "Relying on Spike since" date, or an explicit "skip it".
7. Headshot (square) and logo files, or an explicit instruction on where to source them.
8. Slug / company website URL.

Never guess a missing item, never fill it from LinkedIn or the site on your own, and never write "pending" placeholders and draft anyway. You may look up facts to suggest an answer (for example from the customer's site or Airtable), but present them as suggestions and wait for the user to confirm. If the user answers only some items, ask again for the rest.

## 2. Structure (tight, one-to-two sections)
1. `description`: the H1 and the card blurb. Spike-authored, "Spike helps X ..." style, one sentence.
2. `metaDescription`: 140-160 characters.
3. `quote`: the card quote (see section 4).
4. `author`: name, "Role, Company", avatar.
5. `stats`: Team size (brackets like 11-50, 51-200), Industry, Location. Add "Relying on Spike since" only if the date is confirmed.
6. `intro`: 2-3 sentences on what the company does, from their own site.
7. `body`: one intro paragraph naming the person and role, one general quote, then **one or two H2 sections**. Each section is a benefit-framed heading, a short paragraph, and one specific quote.

Nothing more: no extra sections on tenure, risk or support unless the story is thin without them.

## 3. Quote rules for the story body (non-negotiable)
- Every quote is **verbatim** from the customer's own words. Trim only filler, emojis and the template question. Never paraphrase inside quotation marks.
- If someone internal hands you "quotes", diff them against the customer's original first (the Stakin lesson).
- Keep the customer's own vocabulary inside their quotes, but not in our paragraphs. Avoid unclear words in our copy (for example "flows"). Clarity over matching their wording.

## 4. The card quote (shown on spike.sh/customers)
Rules, derived from an analysis of all 11 live cards (Neat, Sportskeeda, Virtually Human, RevX, Bluem and Thndr read best; Internset, Stakin and SocialBee read weakest):

1. **It carries a feeling or a change.** Calm, confidence, relief or ease, delight, or control. The H1 states what Spike does; the card says how it feels. Dependability phrased as trust also works when it reads well (Perplex: "Spike has become a central and reliable part of how we manage...").
2. **It comes from the customer, in their words.** Verbatim, trimmed only at a sentence boundary. Look for words they actually used ("happy", "easier", "confidence", "peace of mind", "sleep soundly"). Never add an emotion they didn't express.
3. **It stands alone.** Spike is named or clearly implied (no "It has made..." without context). First person ("we", "our") works best.
4. **It is not a feature or usage description** (Internset's styling options, Bluem's old "5 errors in a row"). Not a bare tenure or importance statement either, unless it carries a feeling.
5. **12 to 26 words, one or two sentences.** Longer overflows the card.
6. **A before/after contrast is the best** ("compared to OpsGenie", "much easier").
7. **If no verbatim line has the feeling, do not invent one.** Draft a candidate, get the customer's approval first (the Bluem route), and note the exception in the code comment.

## 5. Copy rules for our own text
- Short sentences. Break long ones up.
- No em dashes. No "deserves" or reward framing.
- The paragraph before a quote says what the quote says in plain words. Do not repeat the section heading.
- Do not claim anything the customer didn't say (for example, linking their certifications to Spike).
- Read the customer's point correctly before writing. Ask what the section is actually about (for example, "ease of connecting monitoring tools", not "what happens after an incident").

## 6. Draft in chat and get approval first
Show the whole story in chat: card, H1, stats, intro, every section, meta description. Say which parts are verbatim and which are ours. When the user wants alternatives for the title, a heading or a paragraph, give **5 options** and apply the one they pick. Do not raise a PR until they approve.

## 7. Images and PR
**Images**
- Avatar: square, 300x300 PNG, named `<first>-<last>.png`.
- Logo: PNG about 500px wide, trimmed of padding, named `<company>.png` (transparent background is fine on the light site).
- CDN link = `https://cdn.spike.sh/website/images/<same file name>`. Always `.png` in the name (the logo helper hardcodes it), even if the file is WebP underneath.
- Put the files in a folder (for example `~/Desktop/<company>-cdn-upload/`) and tell the user to hand them to whoever uploads to the CDN.
- Verify with `curl`: expect 200 and an image type. A **403 means missing**, same as a nonexistent path. Never silently fall back to another URL.
- A local asset (like Stakin's SVG logo) is allowed if the user provides one.

**Repo and PR (spikehq/website_astro)**
- Everything is one entry appended to the array in `src/data/customers.js`. No i18n or page edits are needed.
- `git fetch`, then branch off `origin/production` (the checkout may be on another branch).
- JavaScript only, no raw hex. Omit `image` (no hero photo) unless one is provided.
- Run `npm run build`. Confirm `/customers/<slug>/` is generated.
- Preview and screenshot the story page and the `/customers` card. Check the avatar and logo render.
- PR base `production`. The body lists what changed, the CDN links, and a test-plan checklist.
- The user shares the PR with Kaushik. **Merge only when the user says so** (merge commit). Later copy tweaks are small follow-up PRs.

## 8. When the story is live
Do all three, in this order:
1. **Verify the live page** (a deploy delay of a few minutes is normal). Confirm the H1, stats, card and images.
2. **Update the trackers.**
   - Airtable base "Customer Story Scoring", table Story Pipeline: set the customer's Story Collection Status to **Published** and put the live link in the note (with the PR numbers).
   - Mirror the Status to the same company's row on the Spike Customer Stories Tracker Sheet (match on Company).
   - If a connector is missing, tell the user exactly which fields to update.
3. **Draft the customer update email** with the **customer-email** skill and show it in chat. Reply-all in the existing thread, Kaushik stays CC'd, no greeting, link plus an invitation to suggest changes to the story. **Draft only: the user sends it, never Claude.**

## Quick checklist
- [ ] Facts from the customer's own site, not just LinkedIn
- [ ] Every quote verbatim, diffed against the original
- [ ] Card quote passes the 7 card rules
- [ ] One or two sections, short sentences, no em dashes
- [ ] Full draft approved in chat
- [ ] Images prepared, CDN URLs return 200
- [ ] `npm run build` passes, preview checked
- [ ] PR raised, merged only on the user's word
- [ ] Live page verified
- [ ] Airtable and the Sheet set to Published
- [ ] Update email drafted in chat for the user to send
