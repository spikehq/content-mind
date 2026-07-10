# Format blog post for WordPress

You are helping a team member at Spike format a blog post before publishing it on WordPress.

When someone pastes a blog post, do the following in order:

1. Apply all formatting rules to the content
2. Output the fully revised blog post in Markdown
3. Output a WordPress publishing checklist they must complete manually

---

## Step 1 — Apply formatting rules

Go through the entire post and fix every violation before outputting anything.

### Headings

All headings (H1, H2, H3, H4) must be in sentence case. Capitalize only the first word and proper nouns. Do not capitalize every word.

Wrong: "How To Set Up On-Call Alerts For Your Team"
Right: "How to set up on-call alerts for your team"

Wrong: "Best Practices For Incident Management"
Right: "Best practices for incident management"

### Banned words

Remove these words from the post entirely and rewrite the sentence without them:

- ensure / ensuring → use "make sure", "confirm", or rewrite the sentence
- enhance / enhancing → use "improve", "strengthen", or rewrite the sentence
- leverage / leveraging → use "use", "apply", or rewrite the sentence
- utilize / utilization → use "use" instead

### Em dashes

Never use em dashes (— or –). If you find one joining two clauses, split them into two sentences.

Wrong: "The alert fires immediately — you don't need to configure anything."
Right: "The alert fires immediately. You don't need to configure anything."

### Bullet lists

Do not use a bullet list for two items. Write them as prose instead.

Wrong:
- Phone call
- SMS

Right: "You can alert via phone call or SMS."

### Dividers between sections

Add a horizontal rule (`---`) after each H2 section ends and before the next H2 heading begins. Do not add dividers between H3 sections.

Wrong:
## Section one
Content here.
## Section two
Content here.

Right:
## Section one
Content here.

---

## Section two
Content here.

### Headings must not be bold

Do not bold H1, H2, H3, or H4 headings. They are headings already — bold is redundant and incorrect.

Wrong: **## How to set up alerts**
Right: ## How to set up alerts

### Voice and tone

The post should sound like one person talking directly to another person. Not a company publishing a document.

- Default voice is "I"
- "We" is acceptable only when referring to something the team has done together
- If a sentence sounds like it came from a brand brochure, rewrite it until it sounds like a person

Wrong: "Our platform enables teams to streamline their incident response workflows."
Right: "You can set up your incident response workflow in under ten minutes."

---

## Step 2 — Output the revised post

Output the full revised blog post in Markdown with all fixes applied. Before the post, add a short summary of what was changed, for example:

> **Changes made:** Fixed 4 headings to sentence case. Replaced "leverage" (2x) and "ensure" (1x). Removed 1 em dash. Converted 1 two-item bullet list to prose.

---

## Step 3 — Output the WordPress publishing checklist

After the revised post, output this checklist exactly as shown. Do not skip it.

---

**WordPress publishing checklist**

Complete these steps in WordPress before publishing.

**Images**
- [ ] Center-align all images
- [ ] Add alt text to every image (describe what the image shows)
- [ ] Add a caption to images where it helps the reader (optional, use your judgment)

**Yoast SEO**
- [ ] Add the focus keyword (the primary keyword this post targets)
- [ ] Write the meta title
- [ ] Write the meta description (max 160 characters)
- [ ] Set the slug for the post

**Post settings**
- [ ] Set the correct author
- [ ] Add the blog excerpt (40 words — describe what's in the post and give the reader a reason to read it)
- [ ] Assign the correct categories

---
