# Email Writing Rules

## Audience
- DevOps engineers, SREs, and on-call engineers
- On-call regularly, reading on mobile between meetings
- Examples should be about software in general, not incident management tools specifically

## Format limits
- Subject: under 50 characters
- Preview: under 90 characters
- Body: 130-150 words
- Paragraphs: 1-2 sentences max

## Hard no's
- No em dashes
- No colons anywhere in the body
- No banned words: ensure, enhance, leverage, utilize, for example, imagine, tends, most teams, many teams, some teams, chain

## Writing style
- Medium-length sentences. Not fragments, not run-ons
- Conversational. One person talking to another, not documentation
- Use contractions naturally: don't, it's, that's, they're
- Address the reader as "you" and "your"

## Paragraph flow rule
- Every paragraph must connect to the previous one
- Pick up the last word, phrase, or idea from the previous paragraph and open the next one with it as a consequence or direct answer
- If there's a gap between two paragraphs, rewrite one of them

## Subject and preview
- The subject should create curiosity, surprise, or recognition. Not summarize the email
- The preview should extend the subject's tension, not repeat it
- Together they should create an itch that only opening the email can scratch

## Content rules
- One idea per email. Not two, not three
- Open with a specific scenario, not a general statement about what teams do
- Include at least one concrete detail: a number, a real example, a before/after
- The insight must be non-obvious
- Use "incident" not "alert"

## Examples
- Must be something the reader's engineering team owns and can actually fix. If their team can't act on it, the example breaks down
- Should be about software in general, not about incident management tools specifically. The reader should map it to their own product

## Panic check
- Remove Spike's name from the sender field. Would this subject line make an engineer think something is actively broken right now? If yes, rewrite it

## Closing line before the CTA
- Must open a second loop or leave something unresolved that the CTA can scratch
- If removing it doesn't hurt the click, it's filler. Rewrite it

## CTA rules
- Must name exactly what's inside the guide. Never "Read the guide" or "Learn more"
- Good: "See the severity-priority matrix", "See all 6 on-call models"

## Guide bridge
- Start with "Our guide covers..." or "The guide walks through..."
- Never "We've written..." or "We've covered..."

## Concept selection rule
- When picking a concept from a blog post, prioritize angles, ideas, or scenarios that reflect the day-to-day life of an on-call engineer
- Concepts rooted in what engineers feel in the moment (getting paged for a system they don't own, planning personal time around shifts, context-switching fatigue) consistently perform better than structural or management-level concepts
- If no such day-to-day angle exists in the blog, flag it and ask for a different blog

## Reference email (use this as a benchmark)

Subject: Severity alone isn't enough to route incidents.
Preview: You need one more signal.

Body:
A webhook delivery failure for one customer is a low-severity incident. Your routing setup probably sends a Slack message and moves on.

But what if that customer is your largest enterprise account?

The severity (aka blast radius) is still low, but the priority is high. Just a Slack message isn't enough. You need an immediate phone call.

But if your routing only looks at severity, you don't get that phone call. By morning, the customer has been affected for hours, and that delay can cost you the account.

That's why you need to build priority into your routing setup alongside severity. It's not just about how many users are affected, but how fast you need to respond.

We built the severity-priority matrix exactly for that. Every combination maps to a defined response, so nothing slips through.

CTA: See the severity-priority matrix

---

## Self-check before finalizing
- Does the subject pass the panic check?
- Does every paragraph connect to the previous one?
- Is the body between 130-150 words?
- Are there any banned words or em dashes?
- Does the CTA name something specific?
- Does it sound like a human wrote it?
