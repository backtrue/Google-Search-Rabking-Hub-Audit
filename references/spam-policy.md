# Policy applicability

Reference baseline: 2026-11-26. First scan visible target evidence, then investigate items with relevant clues or an explicit user request. Site-level and historical conclusions need evidence of the corresponding scope

## Assessment method

Use this table to guide investigation. Assess specific conduct against the current definitions, exceptions, and regional conditions in [Google's spam policies](https://developers.google.com/search/docs/essentials/spam-policies)

| ID | Official policy topic | Evidence to obtain |
|---|---|---|
| S01 | Cloaking | Differences between user and search-engine content, and their purpose |
| S02 | Doorway abuse | Similar pages and their actual traffic destinations |
| S03 | Expired domain abuse | Domain history, reuse, and current value |
| S04 | Hacked content | Evidence of unauthorized insertions or anomalous code |
| S05 | Hidden text and link abuse | Hiding methods and their reader-facing purpose |
| S06 | Keyword stuffing | Locations of unnatural repetition |
| S07 | Link spam | Transaction purpose, link relationships, and qualification |
| S08 | Machine-generated traffic | Automated query methods and permission status |
| S09 | Malicious practices | Actual software, navigation, or privacy behavior |
| S10 | Misleading functionality | Differences between promised and available functionality |
| S11 | Scaled content abuse | Scale, original value, and manipulation purpose |
| S12 | Scraping | Original sources, copied scope, and added value |
| S13 | Site reputation policy | Third-party relationships and the purpose of using the host's ranking signals |
| S14 | Sneaky redirects | Redirect behavior by device or referrer and user expectations |
| S15 | Thin affiliation | Copied information and actual added value |
| S16 | User-generated spam | Actual comments, accounts, or uploaded content |
| S17 | Other grounds for demotion or removal | Evidence of legal or personal-information removals, policy circumvention, or fraud |

Preserve observed facts, applicability conditions, and missing evidence in each assessment. For a single article or page, keep missing evidence about site scale, transaction purpose, or domain history pending verification. Site-wide conclusions require site-wide evidence

## Conditions for common situations

Check these conditions against the corresponding sections of the official policies linked above

- AI-generated or human-produced content: assess S11 using scale, manipulation purpose, and user value
- Expandable sections, tabs, and accessibility content: examine their reader-facing purpose for S05
- Paywalls: for S01, compare content available to Google and authorized readers, and consult the applicable paywalled-content guidance
- Affiliate links and sponsorships: for S07 and S15, examine link qualification, original analysis, tests, or comparison value
- Third-party articles: for S13, investigate hosting purpose, regional conditions, actual evidence, and policy exceptions
- Domain reuse: for S03, investigate reuse purpose and current content value
- Redirects: for S14, distinguish normal uses such as migrations, sign-ins, and consolidation, assessing actual purpose and content differences

## Reporting and remediation

Visible page evidence can support findings that need verification or revision. Establish Google's manual-action status through the actual Search Console report. An audit request produces evidence and remediation guidance; formal reports, appeals, indexing-control changes, and publishing follow the authorization for each action
