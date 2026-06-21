---
name: google-ads-campaign-types
description: Deep reference on every Google Ads campaign type — Performance Max, Search, Display, Video (and its 6 subtypes), App (installs/engagement/pre-registration), and Shopping/Performance Max with Merchant Center feed. Covers when to use each type, bidding strategies, targeting options, asset/eligibility requirements, and common pitfalls. Use this skill whenever the user asks about choosing a campaign type, structuring a Google Ads account, auditing a UAC/DemandGen/Search/Shopping/Video/Display campaign, comparing campaign types, troubleshooting underperformance, writing an audit report, or building any tool (Scripts/Sheets/dashboard) that touches Google Ads campaign settings. Trigger even if the user just names a campaign type (e.g. "PMax", "ACi", "UAC", "DemandGen") without saying "Google Ads" explicitly.
---

# Google Ads Campaign Types

A reference skill covering all Google Ads campaign types in depth: what they're for, how they work, bidding/targeting mechanics, setup requirements, and the pitfalls that actually show up in client accounts.

Source: built from Google's own Ads Help Center (support.google.com/google-ads), last refreshed June 2026. Google updates campaign features frequently — if something looks like it might have changed (new bid strategy, new subtype, renamed feature), do a quick web search to confirm before stating it as fact in an audit or client-facing doc.

## How to use this skill

1. **Start here for selection logic** (below) when the question is "which campaign type should I use."
2. **Jump to the relevant reference file** for deep mechanics, bidding, targeting, and pitfalls on a specific type:
   - `references/google-performance-max.md` — Performance Max
   - `references/google-search.md` — Search campaigns
   - `references/google-display.md` — Display campaigns
   - `references/google-video.md` — Video campaigns (all 6 subtypes)
   - `references/google-app.md` — App campaigns / UAC (installs, engagement, pre-registration)
   - `references/google-shopping.md` — Shopping campaigns & PMax with Merchant Center feed
3. **For audits**, read the relevant reference file's "Common pitfalls" section first — it's organized to mirror the kind of issues that actually show up in account audits (tracking misconfiguration, mismatched bid strategy vs. budget/data volume, targeting too narrow/broad, asset gaps).
4. Don't load every reference file for every question — pick the one(s) relevant to what's being asked. Each file is self-contained.

## Campaign type selection logic

Google Ads organizes campaign types around a few entry questions: **what's the goal, what assets do you have, and how much manual control do you want?**

| If the goal is... | Default recommendation | Also consider |
|---|---|---|
| Online sales / leads, full-funnel, willing to trust automation | Performance Max | Search (if you want to protect specific high-intent keywords) |
| Online sales / leads, want keyword-level control | Search | PMax to fill in gaps beyond keyword reach |
| Sell retail/product inventory | Shopping (standard) or PMax with Merchant Center feed | PMax for broader reach; standard Shopping for tighter channel/bid control |
| Brand awareness / reach on YouTube | Video — Video reach campaigns | PMax (if conversions also matter) |
| Drive conversions via video ads | Video — Drive conversions (Video action campaigns) | PMax |
| App installs | App campaigns — App installs (ACi) | — |
| Re-engage existing app users | App campaigns — App engagement (ACe) | — |
| Pre-launch app buzz (before Play Store release) | App campaigns — Pre-registration | — |
| Build awareness while browsing (not search) | Display | PMax, Video |
| Local store visits / nearby footfall | PMax (local goal) or Shopping w/ local inventory ads | — |

**Key relationship to remember**: Performance Max is not a replacement for Search — it's designed to *complement* keyword-based Search campaigns. If a user's search query exactly matches an exact/phrase/broad-match keyword in a live Search campaign, the Search campaign is prioritized over PMax for that auction. PMax can still show on branded terms if the Search campaign is budget-constrained or has stricter targeting — use brand exclusions in PMax or negative keywords to prevent this overlap when it's not wanted. This matters a lot when auditing accounts that run both — cannibalization between PMax and Search is one of the most common audit findings.

## Cross-cutting concepts worth knowing before diving into a specific type

- **Smart Bidding** underlies almost every automated campaign type now (Target CPA, Target ROAS, Maximize Conversions, Maximize Conversion Value). It needs enough conversion volume to exit the "learning phase" reliably — recommend 30+ conversions/month per campaign as a rough floor before trusting tCPA/tROAS numbers.
- **Learning phase**: new campaigns or major setting changes (bid strategy, targeting, creative) trigger a 5–7 day learning phase. Frequent changes during this window reset learning and delay optimization — a very common cause of "this campaign never stabilizes" in audits.
- **Conversion tracking accuracy is the precondition for everything else.** Before evaluating any bid strategy or targeting choice, verify conversion actions are firing correctly and that the optimization goal actually reflects business value (e.g., not optimizing toward a vanity event while the real money event is uncounted).
- **Asset quality drives automated formats.** PMax, Display, and App campaigns are all responsive/asset-based — Google AI assembles ads from the assets provided. Thin asset libraries (few headlines/images/videos) are a frequent root cause of underperformance that looks like a targeting or bidding problem.

## Files in this skill

```
google-ads-campaign-types/
├── SKILL.md
└── references/
    ├── google-performance-max.md
    ├── google-search.md
    ├── google-display.md
    ├── google-video.md
    ├── google-app.md
    └── google-shopping.md
```
