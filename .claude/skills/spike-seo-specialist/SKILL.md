---
name: spike-seo-specialist
description: "Spike.sh's vetted SEO/AEO playbook and evaluation framework, distilled from a full read-through of 152 tips from the seowins.io database against Spike's actual priorities (AI-citation visibility in ChatGPT/Perplexity/Google AI Overviews, legitimate tactics only, B2B SaaS audience — not classic-Google-rank-only or consumer/e-commerce tactics). Use this whenever writing or reviewing content for blog.spike.sh/docs.spike.sh/spike.sh (checks answer-first structure, featured-snippet formatting, GSC keyword-gap workflow, E-E-A-T signals, image/video AEO formatting), whenever asked to evaluate a new SEO/growth/backlink tactic or idea for Spike, or whenever asked what SEO/AEO work Spike should prioritize next. Do not use for customer-facing emails (see customer-email skill) or for SEO work unrelated to Spike.sh."
---

# Spike SEO/AEO Specialist

This skill packages the findings of a full review of the "SEO Wins (Lifetime)" Notion database (152 SEO/AI-SEO tips from seowins.io), each read in full and verdicted against Spike.sh's actual growth priorities. The verdicted tips are bundled alongside this skill:

```
references/
├── implement.md    — 89 tips ready to act on now, with concrete Spike.sh application notes
├── adapt.md        — good mechanics whose original context (affiliate/ad-driven) needs reframing
├── maybe.md        — plausible but lower-priority, or a stretch fit
└── skip.md         — rejected (wrong infrastructure, or conflicts with the no-manipulative-tactics rule)
```

**Read the relevant reference file(s) directly when you need tip-level detail or want to cite a specific tactic** — this SKILL.md summarizes the framework and the highest-leverage tactics, but the reference files are the source of truth for individual tips.

These are a snapshot from the original review (`spikehq` internal repo `seo-wins-playbook`, 2026-09-10). If that repo has since gained new verdicts, prefer pulling an updated copy over trusting this snapshot for anything time-sensitive.

## Spike's SEO/AEO priorities (apply to everything below)

- **AEO first** — the goal is visibility/citation in ChatGPT, Claude, Perplexity, and Google AI Overviews, not just classic Google rank. When a tactic could go either way, prefer the version that helps AI systems cite Spike.
- **Legitimate tactics only** — no manipulative or deceptive growth hacks. Explicitly rejected patterns (see `references/skip.md` for the full reasoning): paying for fake clicks/engagement to manipulate rankings ("pogo-sticking," click farms), ghost job ads to manufacture branded search volume, and undisclosed self-promotion disguised as independent community content (e.g. a "case study" post that buries a product link to "feel organic, not spam"). A tactic that *sounds* like paid promotion isn't automatically disqualified — running ads to drive traffic to genuinely citable content, which then earns organic links, was read carefully twice (#106, #134) and is legitimate. The line is disclosure and genuineness, not "involves money" or "involves a platform."
- **B2B SaaS audience** — SREs/DevOps/engineering managers evaluating incident-management/on-call tools, not consumer or e-commerce buyers. Tactics built around ad networks, affiliate marketplaces, or buying/selling websites don't transfer; tactics built around a UI/content *pattern* (a notification bar, an exit popup, image licensing) usually do once reframed — see `references/adapt.md` for the reframing pattern.
- **Properties in scope**: spike.sh (marketing site), blog.spike.sh (WordPress), docs.spike.sh, changelog (spikehq/changelog on GitHub).

## Job 1: Writing or reviewing content for blog.spike.sh / docs.spike.sh

Apply this checklist (tip numbers reference `references/implement.md`):

- **Answer-first** — give the direct answer/solution in the first 1-2 sentences; don't bury it after a preamble (#56).
- **Second-person, imperative voice** — "you can set up your escalation policy," not "an escalation policy should be set up" (#69).
- **"Because" opener** — open with a sentence stating a concrete reader benefit using "because" (#74).
- **PBC intro formula** for new posts — Preview, Benefits, Call to action (#13).
- **Short paragraphs** — ~3 lines / 25-30 words (#21).
- **Table of contents** on long-form posts, auto-generated from H2s (#20).
- **Featured-snippet formatting** for comparison/definition content: repeat the question at the start of the answer, answer in 40-60 words with key terms bolded, no filler (#30/#49/#89/#96/#105).
- **E-E-A-T signals** — author bio box with real credentials/links under every post (#72).
- **Image AEO** — full natural-language alt text, descriptive filenames, ImageObject schema (#27).
- **Video AEO** — publish full transcripts and captions alongside any embedded video, add VideoObject schema (#132).
- **Content upgrade** — for posts already getting traffic, consider a gated downloadable template/checklist matched to the topic (#91/#108/#149).
- **Freshness** — only bump a "best of"/year-specific title once GSC shows next-year query volume exceeding current-year volume, not on a calendar guess (#141/#148).

If the content is a **refresh of an existing page**, run the standing GSC content-gap workflow first: pull the page's Query data (last 3-6 months), find keywords with high impressions but low clicks or missing entirely, and work them into headings/paragraphs/FAQs/title tag (#9/#28/#40/#47/#55/#63/#68/#83/#85/#104/#114). This is the single most-repeated tactic in the whole review — treat it as one standing quarterly checklist, not a one-off.

## Job 2: Evaluating a new SEO/growth tactic or idea for Spike

When asked "should we do X" or "is this a good SEO/backlink tactic for Spike":

1. **Check whether it's already verdicted.** Read `references/implement.md`/`adapt.md`/`maybe.md`/`skip.md` — 152 tips have already been evaluated, and re-deriving a verdict from scratch risks inconsistency with the existing playbook.
2. **If it's new, apply the same three-part test** used for the full review:
   - Does it help (or at least not hurt) AEO/AI-citation visibility?
   - Is the mechanic genuine and disclosed, or does it rely on deception/fake signals/undisclosed self-promotion?
   - Does it fit a B2B SaaS motion, or does it require infrastructure Spike doesn't have (ad network, affiliate marketplace, buying/selling sites)?
3. **Consider "Adapt" before "Skip."** If the original framing is e-commerce/affiliate/ad-driven but the underlying UI/behavioral mechanic is sound, reframe it rather than rejecting it outright — see `references/adapt.md` for three worked examples (social-proof screenshots, related-content sidebars, CTA placement via heatmaps).
4. **Report a verdict** (Implement/Adapt/Maybe/Skip) with a concrete Spike.sh application, in the same style as existing entries: `### Title` / `- Category: ...` / 2-5 sentence application. If it looks durable and generalizable, offer to append it to the relevant reference file so the playbook stays current — don't silently let good analysis evaporate at the end of the conversation.

## AEO priority framework (the biggest lever — apply proactively, not just when asked)

- **Track what AI platforms actually cite** — mine GSC for long-tail question-intent queries already generating impressions, then use a citation-tracking tool (e.g. Peec) to see which domains AI models pull from for those prompts, broken out by source type. This was flagged as the single most directly relevant tactic in the whole database for Spike's AEO priority (#14).
- **Map the "fan-out."** LLM users rarely stop at one question. Seed a core topic query in ChatGPT/Perplexity, capture the follow-up questions they suggest, and build dedicated FAQ sections answering each — so Spike stays the cited source through the whole conversation thread, not just the first answer (#93).
- **Structure cornerstone content for AI citation**: answer the core question in the first 2-3 sentences, organize the rest around real "People Also Ask"-style questions, format with tables/bullets/FAQs, weave in named trust signals, and close with a concrete next step (#82).
- **Build genuine off-site mentions** — G2/Capterra/StackShare listings, podcast guest slots, Reddit/Quora answers, LinkedIn posts. LLMs weight mentions across the web as trust/citation signals, not just a brand's own site (#143/#152).

## When you're not sure

If a proposed tactic resembles something already rejected (fake engagement, undisclosed self-promotion, ghost content) but the person framing it insists it's "just marketing," read the exact rejected precedent in `references/skip.md` (#22, #70, #140) before agreeing to it — the review already drew that line carefully once.
