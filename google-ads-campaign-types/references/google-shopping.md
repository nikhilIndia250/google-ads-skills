# Shopping Campaigns & Performance Max with Merchant Center Feed

## What it is

Product-listing ads (image, title, price, store name) shown on Search results and the Shopping tab, built from a Merchant Center product feed rather than keywords. There are two ways to run them: **Standard Shopping campaigns** (more manual control) or **Performance Max with a Merchant Center feed** (broader reach, more automation). Store owners can also extend either into **Local Inventory Ads** to promote products available in physical stores.

## Prerequisite

A Google Merchant Center account with: business details, tax info (US), a verified/claimed website, shipping settings, and a complete product feed. The Google Ads account must be linked to Merchant Center before either campaign type can use the feed.

## How Shopping ads work

Product data submitted via Merchant Center (not keywords) determines how and where ads show — Google matches user search intent to the most relevant products in the feed. Google may also enrich ads using landing page content, images, and other signals (including AI-generated enhancements); advertisers can opt out of these enrichments via their account manager if needed.

## Performance Max vs. Standard Shopping — the decision that matters most for retail clients

| | **Performance Max (w/ Merchant feed)** | **Standard Shopping** |
|---|---|---|
| **Where ads appear** | Shopping tab, Search (both shopping units and text ads), Google Images, Display Network, YouTube, Gmail, Demand Gen, Maps (via Local Inventory Ads) — auto-expands to new inventory/formats over time | Shopping tab, Search (shopping units only), Google Images, Search Partners (if enabled) |
| **Ad formats** | Shopping ads, Local Inventory Ads, Display ads, Text ads, YouTube ads, Vehicle ads | Shopping ads, Local Inventory Ads only |
| **Billing** | Pay for performance (clicks, CPM depending on format) | CPC — charged only on clicks to your landing page or local inventory page |
| **Bidding** | Automated only: Maximize Conversion Value (optional ROAS target), Maximize Conversions (optional CPA target) | Automated (Target ROAS, Maximize Clicks) or fully Manual CPC |
| **Creative** | Auto-generated/optimized from asset groups (text, image, video) + feed | Generated and optimized from the feed only — no separate creative assets |
| **Local Inventory Ads** | Auto-enabled when a local products feed is attached | Off by default — must check "Enable ads for products sold in local stores" |
| **Audience/value tooling** | Audience signals, Final URL expansion, New customer acquisition goal | Audience targeting (lists), no equivalent AI steering layer |

**Practical takeaway**: choose Standard Shopping when the client wants tight CPC control, manual bidding, or needs to keep Shopping spend cleanly separated from Display/YouTube/Demand Gen for reporting reasons. Choose PMax w/ feed when the goal is maximizing reach and conversion value across all surfaces and the client trusts automated bidding — which is increasingly Google's default recommendation for retail.

## Local inventory

Store owners can use Local Inventory Ads (within either campaign type) to promote products available at physical locations, surfacing nearby-store availability to local searchers — relevant for any client with both an online store and physical retail presence.

## Common pitfalls (audit checklist)

- **Incomplete or stale Merchant Center feed**: missing GTINs, mismatched pricing/availability vs. the live site, or disapproved products silently suppressing ad eligibility — always check Merchant Center diagnostics, not just Google Ads, when Shopping performance looks off.
- **Feed/Ads account link broken or using the wrong Merchant Center account** in multi-account setups.
- **Local Inventory Ads not enabled** for a Standard Shopping campaign when the client has physical stores and would benefit from local-intent visibility.
- **PMax vs. Standard Shopping chosen by default rather than deliberately** — i.e., nobody actually decided which fits the client's control/reporting needs, they just took whatever the new-campaign flow suggested.
- **No value rules / new customer acquisition goal configured on PMax** when customer value genuinely varies (e.g., repeat buyers vs. new), leaving bidding blind to that signal.
- **Manual CPC left running indefinitely** on Standard Shopping without ever testing automated bidding, especially once enough conversion volume exists to make Smart Bidding viable.
