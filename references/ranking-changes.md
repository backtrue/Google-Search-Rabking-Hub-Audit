# Update impacts, feedback, and appeals

Load when the user requests ranking or traffic change analysis, or feedback preparation. Reference baseline: 2026-11-26

## Verify the event and data

1. Read [ranking update notices](https://developers.google.com/search/docs/ranking/stay-informed) and the [Search Status Dashboard](https://status.search.google.com/), then open the specific event's direct URL. Record the preannouncement, rollout start, completion, and timezone
2. Distinguish preannouncements from actual rollout. Use the event notice for applicable locations, languages, and timing; apply UK notice requirements according to the conditions in Google's linked CMA source
3. For formal core-update impact analysis, follow the [core update guide](https://developers.google.com/search/docs/appearance/core-updates#check-if-theres-a-traffic-drop-in-search-console): wait for rollout completion and at least one full week of subsequent data, then compare an appropriate pre-rollout period. Record the observation window and data maturity for early snapshots
4. While data accumulates, continue investigating service, access, indexing, and measurement issues that can be checked immediately

## Analysis method

Verify the correct site, account, period, timezone, and filters before examining clicks, impressions, CTR, positions, and actual conversion data. Segment by page, query, country, device, and search type to locate changes, considering data anomalies, seasonal demand, site changes, and indexing issues as alternative explanations

Use [Debugging Search traffic drops](https://developers.google.com/search/docs/monitor-debug/debugging-search-traffic-drops). Separate verified changes, possible explanations, supporting evidence, and factors still to investigate. Overlapping timing supports correlation only. Preserve the meaning of null and unavailable data

## Prepare feedback

Follow the [ranking feedback guide](https://developers.google.com/search/docs/ranking/submit-feedback) to prepare:

- The relevant update identity and hashtag, preferring the identifier in the event notice
- Exact queries, country, language, affected URLs, and comparison URLs
- Performance snapshots, before-and-after data, timing, and impact scope
- A concrete explanation of how results affect users' access to useful information, including UK market effects when applicable

Label illustrative hashtags as examples; use the actual event notice for event details. Engineering teams aggregate feedback to investigate systemic issues. Individual URL manual ranking adjustments fall outside this mechanism

## Select the appropriate channel

Ranking-update feedback, manual-action reconsideration, copyright, SafeSearch, and regional dispute processes have their own conditions. Select the channel using the corresponding official feedback section and actual account status. Record scheduled dates and present availability for channels whose effective date is still in the future

Prepare a reviewable submission draft first. When the user has authorized submission, send it and read back the resulting status. Tool responses establish only the processing stage actually confirmed
