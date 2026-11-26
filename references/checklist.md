# Core checklist

Reference baseline: 2026-11-26. Evidence-gathering methods are this skill's procedures; the force and applicability of official guidance follow the corresponding current source

## T: Search eligibility and discoverability

| ID | Check and evidence | Guidance type and assessment boundary |
|---|---|---|
| T01 | For pages intended for public indexing, examine public access, robots.txt, and relevant access controls | Technical requirement; collect separate evidence for ordinary client access and Googlebot access |
| T02 | Read the final URL and HTTP status, confirming that the intended content works | Technical requirement; HTTP 200 is one eligibility condition |
| T03 | Examine indexable main content and indexing controls such as meta robots and X-Robots-Tag | Technical requirement; establish whether the user wants this page to appear in Search |
| T04 | Verify actual indexing status using URL Inspection or Search Console, recording the data date | Evidence confirmation; record eligibility conditions and actual inclusion separately |
| T05 | Check that titles, main headings, alt text, and link text accurately describe the content | Best practice; assess against readers' actual vocabulary |
| T06 | Inspect relevant internal links to verify discovery of the target and related content | Best practice; gather evidence within the authorized scope |

T01-T04 use [Google Search technical requirements](https://developers.google.com/search/docs/essentials/technical); T05-T06 use [Search Essentials: key best practices](https://developers.google.com/search/docs/essentials#key-best-practices). For indexing controls, use [robots meta and X-Robots-Tag](https://developers.google.com/search/docs/crawling-indexing/robots-meta-tag)

## C: Content quality and trust

| ID | Check and evidence | Applicability |
|---|---|---|
| C01 | Identify the target reader's task and assess whether the complete content enables its completion | Quality recommendation; consider informational, transactional, comparison, tool, and other page purposes |
| C02 | Identify original information, practical work, research, or analysis and its evidence | Quality recommendation; tools, images, videos, and interactive features can also be main content |
| C03 | Verify claims against data, sources, conditions, and checkable facts | Quality recommendation; return to primary evidence in proportion to a claim's significance |
| C04 | Check actual support for the author or site's background, relevant experience, and expertise | Quality recommendation; select relevant E-E-A-T evidence for the purpose, with trust at its core |
| C05 | Verify professional evidence and applicable conditions for significant health, financial, or safety claims | Quality recommendation; examine these YMYL topics in greater depth |
| C06 | Check title-content alignment, depth, readability, and added value | Quality recommendation; choose length according to the reader's task |
| C07 | Check time-sensitive information and whether date changes reflect substantive updates | Quality recommendation; assess freshness needs for the topic |

Use the self-assessment, main-content, and E-E-A-T sections of [Creating helpful, reliable, people-first content](https://developers.google.com/search/docs/fundamentals/creating-helpful-content). E-E-A-T describes quality dimensions identified through multiple signals. Quality-rater feedback evaluates system quality; automated systems determine rankings

## E: Page experience

| ID | Check and evidence | Guidance type |
|---|---|---|
| E01 | Measure Core Web Vitals, recording the URL, date, data type, and valid sample | Published ranking consideration; keep pending verification for drafts or missing measurements |
| E02 | Check secure connections and mobile rendering | Experience recommendation |
| E03 | Examine ads, interstitials, and main-content identification, preserving rendered evidence | Experience recommendation |

Use [Understanding page experience](https://developers.google.com/search/docs/appearance/page-experience). Distinguish Core Web Vitals from other experience recommendations. Page experience covers multiple aspects; measurement conclusions follow the scope of the original data

## A: AI search eligibility and representation

Use when the user requests an AI search audit; load this section for a draft review when its goal includes AI search

| ID | Check and evidence | Assessment boundary |
|---|---|---|
| A01 | Verify actual indexing and snippet eligibility, reusing T-group evidence | Official eligibility requirement; record actual citation outcomes separately |
| A02 | Check textual representation of important information and discoverable internal links | Official best practice |
| A03 | When structured data exists, compare it with visible content; check merchant information freshness when applicable | Official best practice; verify data correctness and eligibility for specific Search features separately |
| A04 | When checking an existing AI response, preserve the query, date, locale, response, and cited URLs | Representation accuracy check; read whether the sources support the associated claims |
| A05 | Read the Search Console Search generative AI setting and its effective value after parent-property inheritance | AI search eligibility setting; assess Include or Exclude against the goal, keeping missing account evidence pending verification |
| A06 | When evaluating AI visibility, read the Generative AI performance report, preserving report identity, period, PT timezone, dimensions, and aggregation | AI impression measurement; distinguish impressions, traffic, and conversions, checking impression volume and A05 when the report is missing |

Use [AI features and your website](https://developers.google.com/search/docs/appearance/ai-features) and [Attribution and factuality](https://developers.google.com/search/docs/fundamentals/gen-ai-attribution-factuality). Google specifies the SEO foundations; dedicated AI files and special schema are not eligibility requirements. Connect recommendations to observable reader needs, understandability, or supporting sources

For A05, use [Search generative AI control](https://support.google.com/webmasters/answer/16908024) to verify the property's actual setting and parent inheritance. Published defaults provide background; setting changes follow user authorization. For A06, use [Generative AI performance report](https://support.google.com/webmasters/answer/16984139): this report covers AI Overviews and AI Mode impressions, with a separate report for Discover. The documentation states that exported values may turn the interface's `~` or `-` into 0; preserve the original interface state and missing-value meaning in analysis

## Using ranking-system background

When explaining observation boundaries, read the [ranking systems guide](https://developers.google.com/search/docs/appearance/ranking-systems-guide). Semantic understanding, originality, links, reviews, freshness, deduplication, and spam detection provide background. Examine the corresponding quality through actual content; internal triggers, weights, and scores lie beyond external observation

The [Ranking Hub principles](https://developers.google.com/search/docs/ranking/principles-for-ranking-results) explain a shared usefulness standard. Gather evidence for each feature's results and source selections through its actual behavior
