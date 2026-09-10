# Maybe — plausible, lower priority, or needs more thought

23 tips that could work for Spike.sh but are either a stretch fit, tool/workflow-heavy relative to their payoff, or carry some risk of feeling off-brand for a technical B2B audience. Revisit once the "Implement" list is underway.

### #7 — Future Keywords To Rank #1 Without High Effort
- Category: Keyword Research
- Target "future prediction keywords" — anticipated next-version product names or upcoming integrations/platforms before official info exists, and monitor Product Hunt/Kickstarter-style launch feeds for new products worth early coverage. Plausible around anticipated competitor feature launches or new platforms Spike could integrate with, but a stretch fit for a B2B incident-management product — opportunistic only.

### #10 — SEO Hack That Skyrockets The Site's User Retention
- Category: On-Page SEO
- Deliberately cut off visuals (stats/charts/tables) at the top of content so only half is visible, inducing scroll to see the rest. Could apply to data-heavy posts (e.g. downtime/incident statistics content), but somewhat gimmicky for a technical B2B audience — test cautiously.

### #11 — Boost Website CTR Using A Simple Way
- Category: On-Page SEO
- For list-based articles, add a curiosity-gap modifier to one item in the title (e.g. "10 Incident Management Best Practices (#7 Will Change How You Run Postmortems)") to lift CTR from search results. Usable sparingly for blog listicles; overuse risks feeling clickbait-y.

### #15 — Rank #1 Easily For Reddit Based Keywords
- Category: Content Optimization
- Target "[keyword] + Reddit" search queries by curating real Reddit discussion into a dedicated article — e.g. "Best On-Call Software Reddit" or "PagerDuty Alternatives Reddit" roundups. Double benefit: classic SEO for the "+ Reddit" query pattern, and AEO since Reddit content is heavily cited by AI systems. Worth testing as a content format.

### #18 — How Many Times Should Keywords Be Used In A Post
- Category: On-Page SEO
- Count target-keyword frequency across the top 10 ranking pages and average it as a target. Keyword-density matching is a somewhat dated practice (modern Google is more semantic/intent-based) — use loosely as a sanity check, not a strict target.

### #19 — Find Unlimited Keywords For Programmatic SEO
- Category: Keyword Research
- Programmatic SEO via templated pages with one incrementing variable (number, location, brand name) to generate keyword variants at scale. Could work narrowly — e.g. "[Integration] on-call alerting setup" pages per integration, or "[Competitor] alternative" pages per competitor — but full programmatic scale (thousands of thin pages) doesn't fit Spike's content-quality bar. Borrow the pattern selectively.

### #36 — Increase Font Size To Boost Website's Revenue
- Category: On-Page SEO
- Default WordPress font size (16px) is often too small, especially on mobile; bumping to ~20px with better contrast improves readability and time-on-page. Worth a quick readability/accessibility audit on blog.spike.sh, but minor and low-priority — the original "more ads" revenue rationale doesn't apply.

### #44 — Know Search Volume For 0 Search Volume Keywords
- Category: Keyword Research
- For keywords showing "0 search volume" in Keyword Everywhere, cross-reference a ranking page's actual Search Traffic estimate and ranked-keywords export to find the keyword's real, undercounted traffic. Useful nuance for deep-dive keyword research, but tool/workflow-specific and lower leverage than the GSC-based tactics already slated for implementation.

### #48 — Boost Visitors Using Notifications Without Hassle
- Category: Technical SEO
- Install a push-notification platform (e.g. OneSignal) so opted-in visitors get notified of new content/changelog updates, driving repeat visits. Plausible for re-engaging blog readers or changelog subscribers, but adds friction/complexity and isn't core to AEO/backlink goals — test only if the team wants a dedicated return-visit lever.

### #60 — Get Free Links Using Image Link Building Strategy
- Category: Backlinks
- Release original photos/graphics under a Creative Commons license (distributed via Flickr) so other sites can reuse them in exchange for attribution backlinks. Could adapt into releasing original diagrams (incident-response-process diagrams, architecture diagrams) under a similar sharing license — but this is a stretch fit for a B2B SaaS versus a photography/design niche. Small experiment only.

### #119 — Find Out Who Is Stealing Your Content For Free
- Category: SEO
- Copy a distinctive 5+ word sentence from Spike's own content and search it on Google in quotes — any site republishing/scraping the content will surface in results, letting you detect content theft without paid tools. Useful periodic content-protection check for blog.spike.sh/docs.spike.sh (scraped content can also cause duplicate-content SEO issues) — a defensive maintenance task, not a growth tactic. Low priority, occasional use.
- Note: read out of order (row numbering runs 1-152, this one was opened while scouting later rows).

## Batch 1 (rows 65-91)

### #73 — Increase Traffic Using Brand Alternative Method
- Category: Keyword Research
- Same "swap one variable" pattern as existing #45 (Implement) and #19 (Maybe), pushed further: copy 80-90% of an article and only swap the brand/product name to generate near-duplicate variants at scale. Risky for a quality-focused B2B blog — this level of near-duplicate generation could read as thin content if applied broadly (e.g. to "[Integration] on-call setup" pages). Usable in a limited, hand-reviewed way only.

### #80 — Turn Free Stock Photos Into Free Backlinks
- Category: Backlinks
- Same mechanic as existing #60 (Maybe): upload original images to Unsplash/Pexels, track reuse (Unsplash stats, WordPress credit lines, reverse image search), then ask sites to credit Spike directly. For Spike this would mean publishing original diagrams (incident-response flowcharts, on-call architecture diagrams) rather than photos — a stretch fit versus a photography niche, but a low-cost experiment alongside #60 since it's the same tactic.

### #84 — How To Measure True Keyword Difficulty
- Category: Keyword Research
- A more rigorous refinement of the existing keyword-viability checklist (#37): manually score Relevance/Authority/Popularity (1-5) for ranking pages via Keywords Everywhere's Detailed Breakdown instead of trusting a single automated KD score, to catch cases where a keyword looks harder or easier than it really is. Useful nuance but heavier effort (30 min, 5-star) relative to payoff — an optional deeper pass for high-value keywords only.

### #90 — GIFs For Website Brand Awareness To Millions People
- Category: Backlinks
- Upload branded GIFs (Spike name/logo) to GIPHY; since Twitter/Slack/iMessage pull GIFs via GIPHY's API, a popular GIF can circulate widely with "via [brand]" attribution, building awareness and occasional backlinks. Plausible novelty experiment, but meme-style branded GIFs are a stretch fit and carry some risk of feeling off-brand for a technical SRE/DevOps B2B audience — test small first.

## Batch 2 (rows 92-124)

### #112 — Turn Your Website Into A Brand With YouTube
- Category: SEO
- Sponsor SRE/DevOps-niche YouTubers to do a screen-recorded walkthrough of Spike, explaining what it does and linking to spike.sh — the goal is lifting "branded searches" (people searching "Spike" directly after seeing the video), which both Google and AI systems read as a trust/relevance signal. Legitimate but paid and relationship-dependent, and the SRE/DevOps YouTube niche is much smaller than the general niches this tip was written for — pilot with one or two channels before committing real budget.

### #113 — Licensed Photos To Earn Automatic Backlinks
- Category: Backlinks
- Same mechanic as the existing #60/#80 (Maybe) image-licensing tactic, with a specific implementation detail: embed an HTML caption with a copyright/attribution backlink directly beneath original images before distributing them (e.g. via Unsplash), so any site that reuses the image also carries the link. Doesn't change the underlying stretch-fit concern already noted for #60/#80 — group as one experiment if pursued.

## Batch 3 (rows 125-152)

### #126 — Build Free Backlinks Using AI Generated Images
- Category: AI SEO
- Generate niche-relevant AI images, upload to image-sharing sites under a branded account name, and track reuse for photo-credit backlinks. Same stretch-fit concern already flagged for the existing #60/#80/#113 image-licensing tactics — group as one experiment if pursued.

### #128 — Become Viral On Facebook For Your Website
- Category: SEO
- Build a Facebook page, post AI-generated eye-catching niche images, and share into relevant Facebook groups for organic engagement/traffic. Facebook skews consumer-audience relative to Spike's SRE/DevOps buyer, who is far more active on LinkedIn/X/Reddit — plausible minor channel, not a priority.

### #135 — Emulate Searches From Any Location You Want
- Category: SEO
- Use Chrome DevTools' Sensors panel with Google Maps coordinates to see how search results/AI Overviews look from a specific city or country. Useful for checking Spike's visibility in specific international markets, but a research/QA utility rather than a growth lever — occasional use alongside the keyword-viability checklist (#37).

### #138 — Easily Get Traffic For High Competition Keywords
- Category: SEO
- Create a dedicated X/Twitter account named after a high-competition keyword niche, post short link-backed content, and let X's domain authority claim a Twitter-card slot in Google's SERP for that keyword. Legitimate (real account, real content), but running a second keyword-branded identity separate from Spike's main voice is extra overhead and a stretch fit for enterprise B2B tone — test small first.

### #139 — Increase CTR Using A Very Simple Method
- Category: On-Page SEO
- For page-1-ranking blog.spike.sh posts, add one relevant emoji to the title tag to stand out in the SERP and lift CTR. Cheap to test, but risks reading as unprofessional for an enterprise SRE/DevOps audience if overused — same caution already flagged for the curiosity-gap title tactic (#11); use sparingly and only where genuinely on-topic.

### #144 — Build High Quality Backlinks For Free
- Category: Backlinks
- Publish "best X tools" listicle content that attracts inbound outreach from other sites wanting to be featured, then negotiate a reciprocal backlink in exchange for inclusion. The listicle-publishing half is redundant with tactics already in place; the explicit link-for-inclusion exchange brushes against Google's link-scheme guidance on reciprocal linking — if pursued, publish for the listicle's own SEO value and treat any inbound link as a bonus rather than actively negotiating quid-pro-quo exchanges.
