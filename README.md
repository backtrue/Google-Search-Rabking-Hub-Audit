# Google Search Ranking Hub Audit

A Codex skill for reviewing web pages, article drafts, and search performance evidence against Google's published Search guidance

The skill turns applicable guidance into findings with evidence, source links, suggested changes, and acceptance criteria. Its 39 checklist items cover search eligibility, content quality, page experience, spam policies, and AI search eligibility, with a separate workflow for ranking update analysis

Skill name: `audit-google-search-ranking`

## What you can use it for

- Review a live page for crawlability, indexing controls, content quality, and page experience
- Review an unpublished draft for reader value, factual support, sourcing, and relevant policy concerns
- Check AI search eligibility, visible content and structured data consistency, Search Console inclusion settings, and available AI impression data
- Investigate traffic changes using Search Console exports, service records, and confirmed Google update notices
- Recheck revised content against a previous audit's findings and acceptance criteria

The audit selects checks that apply to the supplied material. Draft reviews cover the content available; live indexing, performance, and account settings remain pending until the corresponding evidence is available

## Install in Codex

For a fresh installation, run these commands in a macOS or Linux shell with Git installed:

```bash
skill_root="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$skill_root"
git clone --depth 1 --branch main \
  https://github.com/backtrue/Google-Search-Rabking-Hub-Audit.git \
  "$skill_root/audit-google-search-ranking"
```

This places `SKILL.md`, `agents/`, and `references/` in `$CODEX_HOME/skills/audit-google-search-ranking`, using `~/.codex/skills` when `CODEX_HOME` is unset. The installation directory is named after the skill; the GitHub repository URL retains its original `Rabking` spelling

Start a new turn in Codex, then invoke `$audit-google-search-ranking` with a URL, file, or pasted content

For an installation created with Git, fetch later versions with:

```bash
git -C "${CODEX_HOME:-$HOME/.codex}/skills/audit-google-search-ranking" pull --ff-only
```

## What to provide

Provide the target URL, exact local file path, attached document, or complete draft text. Add the intended audience and page goal when available, such as public indexing, product comparison, or AI search eligibility

Live guidance checks require web access in the Codex session. Indexing, account settings, and performance findings use the relevant Search Console evidence, connected tools, or exports you provide. Missing data is recorded as pending verification, and available checks continue

The skill instructions, reference files, and interface labels are in English. The examples below explicitly request an English report

## Usage examples

Replace angle-bracket placeholders with your actual URLs, file paths, or update names

### Audit a live page

```text
Use $audit-google-search-ranking to audit <page-url>.
The page is intended to be publicly indexed and help readers choose a product.
Return the report in English with evidence, official sources, priorities,
and acceptance criteria for each finding.
```

### Review an article draft

```text
Use $audit-google-search-ranking to review <path-to-draft.md> for SEO and AEO.
The article has not been published yet.
Review its usefulness, claims, sources, and relevant policy concerns.
List deployment checks separately as pending verification.
Return the report in English.
```

### Check AI search eligibility

```text
Use $audit-google-search-ranking to check <page-url> for AI search eligibility.
Use the attached Search Console evidence for the property's effective
Search generative AI setting, including any inherited value.
Compare structured data with visible content and flag missing evidence.
Return the report in English.
```

### Investigate a traffic change

```text
Use $audit-google-search-ranking to analyze the attached Search Console export
and service records for <site-url> around <update-name>.
Verify the update's announcement, rollout, and completion status.
Separate observed changes, possible explanations, and evidence still needed.
Keep the data's original timezone and missing-value meanings.
Return the report in English.
```

### Recheck a revision

```text
Use $audit-google-search-ranking to recheck <revised-page-url-or-file>
against the attached previous audit.
Update each finding using the revised content and its acceptance criteria.
Return the report in English.
```

## What the report contains

The report begins with the audit date, scope, evidence obtained, and main findings, followed by:

1. An audit table with check IDs, applicable guidance, status, evidence locations, and official source links
2. A remediation and verification table with priorities, specific changes or evidence requests, reasons, limitations, and acceptance criteria

| Status | Meaning |
|---|---|
| Meets the check | Available evidence supports the applicable condition within the audited scope |
| Needs revision | A concrete issue is supported by evidence and applicable guidance |
| Pending verification | A conclusion needs more evidence, access, or clarification |
| Not applicable | The feature or condition falls outside the target's scope |

P0, P1, and P2 express remediation priority within the audit. Official requirements, policies, quality recommendations, system background, and the audit's own analysis are identified separately

Checks cover observable evidence. Search rankings and AI citations are assessed through actual results; internal ranking weights and system scores remain outside the evidence available to this skill

An audit request produces a report. When the same request also authorizes changes, the skill follows that scope and verifies the revised result; account changes, submissions, publishing, and deployment follow the authorization for those actions

## Checklist coverage

| Group | Items | Focus |
|---|---:|---|
| T — Technical eligibility and discovery | 6 | Access, HTTP responses, indexing controls, actual index status, descriptive text, and internal links |
| C — Content quality and trust | 7 | Reader tasks, original value, factual support, authorship, sensitive claims, clarity, and freshness |
| E — Page experience | 3 | Core Web Vitals, connection and mobile experience, and content accessibility |
| A — AI search eligibility and representation | 6 | Indexing and snippets, readable content, data consistency, citations, inclusion settings, and AI impressions |
| S — Spam policy investigation | 17 | Applicable spam behaviors and other grounds for demotion or removal |

Ranking update analysis additionally checks event stages, comparison periods, data quality, alternative explanations, and appropriate feedback channels

## Repository contents

```text
.
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── checklist.md
    ├── ranking-changes.md
    └── spam-policy.md
```

- [SKILL.md](SKILL.md) defines the audit workflow, evidence rules, statuses, and output format
- [Core checklist](references/checklist.md) contains technical, content, experience, and AI search checks
- [Spam policy checks](references/spam-policy.md) define investigation points and applicability conditions
- [Ranking changes](references/ranking-changes.md) covers update analysis, feedback preparation, and dispute routes
- [Codex interface metadata](agents/openai.yaml) provides the display name and default invocation prompt

The reference baseline is November 26, 2026. Each audit reads the relevant current official sections and records source changes or verification gaps. Official links are included alongside their corresponding checks, starting with the [Google Search Ranking Hub](https://developers.google.com/search/docs/ranking/)
