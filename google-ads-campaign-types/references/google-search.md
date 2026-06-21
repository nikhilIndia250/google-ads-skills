# Search Campaigns

## What it is

Text ads on Google Search results pages, shown to people actively searching for your products/services. Targeting is built primarily on keywords, not audience signals — the closest thing to "old school" intent-based advertising in Google Ads, and still the highest-control campaign type.

## When to use it

- Sales, leads, or website traffic goals where you want keyword-level control over exactly which queries trigger your ads.
- Longer sales cycles, where leads (not last-click sales) are the more honest objective.
- You want easy setup with no special creative assets required (just text + keywords), as opposed to Display/Video/Shopping which need images, feeds, or video.

## Setup mechanics

### Campaign goal & structure
- New campaign → choose objective (Sales / Leads / Website traffic, or "create without a goal's guidance") → select Search as the campaign type → at least one conversion goal is required even without goal guidance.

### Bidding
- Choice of bid focus aligns to objective: **Conversions** (sales/leads — requires conversion tracking), **Clicks** (traffic), **Conversion value** (when conversions have assigned values — enables ROAS targeting), or **Impression Share** (visibility on a target % of relevant search pages).
- More experienced advertisers can select a bid strategy directly rather than going through the goal-based flow.
- Additional controls: conversion type selection, ad schedule (dayparting), ad rotation (optimize vs. even rotation).

### Targeting
- **Search Network + Search Partners**: toggle whether ads also show on partner search engines beyond google.com.
- **Display Network expansion**: optional checkbox to extend select Search campaigns onto Display inventory when Google judges it effective — worth flagging in audits since it can quietly shift spend off pure search intent.
- **Location options**: refine by relationship to the targeted location (e.g., "people searching for your targeted locations" vs. "people in your targeted locations") — relevant for travel/event advertisers targeting a destination rather than a resident base.
- **Location exclusions**: target broad and carve out specific areas.
- **Language targeting**: ads/keywords should match the languages selected.
- **Audience layering**: demographics, interests, in-market, remarketing — layered on top of keyword targeting, not a replacement for it.

### Keyword match types
- **Broad match** (default, no symbols): widest reach, most reliant on Smart Bidding to find relevant queries.
- **Phrase match** (`"keyword"`): matches the phrase and close variants.
- **Exact match** (`[keyword]`): closest targeting to the literal query.
- **Negative keywords** (`-keyword`): exclude irrelevant queries.

### Ad group structure
- **Standard**: you supply keywords; you write ads to match. One ad group type per campaign.
- **Dynamic Search Ads (DSA)**: Google crawls your site content to auto-generate headlines/final URLs/targeting from page content or categories; you still write description lines. Better suited to large catalogs/advertisers than first-time users.

### Ad assets
Sitelinks, callouts, calls, structured snippets, app assets, promotions, lead forms, price assets, location assets, image assets — these expand ad real estate and are worth auditing for completeness (default population is sitelink/callout/call only; the rest must be added deliberately).

## Common pitfalls (audit checklist)

- **Match type skew**: heavy reliance on broad match without strong negative keyword hygiene or sufficient conversion data for Smart Bidding to interpret broad match well — common cause of irrelevant spend.
- **Search Partners / Display expansion on by default** diluting pure search intent without the client realizing it's enabled.
- **Bid focus mismatched to goal**: e.g., bidding on Clicks when the real objective is Leads, or vice versa.
- **Conversion tracking not set up or misattributing** — bidding strategy is only as good as the conversion signal it optimizes on.
- **Single ad group catch-all** structure instead of tightly themed ad groups — hurts Quality Score and ad relevance.
- **Fewer than 3 ads per ad group** — Google recommends at least 3 to give Smart Bidding/Ad Strength enough variation to learn from.
- **Missing or thin ad assets** (sitelinks/callouts/etc.) — easy wins left on the table, and a frequent finding in account audits.
- **Location targeting too narrow**, sometimes to the point predicted clicks show as 0 — easy to miss without checking campaign construction warnings.
