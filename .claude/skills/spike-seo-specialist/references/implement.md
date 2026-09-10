# Implement — SEO Wins tips ready to act on

89 tips, verdicted as directly applicable to Spike.sh. Grouped roughly by theme below (source database order preserved via tip #).

## AEO / AI citation tactics

### #14 — Get Citations Every Time From AI Platforms
- Category: AI SEO
- **The single most directly relevant tactic in the whole database for Spike's AEO priority.** Workflow: (1) mine GSC for long-tail "how to / what is / best X for / can you" queries already generating impressions — these reveal which prompts are triggering AI citations; (2) use an AI-citation tracking tool (e.g. Peec) to see exactly which domains/URLs AI models pull from for those prompts, broken out by source type (UGC/Social like Reddit, Editorial/Media, Corporate, Reference, Institutional); (3) identify which source type dominates for Spike's category and competitors, and concentrate effort there (e.g. if Reddit dominates on-call/incident-mgmt prompts, get genuinely active in relevant subreddits); (4) monitor citation/visibility changes over weeks-to-months since AI indexing lags behind classic SEO.
- **Recommend setting this up as an ongoing tracked program, not a one-off.**

### #3 — How To Rank #1 In Google AI Overviews
- Category: AI SEO
- Write a listicle blog post about the incident-management category ("Top Incident Management Tools in 2026") on blog.spike.sh and rank Spike #1 in it (framed honestly, not spammy). Republish the same listicle format as a LinkedIn Pulse article (list real competitors there too — the goal is the *format*, not self-promotion). Make a YouTube video covering the same list, and pursue ~10 guest posts on relevant SRE/DevOps sites using the same listicle structure. Doing all four in the same style trains AI Overviews to associate Spike with "best incident management tool" within 2-3 weeks.

### #32 — LinkedIn Pulse To Earn Citations In AI Overviews
- Category: AI SEO
- LinkedIn Pulse articles are disproportionately cited by AI Overviews/Gemini/ChatGPT even with minimal engagement, due to LinkedIn's domain trust and easy-to-parse format. AI Overviews pull from 3-6 sources across ~3.6 domains on average, over half outside the top-50 Google results — and articles under ~328 words (avg cited length 157 words) get cited most. Have Spike (company page and/or team members) publish short, structured LinkedIn Pulse posts on incident-management topics: prompt-aligned headline ("How to X," "What is Y," "A vs B"), TL;DR/short answer summary, 2-4 structured bullet points with subheads, a clear takeaway, and cited stats.
- **Low effort, high potential AEO payoff — should be a recurring content format, not a one-off.**

### #27 — How To Rank Images On AI Platforms
- Category: AI SEO
- AI platforms process images and text together for multimodal answers. Audit blog.spike.sh/docs.spike.sh images: write full natural-language alt text (not single keywords), use descriptive filenames (not IMG_123.jpg), add ImageObject schema markup, and treat cornerstone posts as "knowledge packages" (image + short video/transcript + schema) to maximize AI image-citation odds.

### #56 — Improve The User Experience Using A Way (answer-first structure)
- Category: AI SEO
- Give the direct answer/solution to the reader's problem in the first 1-2 sentences of any piece — don't bury it after a long preamble. This reduces bounce/pogo-sticking and specifically helps win AI Overviews/AI Mode citations and Featured Snippets, since both AI systems and searchers reward front-loaded, direct answers.
- **Recommend making "answer-first" a mandatory structural rule in Spike's content style guide** — high leverage for both classic SEO and AEO.

## Backlinks

### #4 — Get Backlink Directly From Google Official Website
- Category: Backlinks
- Build a small Chrome extension (e.g., a quick on-call status checker or incident dashboard widget), publish it to the Chrome Web Store, and set spike.sh as the Homepage URL in the store listing. Legitimate high-authority (chrome.google.com) backlink plus a discoverability channel.

### #6 — Earn Free Backlinks From OpenAI Or ChatGPT
- Category: AI SEO
- Build a public custom GPT (e.g. "Spike Incident Response Assistant" or "On-Call Runbook Helper") via ChatGPT Plus, then verify spike.sh as the owning website through OpenAI's Builder Profile (adds a TXT record to Spike's DNS). Earns a dofollow backlink from a DA-85 domain and puts Spike inside ChatGPT's GPT store — direct AEO exposure plus link equity.

### #12 — Unlimited Backlinks From Creators' YouTube Videos
- Category: Backlinks
- Search YouTube for videos on "incident management," "on-call best practices," "SRE," "postmortems," etc., sorted by view count. Pull the creator's email from their channel's About page and pitch Spike's relevant guide/doc as a helpful resource link for their video description. Nofollow but scalable, free, legitimate, and drives referral traffic.

### #25 — Get Free Backlinks Using Statistics Way
- Category: Backlinks
- Directly reinforces the existing statistics-driven backlink strategy. Publish original data/statistics content (e.g. a "State of On-Call 2026" survey or report) designed specifically to be a citable reference — other sites link to statistics pages as sources, and AI systems favor citable data pages too.

### #23 — Build Online Tools To Earn Free Backlinks
- Category: AI SEO
- Build and host free, niche-relevant tools on spike.sh — e.g. an on-call schedule generator, an SLA/uptime-percentage calculator, an incident-cost calculator, or an error-budget calculator. Free tools attract organic backlinks/shares because most site owners can't build their own. Can be scaffolded quickly with AI-generated HTML/CSS/JS.

### #54 — Free Backlinks From Real Bloggers, Not Marketers
- Category: Backlinks
- Passion bloggers (as opposed to professional SEOs) will often link for free if approached respectfully with a specific, genuine value proposition — unlike paid-link-expecting marketers. Process: create genuinely shareable content, engage authentically in relevant community/blog spaces (dev.to, Hashnode, personal SRE/DevOps blogs), then reach out via the blogger's own contact form/email explaining specifically why linking to Spike's content benefits their readers.

## GSC content-gap workflow (consolidate #9/#28/#40/#55/#63 into one standing process)

These five are the same underlying technique applied slightly differently — treat as **one recurring workflow**, not five separate tactics:

### #9 — Increase Website Visitors Without Increasing Rank
- For any blog.spike.sh/docs.spike.sh content older than 6 months, pull GSC Performance → Pages sorted by Impressions, then check that page's Queries for keywords with high impressions but low clicks (meaning it's already showing in search but not getting picked). Work those exact keywords into headings/paragraphs/FAQs at least twice; traffic typically lifts within 7-15 days.

### #28 — Google Search Console Under-served Keywords
- Export a page's GSC query data, find high-impression keywords with zero mentions in the existing content, and insert them into paragraphs/headings/FAQs.

### #40 — Hidden Questions Within Content To Increase Traffic
- In GSC Performance, filter Queries with the custom regex `^(who|what|where|when|why|how)` to find question-intent queries already generating impressions on existing pages, then add explicit Q&A content answering those exact questions. Especially valuable for FAQ schema and AI/voice-search visibility.

### #55 — Use Hidden Keywords To Grow Visitors
- Filter a page's 6-month query data by low clicks + high impressions, then work those exact keywords into paragraphs/title/meta description/images/FAQs.

### #63 — Use Long Tail Keywords To Increase Visitors
- Find long-tail keywords already getting impressions but underused in existing content, and work them in.

**Action:** build this into one standing "GSC content optimization" checklist run quarterly against the top 10-20 blog/docs pages, rather than treating as separate tasks.

## Content structure / on-page

### #8 — Double Website Traffic In Just A Few Minutes
- Category: Content Optimization
- In GSC, compare the last 3 months vs. the same period last year, sort Pages by Clicks Difference to find blog.spike.sh posts losing traffic, drill into that page's Queries (also sorted by Clicks Difference) to see which specific keywords dropped, then refresh the post with updated info, added paragraphs/headings/FAQs targeting those keywords. Run this quarterly on the top 10-20 posts.

### #13 — Improve Website Bounce Rate Up To 30% Instantly (PBC Formula)
- Category: Content Optimization
- Adopt the "PBC Formula" as a mandatory intro structure for every new blog.spike.sh post: **P**review (what the post covers), **B**enefits (what the reader gets from reading), **C**all to Action. Add to the content style guide.

### #21 — Shorter Paragraphs' Size To Boost Revenue
- Category: Content Optimization
- Adopt a style-guide rule of ~3 lines / 25-30 words per paragraph on blog.spike.sh for scannability and engagement.

### #20 — Table of Contents To Get Extra Visitors
- Category: On-Page SEO
- Add a Table of Contents (auto-generated from H2s) to long-form blog.spike.sh and docs.spike.sh articles. Google frequently surfaces TOC headings as jump-links directly in search results, increasing CTR.

### #30 — Optimize Content For Featured Snippets
- Category: Content Optimization
- For comparison-style articles, answer the core comparison in exactly 40-60 words with the main keywords bolded, no filler — wins Featured Snippet (position #0). Apply to Spike's comparison content (Spike vs PagerDuty, Spike vs OpsGenie, etc.).

### #49 — Get Featured Snippets With This Simple Trick
- Category: Content Optimization
- For "X vs Y" comparison content, open the key differentiating paragraph with the literal phrase "The main difference between..." — disproportionately picked up as Google's Featured Snippet for comparison queries. Apply as a standing convention across all Spike vs [Competitor] pages.

### #53 — Product Comparison Table To Increase Revenue
- Category: Content Optimization
- Build structured comparison tables for Spike vs PagerDuty/OpsGenie/Squadcast/Zenduty/Rootly (features, pricing tiers, integrations), with a "Start Free Trial"/"Book a Demo" CTA embedded directly in or beside the table. Strong for both on-page conversion and AI citation — comparison tables are exactly the structure AI Overviews like to extract from.

### #42 — Increase Post Rank With The Help Of Homepage
- Category: On-Page SEO
- Add a "recent/featured articles" section to spike.sh's homepage linking to key blog.spike.sh/changelog content. Google crawls homepages frequently, so a homepage link passes crawl priority and authority to linked content, speeding up indexing/ranking.

### #43 — Boost Post Rank With The Help Of Navigation Menu
- Category: On-Page SEO
- Same mechanism as #42 but via the site nav bar — a nav-menu link (e.g. a "Resources" or "Guides" item) pointing to Spike's cornerstone content/comparison pages/free tools passes crawl frequency and link equity sitewide. Cited example result: 0 to 858 visitors in 28 days.

### #47 — Optimize Title Using GSC Data To Boost Traffic
- Category: On-Page SEO
- In GSC, pull a specific page's Queries data (last 3 months), find the keyword with the highest impressions, and check whether it's present in the page's title tag — add it if missing. Run periodically against underperforming blog.spike.sh/docs.spike.sh pages.

### #51 — Update A Single Thing To Grow Traffic Easily
- Category: On-Page SEO
- Add a quarterly task to refresh the "last modified" date on evergreen blog.spike.sh cornerstone content — but pair it with an actual content update (from the #8/#9 workflow), not a date-only change, since stale-looking dates reduce clicks even on good content.

## Keyword research

### #17 — How Many Words Should A Post Contain
- Category: On-Page SEO
- Before writing any new blog.spike.sh or docs.spike.sh article, search the target keyword, open the top 10 ranking pages, and average their word counts to set a target length. Add as a pre-writing checklist step.

### #29 — Find Low Competitive Keywords In 1 Minute
- Category: Keyword Research
- Use the Keywords Everywhere extension with `site:quora.com "keyword"` (or similar UGC-site operators) to surface low-competition, achievable keywords for incident-management/on-call topics.

### #35 — Find Unlimited Keyword Ideas Using Asterisk
- Category: Keyword Research
- Type a target keyword into Google with an asterisk inserted between words (e.g. "on-call * software" or "incident * management") — Google's autocomplete fills the wildcard with related long-tail keyword ideas.

### #37 — Analyze Google's SERPs To Know If You Can Rank
- Category: Keyword Research
- Formalize as Spike's pre-publish keyword-viability checklist: (1) check search volume via Keywords Everywhere/Keyword Surfer; (2) check whether UGC sites (Reddit/Quora) rank on page 1 — a low-competition signal; (3) compare the lowest Domain Authority among ranking pages (via MozBar) against spike.sh's own DA; (4) assess whether ranking pages actually satisfy the search intent (gaps = opportunity). Run before committing writer time to any new topic.

### #57 — Find Unlimited Keywords Where Forums Are Ranking
- Category: Keyword Research
- If forums/UGC/low-DA sites rank on page 1 for a keyword, that signals low competition. Use `site:quora.com`, `site:reddit.com`, `site:imgur.com`, `site:discord.com`, `site:medium.com` + "keyword" search operators to find low-competition keywords tied to incident-management/on-call topics.

### #64 — High Volume But Easy Keywords To Write Content
- Category: Keyword Research
- In Ahrefs Webmaster Tools (free, import from GSC), go to Organic Keywords and filter Position 20-99, Volume ≥1000, KD 0-15. Surfaces keywords spike.sh/blog.spike.sh already ranks weakly for with real volume and low difficulty — a dedicated, well-optimized page targeting that keyword should be able to rank strongly.

### #33 — Outrank Big Websites Using Timing Technique
- Category: SEO
- For recurring "best of" content, publish next year's edition early (e.g. publish "Best On-Call Software 2027" in late 2026) to own the freshness/timing signal before competitors do — use the prior year's search-volume data as a proxy since the new-year keyword itself has no data yet. Pair with solid on-page SEO (3000+ words) and some backlink/social promotion.

### #45 — Find Content Ideas From Parallel Websites
- Category: SEO
- Take a top-performing post and swap one variable to generate an analogous piece — swap a competitor name in a comparison post, swap "on-call" for "incident response," swap an industry vertical in a use-case post. A systematic way to multiply content output from proven formats without starting from scratch each time.

### #59 — The Amount Of Content You Should Publish Per Month
- Category: SEO
- Use `site:competitor.com` combined with `-before:[end-of-month]` and `-after:[start-of-month]` Google search operators to count how many articles PagerDuty/OpsGenie/Squadcast/Rootly published/indexed in a given month, and use that to calibrate blog.spike.sh's own realistic monthly publishing cadence.

## Technical

### #24 — Actual Image Format To Increase Website Speed
- Category: Technical SEO
- Resize, compress, and convert images on spike.sh/blog.spike.sh/docs.spike.sh to WebP. Fold into the routine technical-SEO maintenance cadence (ties into the prior Ahrefs image-issue fixes already done).

## Batch 1 (rows 65-91)

### #65 — Write Trending Topics On Any Niche
- Category: AI SEO
- When a topic trends in tech/AI/SRE circles (a major cloud outage, a new AI model launch, a postmortem going viral), write a piece connecting it to incident management from Spike's angle — e.g. "What the [Major Outage] Teaches Us About Incident Response" or "How AI Coding Assistants Change On-Call Debugging." Make "newsjacking" a repeatable content-ideation habit: whenever something trends in DevOps/SRE/AI, ask how it applies to incident management and publish quickly on blog.spike.sh while interest is high.

### #67 — Find Viral Topic Ideas Using Reddit
- Category: SEO
- Periodically browse r/sre, r/devops, r/sysadmin (and similar) sorted by Top → This Year to surface trending pain points and discussions in the incident-management space, then turn the best ones into blog.spike.sh articles. Low-effort, recurring content-ideation source.

### #68 — Questions People Are Asking About Your Website
- Category: On-Page SEO
- Same mechanic as the existing GSC content-gap workflow, filtered to brand-specific queries. In GSC, filter Queries with a custom regex like `^(who|what|where|when|why|how).*(spike).*` to surface exactly what people search about Spike itself, and make sure clear answers exist on-site (About page, FAQ, docs). Fold into the existing quarterly GSC content-optimization checklist as a brand-query variant.

### #69 — Write In Second Person Narrative For AI Featured
- Category: Content Optimization
- Add a "second-person, imperative voice" rule to Spike's blog style guide: replace "users/teams can…" with "you can…," and use direct commands ("Set up your escalation policy" instead of "An escalation policy should be set up"). This conversational framing matches how people phrase voice/AI queries, aiding both readability and AEO citation odds.
- **Cheap, style-guide-level change with real AEO upside — bundle with the existing "answer-first" rule (#56).**

### #71 — Steal Competitors' Traffic By Using Headings
- Category: Content Optimization
- For target keywords (e.g. "incident management best practices"), pull H1–H3 headings from the top 3-5 ranking articles (including PagerDuty/OpsGenie/Atlassian content), identify subtopics Spike's article doesn't cover, write ~200 words per gap, republish, and request re-indexing via GSC. Legitimate content-gap analysis — fold into the standing content-refresh workflow alongside the GSC group.

### #72 — How To Improve Google E-E-A-T Easily
- Category: On-Page SEO
- Add an author bio box under every blog.spike.sh post (photo, name, credentials/experience, links to LinkedIn/Twitter). Ensure spike.sh's About page clearly answers "when/why was Spike started," "who's behind it," and "how can people contact you." Directly strengthens E-E-A-T signals both Google and AI systems use to weight trustworthiness.

### #74 — Because Word To Boost Your Website Engagement
- Category: AI SEO
- Add a style-guide rule: open articles with a sentence using "because" plus a concrete reader benefit (classic Cialdini persuasion research) — e.g. "This guide saves you hours during your next on-call rotation because it includes copy-paste escalation policy templates." A cheap, one-sentence tweak per post that increases time-on-page.

### #76 — Monitor Website To Prevent Rank Drop
- Category: Technical SEO
- Set up uptime monitoring on spike.sh/blog.spike.sh/docs.spike.sh — frequent downtime hurts both UX and ranking. Since Spike is an incident-management company, dogfooding this (using Spike itself to monitor and alert on its own uptime) doubles as an SEO safeguard and a credible case-study anecdote.
- **Worth a blog post: "we monitor our own marketing site with Spike."**

### #77 — Improve Information Gain Scores To Rank Higher
- Category: On-Page SEO
- For a target keyword, search Google with `filetype:pdf`, `filetype:ppt`, and `filetype:doc` appended to surface whitepapers/decks covering angles top-ranking blog content misses. Add those unique angles into Spike's own article to differentiate it and increase "information gain" — useful for comparison and best-practices pages.

### #78 — Find Unlimited Content Ideas For Topical Relevance
- Category: Keyword Research
- Use `site:domain.com "keyword"` (e.g. `site:pagerduty.com "incident management"`) against topical-authority competitors to see the full breadth of subtopics they've covered, then use that list to build out blog.spike.sh's topical depth in the incident-management category — supports topical authority for both classic SEO and AEO.

### #79 — Get Free Social Signals Or Shares And Backlinks
- Category: SEO
- When blog.spike.sh content positively mentions a specific company, tool, or practitioner, reach out afterward to let them know, without asking for anything. Many will share the post themselves or link to it — a relationship-based way to earn shares/backlinks. Fits Spike's customer-story and integration-partner content well.

### #80b — Increase CTR In Just 1 Minute Small Task
- Category: Content Optimization
- Add small icons/emoji next to row labels in Spike's comparison tables (Spike vs PagerDuty, vs OpsGenie, etc.) — Google sometimes surfaces these icons in rich results, making the listing stand out and lifting CTR. Pairs directly with the existing comparison-table tactic (#53).

### #82 — Content Writing Structure To Get Brand Mentions
- Category: AI SEO
- Adopt a five-part structure for cornerstone content aimed at AI citation: (1) answer the core question in the first 2-3 sentences; (2) structure the rest around real "People Also Ask"-style questions; (3) format with tables/bulleted lists/FAQs (AI Overviews prefer scannable formats); (4) weave in trust signals (named expertise, concrete numbers); (5) close with a concrete next step (calculator, template, "which plan fits you" guide).
- **One of the most directly actionable AEO frameworks in this batch — recommend formalizing as a checklist alongside #14 and #56.**

### #83 — Boost Traffic Using Under-served Headings
- Category: On-Page SEO
- Same mechanic as the existing GSC content-gap workflow (#9/#28/#40/#55/#63), applied specifically to headings: export GSC query data, find missing high-impression keywords, and work them into H2/H3s rather than only body copy. Fold into the same standing quarterly checklist.

### #85 — Boost Traffic Using Under-served Paragraphs
- Category: Content Optimization
- Identical technique to #83, applied to paragraph copy instead of headings. No separate workflow needed — it's the same standing GSC content-optimization checklist already covering #9/#28/#40/#55/#63/#83.

### #87 — Find Top Talented Writers For Your Website
- Category: SEO
- To source technical writers for blog.spike.sh, search incident-management/SRE keywords on Google, open top-ranking posts, and check bylines of well-written articles. If the author isn't in-house, find them on LinkedIn/Twitter and ask about freelance rates/availability. A repeatable way to build a bench of qualified SRE/DevOps freelance writers.

### #88 — How To Find Semantically Related Keywords
- Category: Keyword Research
- Before writing a new blog.spike.sh/docs.spike.sh article, run the target keyword through Semrush's free SEO Content Template tool to pull semantically related terms from top-ranking pages and work relevant ones into the draft. Add as a step in the existing pre-writing keyword-viability checklist (alongside #17/#37).

### #89 — Win Featured Snippets Within 15 Minutes
- Category: Content Optimization
- Reinforces the existing featured-snippet tactics (#30, #49): before writing a comparison/definition answer, open the current featured snippet for that query, note its exact word count (usually 40-50), format, and position (often under an FAQ H3), then match that structure exactly, repeating the question at the start of the answer. A sharper checklist for #30/#49, not a new workflow.

### #91 — Collect Visitors' Emails By Upgrading Content
- Category: SEO
- For blog.spike.sh posts that already rank and get meaningful traffic, add a content upgrade matched to the topic — e.g. a downloadable "On-Call Rotation Template," "Incident Postmortem Template," or "Escalation Policy Checklist" gated behind email signup. A standard, legitimate B2B lead-gen tactic and natural extension of existing content investment.

## Batch 2 (rows 92-124)

### #92 — Grow Visitors Using The Mother Technique
- Category: Technical SEO
- Content consolidation via 301 redirects: identify blog.spike.sh/docs.spike.sh pages that target the same or highly overlapping keyword phrases (keyword cannibalization), designate the most comprehensive one as the "Mother Content," 301-redirect all thinner, closely-related pages into it, then expand the surviving page with any unique information from the redirected pages. Prevents Spike's own content from competing against itself in search and AI Overviews, and consolidates link equity/AI-citation signals onto a single stronger page.

### #93 — Get Visibility For AI Follow-up Questions or Queries
- Category: AI SEO
- LLM users rarely stop at one question — they ask follow-ups, go deeper, and rephrase ("fan-out"). For core Spike topics (e.g. "what is an escalation policy"), seed that query in ChatGPT/Perplexity, capture the follow-up questions they suggest (plus "People Also Ask" results), then build short, dedicated sections or FAQ entries on blog.spike.sh/docs.spike.sh answering each follow-up so Spike stays the cited source through the whole conversation thread, not just the first answer.
- **Directly reinforces Spike's AEO priority — recommend pairing with the existing #14 AI-citation-tracking program and #82 cornerstone-content framework.**

### #95 — Find Posts That Contain Older Years Using An Operator
- Category: Technical SEO
- Use a Google search operator (e.g. `site:blog.spike.sh "2023"`) to find published posts still referencing outdated years, then update them to the current year alongside a real content refresh. A lightweight addition to the existing quarterly content-refresh workflow (#8/#51) — stale year mentions quietly suppress CTR even when the underlying advice is still accurate.

### #96 — Get A 100% Chance Of Winning Featured Snippet
- Category: Content Optimization
- When answering a question in FAQ/comparison content, literally repeat the question at the start of the answer paragraph (e.g. "What is an escalation policy? An escalation policy is..."). Reinforces the existing snippet tactics (#30/#49/#89) — fold in as a standing formatting rule rather than a separate task.

### #100 — Find Anchor Texts For Backlinks Using ChatGPT
- Category: AI SEO
- Use a ChatGPT prompt ("Generate a list of NLP-friendly anchor texts for the article '[title]', clear/specific/relevant/concise, 3-7 words, avoid generic phrases like 'click here'") whenever interlinking blog.spike.sh/docs.spike.sh articles or reaching out for guest-post backlinks, instead of defaulting to generic anchor text.

### #101 — Find Unique Topic Ideas From Reddit Goldmine
- Category: SEO
- Search `site:reddit.com "[competitor]" "alternative"` (or "any website") to surface Reddit threads where people are actively asking for alternatives to PagerDuty/OpsGenie/Squadcast/etc. — a goldmine for both content ideas (address the exact pain points/objections raised) and light-touch community engagement. Same spirit as the existing #67 Reddit-browsing tactic but targeted at direct competitor-alternative intent.

### #102 — Generate Google Search Console RegEx With ChatGPT
- Category: AI SEO
- Use ChatGPT to write the custom regex filters for GSC's Queries tab instead of hand-crafting them — speeds up the existing GSC content-gap workflow (#9/#28/#40/#55/#63/#68/#83/#85) whenever a new pattern (question-intent, brand-query, "pdf", synonym, etc.) needs to be isolated.

### #104 — Use Synonyms Keywords From GSC To Increase Traffic
- Category: Keyword Research
- For each cornerstone blog.spike.sh/docs.spike.sh page, take its top GSC keyword, Google "[keyword] + synonyms" to pull Google's own synonym list, then check GSC to see if any synonym is already generating impressions for that page and work it into the copy. Another variant to fold into the standing GSC content-optimization checklist.

### #105 — Featured Snippets By Looking At Qualified Sites
- Category: On-Page SEO
- For a query where a competitor currently holds the featured snippet, append `-domain.com` (e.g. `-pagerduty.com`) to the search to see which page Google would promote next — revealing the format/structure Google considers "next in line" and giving a concrete template to match or beat. Sharpens the existing snippet checklist (#30/#49/#89/#96).

### #106 — Unlimited Backlinks Using Google Advertisements
- Category: Backlinks
- **Read in full under extra scrutiny — verdict is Implement, not Skip.** The actual mechanic (documented via an Ahrefs ad-spend experiment) is not a paid-link scheme: publish genuinely citable case-study/statistics content, then run a legitimate Google Search Ads campaign driving traffic to it. The ad spend buys visibility with journalists/bloggers who then link to the content organically because it's genuinely useful — no link is purchased or inserted directly. Apply as a paid-amplification layer on top of Spike's existing statistics-backlink strategy (#25): run a modest Search Ads campaign pointing at a "State of On-Call/Incident Management" stats page to get it in front of people likely to cite it.

### #107 — Collect Autosuggest Keywords Using Google Gemini
- Category: AI SEO
- Since Gemini can access live search, ask it directly for "all Google autosuggest keywords for '[topic]'" to pull autosuggest-style keyword ideas without a third-party tool. Add as a step in the existing pre-writing keyword-research checklist alongside #35 (asterisk technique) and #88 (Semrush).

### #108 — Turn Exit Visitors Into Leads Using A Simple Hack
- Category: On-Page SEO
- Add an exit-intent popup (triggers when the cursor moves toward closing/leaving the tab) on blog.spike.sh offering a short, relevant interactive lead magnet — e.g. a 5-question "on-call maturity" or "alert-fatigue" quiz that emails the visitor a personalized action plan. Standard, legitimate B2B lead-capture pattern that complements the existing content-upgrade tactic (#91).

### #109 — Understand Your Audience's Language From Memes
- Category: SEO
- Search "[audience] + memes" (e.g. "SRE memes," "on-call memes," "DevOps memes") to see how the target audience jokes about their own pain points (2am pages, alert fatigue, escalation chaos) — a fast, low-effort way to mine authentic language/tone for headlines and topic ideas that will resonate more than generic SEO phrasing.

### #114 — Boost Traffic Using Under-served FAQs
- Category: Content Optimization
- Same GSC content-gap mechanic as the existing standing workflow (#9/#28/#40/#55/#63/#68/#83/#85), applied specifically to FAQ blocks: export a page's query data, find high-impression keywords missing from its FAQ section, and add them as new Q&A entries. No new process — just another variant for the same quarterly checklist.

### #115 — Make Your Website Posts Go Viral On Social Media
- Category: SEO
- Follow relevant industry figures/accounts (major cloud providers, well-known SREs, competitor product accounts) for real-time announcements or outage news, quickly tie the story to an existing or new Spike piece with a strong caption and link, post to the platform where Spike's audience is most active, and optionally back it with a small paid boost for reach. Same newsjacking spirit as the existing #65 tactic — fold in the "paid boost when timing matters" step.

### #116 — Find Out If Your Writer Is Feeding Duplicate Content
- Category: SEO
- Before publishing freelance-written blog.spike.sh content, copy a single distinctive sentence (5+ words) from the draft and Google-search it in quotes — if it surfaces on another site, the writer likely copied/spun existing content. A free, zero-tool plagiarism check to add as a pre-publish QA step alongside the existing freelance-writer sourcing workflow (#87).

### #117 — Boost Pageviews Through Keyboard Navigation
- Category: Technical SEO
- Add simple prev/next navigation (with a visible "use < > keys to navigate" hint) at the end of blog.spike.sh/docs.spike.sh articles so readers can move to related content with one click or keypress, reducing the friction to viewing a second page. Complements the existing related-content sidebar tactic (#5, Adapt).

### #121 — Increase Website Traffic Through PDF Keywords
- Category: Technical SEO
- In GSC, filter Queries containing "pdf" to see which existing blog.spike.sh/docs.spike.sh topics people specifically want a downloadable version of, then add a matching PDF (e.g. "On-Call Rotation Template," "Incident Postmortem Checklist") — directly extends the existing content-upgrade tactic (#91) with a demand-validation step instead of guessing which templates to build first.

### #124 — Protect WP Config File From Attack And Save CPU Usage
- Category: Technical SEO
- Add a Cloudflare WAF rule blocking repeated/brute-force requests targeting `wp-config.php` on blog.spike.sh (WordPress). Reduces server load from attack traffic and the resulting downtime/latency risk, which ties directly into the existing uptime-monitoring rationale (#76) — downtime and slow response times both hurt rankings.

## Batch 3 (rows 125-152)

### #125 — Get Free Backlinks With The Help Of Events
- Category: Backlinks
- Organize a virtual or physical SRE/on-call-focused event (an "Incident Response Summit" webinar series, or a small meetup at an existing DevOps conference) under the Spike brand. Trade press and community outlets (The New Stack, DevOps.com, SRE newsletters) covering the event will link back to spike.sh for free — the same mechanic that got Pubcon a link from Search Engine Journal for organizing an SEO conference.

### #129 — Actual Feature Image Size That Can Fit Everywhere
- Category: On-Page SEO
- Standardize blog.spike.sh's featured/OG image size at 1280×720 so images render fully (not cropped) when shared on Facebook, X, LinkedIn, WhatsApp, and Google Discover. A one-line addition to the CMS template/style guide.

### #132 — How To Rank Videos On AI Platforms
- Category: AI SEO
- For Spike's video content (webinar recordings, product demos, onboarding walkthroughs), publish full transcripts alongside the embed on blog.spike.sh/docs.spike.sh, add closed captions, add VideoObject schema, and repurpose clips into short-form videos with text overlays. AI platforms increasingly parse transcripts as indexable text, making video citable the way blog text already is.
- **Extends the existing AEO framework (#14/#82/#93) into video/multimodal content.**

### #133 — Underserved Quora Questions To Get Sure Visitors
- Category: SEO
- Use `site:quora.com "on-call" "1 answer" "k views"` (swap in incident-management/SRE keywords) to find high-view, low-answer-count Quora questions, then post a genuinely helpful answer referencing Spike where relevant. Turns the existing Quora/UGC keyword-research tactics (#29/#57) from "find keywords" into "go answer them."

### #134 — Generate Free Backlinks Using The PPC Ads
- Category: Backlinks
- **Read in full under extra scrutiny — verdict is Implement, not Skip, identical resolution to #106.** Publish a genuinely citable statistics page (e.g. "State of On-Call 2026"), then run a targeted Search Ads campaign against the exact keyword journalists/bloggers search when they need a source to cite. They click the ad, find a useful reference page, and link organically — no link is purchased. Treat as the same tactic as #106, layered onto Spike's statistics-backlink strategy (#25), not a separate workstream.

### #137 — High Converting Popups To Boost Income
- Category: On-Page SEO
- Same mechanic as the existing exit-intent tactic (#108): use a popup builder to surface an offer at the right moment on blog.spike.sh. Point it at the content upgrades/lead magnets already planned (on-call templates, the maturity-quiz scorecard in #149) instead of a generic "offer" — another trigger/placement for the same lead-capture assets, not a new workflow.

### #141 — Add [YEAR] To The Content Title
- Category: On-Page SEO
- Add the current/next year to evergreen "best of" title tags on blog.spike.sh (e.g. "Best On-Call Software 2026") as a freshness signal. Pairs directly with the existing #33 (publish-next-year-early) and #8/#51 (quarterly refresh) tactics.

### #142 — Find The Most Shared Content On Reddit
- Category: SEO
- Use `reddit.com/domain/[competitor-domain]/top/?sort=top&t=all` (swap in pagerduty.com, opsgenie.com, atlassian.com) to see which competitor pages got the most Reddit traction, then mine those threads for topic gaps blog.spike.sh doesn't cover. A domain-targeted sharpening of the existing Reddit content-ideation tactics (#67/#101).

### #143 — Build Mentions To Get Lots Of AI Visibility
- Category: AI SEO
- Systematically pursue genuine third-party mentions beyond spike.sh itself — G2/Capterra/StackShare listings, guest slots on SRE/DevOps podcasts, Reddit/Quora/Medium answers, YouTube mentions, LinkedIn posts — since LLMs pull citation/trust signals from mentions across the web, not just a brand's own site.
- **Formalize as a recurring off-site workstream alongside the existing #14/#93 AEO-tracking program** — every legitimate mention is effectively a ranking signal for AI-generated answers.

### #147 — Get Featured In From Sources Across The Web
- Category: SEO
- Use `intitle:"incident management software" (intitle:top OR intitle:best) -intext:spike` to find "best X" roundup articles that don't yet mention Spike, then find the author/site owner via Hunter or LinkedIn and pitch for inclusion. Targets Google's "Sources across the web" SERP feature and improves odds of AI-platform citation. Extends the existing outreach tactics (#54/#79/#100) with a specific gap-finding search operator.

### #148 — Exact Time To Change The Year From Title
- Category: Content Optimization
- Before bumping a title's year (per #33/#141), check GSC Performance for the last 28 days: compare impressions on queries containing the current year vs. next year, and switch once next-year volume exceeds current-year volume. A data-driven trigger rather than a calendar guess — add to the standing GSC content-optimization checklist.

### #149 — Turn Visitors Into Leads With Quiz Scorecard System
- Category: SEO
- Build a gamified scorecard quiz (e.g. via ScoreApp) such as an "On-Call Readiness Score" or "Incident Response Maturity Score" — a few questions generating a personalized score/report in exchange for an email. Extends the existing content-upgrade/lead-magnet tactics (#91/#108) with a more interactive format.

### #151 — Blog Title Templates That You Can Steal For Your Site
- Category: SEO
- Swipe-file of proven title templates for content planning: "Case Study: How We [Result]" ("How We Cut MTTA by 40% With Spike"), "[Product] vs [Product]: Which Is Best for You?" (already used for comparison pages), "X Best [Competitor] Alternatives," "How To [Solve Problem] in X Easy Steps," "[Topic]: The Definitive Guide." Reinforces several already-implemented tactics with proven formats.

### #152 — Utilize Social Platforms That Optimize AI Searches
- Category: AI SEO
- Maintain a consistent, genuine posting cadence on LinkedIn (explicitly "essential for B2B brand authority in AI-generated content"), plus Reddit, X, and YouTube — AI models draw entity/trust signals from social platforms when deciding whose content to surface, not for backlinks but for credibility.
- **Reinforces the existing #32 LinkedIn Pulse tactic and the #14/#93 AEO program — treat consistent LinkedIn presence as standing AEO work, not a one-off.**
