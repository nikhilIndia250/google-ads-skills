# App Campaigns (UAC)

Commonly called "UAC" (Universal App Campaigns) historically; Google's current naming is just "App campaigns," with three subtypes: App installs (ACi), App engagement (ACe), and App pre-registration.

## What it is

A fully automated, asset-based campaign type that promotes an app across Search, Google Play, YouTube, Discover, Gmail, and the Display Network — all from one campaign. You provide text, starting bid/budget, languages/locations, and creative assets; Google tests asset combinations and serves the best-performing ads across formats and networks automatically. There's no placement-level control — this is the most "hands-off the wheel" campaign type in Google Ads.

## Eligibility / prerequisites

- App must already be published on Google Play (Android) or the App Store (iOS) — App campaigns can't run pre-launch except via the dedicated pre-registration subtype.
- A valid payment method on the account.
- Basic app info: name, category, target audience.
- Ad assets: text, images, videos, and HTML5 if relevant (auto-pulled in part from the store listing, but supplementing them improves coverage).

## Subtype 1: App installs (ACi)

Focused on driving new downloads.

### Bid strategies (choose based on goal and data volume)
- **Target cost per install (tCPI)**: optimize purely for install volume at a target cost.
- **Target cost per action (tCPA)**: optimize for a specific in-app event post-install (e.g., signup, first purchase) — needs install + in-app conversion tracking wired up.
- **Target return on ad spend (tROAS)**: optimize for revenue value of installs — needs in-app purchase/value tracking.
- **Maximize Conversions**: no target bid required; spend the budget to get as many conversions as possible per the selected conversion action.

tCPA and tROAS strategies may continue serving ads until the conversion window closes (not just until the literal install event), which is worth knowing when interpreting "why is this campaign still spending after installs look flat."

### Setup specifics
- Campaign goal: App promotion → subtype: App installs.
- Android apps get an automatic Google Play download conversion action created if one doesn't already exist for that app in the account/manager account — this happens as soon as campaign construction starts, even if construction is abandoned, so orphaned auto-created conversion actions are a known artifact to watch for in account audits.
- Deep links: iOS deep links route users who already have the app installed straight to an in-app page (others land on the store page); Android deferred deep links route users to an in-app page right after install+open.
- Audience signals (optional) can be added to steer targeting faster, similar to PMax.
- Up to 20 each of images, videos, HTML5 assets per ad group.

### Optimization tips
- Use square and vertical video — mobile-heavy inventory rewards it.
- Use feeds in App campaigns to surface specific in-app content/products in ads (more relevant, better targeted creative).
- Review App campaign asset reporting regularly — thin or stale asset libraries are the most common silent performance drag.

## Subtype 2: App engagement (ACe)

Aimed at existing app users — driving them back into the app to take a specific action, rather than acquiring new installs. Typically paired with App Connect / deep linking so that campaigns originally built for web conversions can also route engaged users into the app experience. Useful for retention/reactivation plays once a meaningful installed base exists — generally not the right subtype until there's enough existing user volume to target.

## Subtype 3: App pre-registration

Promotes pre-registration for an app or game before it's released on Google Play — used to build a launch-day install spike rather than ongoing installs. Only relevant pre-launch; once the app ships, campaigns typically transition to ACi.

## Common pitfalls (audit checklist) — these mirror real recurring findings in agency UAC audits

- **Conversion tracking misconfiguration**: install or in-app event tracking not firing correctly, or tCPA/tROAS optimizing against the wrong event entirely (e.g., optimizing toward a low-value engagement event while the real monetization event goes untracked).
- **Fictional/unrealistic tCPA or tROAS targets**: targets set without basis in actual historical CPA/ROAS data, causing the algorithm to either underspend (target too aggressive) or overspend with no discipline (target too loose).
- **Impression share loss going unmonitored**: budget or bid constraints quietly capping reach without anyone noticing until volume drops.
- **Network split inefficiency**: spend concentrated on lower-intent networks (e.g., Display-heavy delivery) without review of where conversions are actually coming from, since App campaigns abstract away placement-level reporting by default — deeper reporting (e.g., via Google Ads Scripts pulling network/geo/asset-level data) is often needed to see this.
- **Language-targeted campaigns underinvested relative to performance**: in multilingual markets, language-segmented campaigns sometimes show a meaningfully better CPA than the broader campaign but stay capped at a low budget out of inertia rather than reallocation.
- **Orphaned auto-created conversion actions** from abandoned campaign construction attempts, muddying the conversion action list.
- **Thin or store-listing-only assets**: relying solely on auto-pulled store listing assets instead of supplementing with dedicated ad creative.
- **Deep links not configured**, sending engaged/returning users to the generic store page instead of relevant in-app content.

## Note on Google's pace of change here

App campaign features (bid strategies, asset types, audience signal options) are updated more frequently than most other campaign types. Treat the bid-strategy and asset-limit specifics above as accurate as of mid-2026, but verify against the live UI or a quick search before stating exact limits in a client-facing audit.
