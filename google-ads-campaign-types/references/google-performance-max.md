# Performance Max

## What it is

A goal-based campaign type that runs from a single campaign across all Google Ads inventory: Search, Display, YouTube, Discover, Gmail, and Maps. Instead of picking placements or keywords, you give Google your conversion goal (CPA/ROAS target), creative assets, and audience signals, and Smart Bidding + Smart Creative decide where and to whom to show ads in real time.

## When to use it

- You have a clear conversion goal (sales, leads, local visits) and conversion tracking is reliable.
- You want reach across all Google channels without managing separate campaigns per channel.
- You want incremental reach/value beyond what a keyword-based Search campaign alone can capture.
- PMax becomes a selectable campaign type when the advertising objective is Sales, Leads, or Local store visits/promotions. If it's not showing (or is the only option when you wanted something else), use "Create a campaign without a goal's guidance" to reveal all campaign types.

## How it works

- **Bidding**: Smart Bidding (Maximize Conversions / Maximize Conversion Value, optionally with a tCPA or tROAS target) combined with cross-channel attribution.
- **Creative**: Built from asset groups (headlines, descriptions, images, logos, videos). If "Final URL expansion" is on, Google can swap in a different landing page than your specified Final URL based on the user's query, and generate matching headline/description/assets — worth knowing when a client asks why traffic is landing somewhere unexpected.
- **Audience signals**: Optional but valuable — first-party customer data, in-market/affinity segments, etc. They steer (not restrict) targeting; PMax can still go beyond the signal if it finds higher-converting users.
- **Value rules**: Let you tell PMax that some conversions are worth more than others (e.g., new customers, specific locations) so bidding optimizes for actual business value rather than raw conversion count.
- **Brand safety**: Account-level controls exist to exclude content categories you don't want ads to appear next to.

## Relationship to Search campaigns

- PMax is designed to complement, not replace, keyword-based Search campaigns.
- If a user's query exactly matches an exact/phrase/broad keyword that's live in a Search campaign, the Search campaign wins that auction over PMax. Search themes inside PMax get the same priority tier as phrase/broad match keywords.
- PMax can still surface for branded terms even when those are set to exact match in a Search campaign — typically when the Search campaign is budget-limited or has narrower targeting. Fix with brand exclusions in PMax or negative keywords.

## Merchant Center / retail use case

- For online sales goals, link a Merchant Center account (with complete product data, shipping, tax settings) to power Shopping-style placements inside PMax.
- Advertisers with a Merchant Center feed don't strictly need creative assets to launch, but providing them improves surface coverage and performance — without them, ads are more limited and may rely more heavily on auto-generated content from the feed.
- Up to 100 PMax campaigns per account; Google recommends consolidating where possible rather than fragmenting budget across many small PMax campaigns (fragmentation starves each campaign of the conversion volume Smart Bidding needs).

## Store goals / local

Advertisers with local contacts or directions set up as a conversion goal can run PMax for local visits — this is the modern path for what used to be Local campaigns, with no separate budget or inventory setup required.

## Common pitfalls (audit checklist)

- **Cannibalization with Search**: check for brand term overlap between PMax and Search campaigns; missing brand exclusions is one of the most common findings.
- **Conversion goal misconfigured**: PMax bidding is only as good as the conversion action it's optimizing toward — verify the conversion action reflects real business value, not a proxy/vanity event.
- **Thin asset groups**: too few headlines/images/videos limits how PMax can serve across surfaces; this is often misdiagnosed as a targeting or budget problem.
- **No audience signals provided**: PMax can technically run without them, but it loses a meaningful steering input, especially early when there's little conversion data to learn from.
- **Final URL expansion surprises**: if a client complains traffic lands on an unexpected page, check whether Final URL expansion is on and whether the landing pages it's allowed to choose from are actually appropriate.
- **Budget fragmentation**: many small PMax campaigns instead of consolidated ones — each one individually starved of conversion volume, none of them reliably out of the learning phase.
- **Value rules absent on mixed-value conversions**: if some conversions (e.g., a high-AOV customer) are worth more than others and there are no value rules, bidding optimizes blindly toward volume.
