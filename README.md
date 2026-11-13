# Farmbook source repository

This repository currently contains two distinct published Farmbook applications in separate output roots:

| Application | Source directory | Pages output directory | Custom domain |
|---|---|---|---|
| Farm Album | `site/` | `site/` | `fb.bucklerfamily.estate` |
| Farmbook 2 · Today | `site2/` | `site2/` | `fb2.bucklerfamily.estate` |

Both directories are built from this repository's `main` branch using the same validation script:

- Farm Album: `node check.mjs`, output `site`
- Farmbook 2: `node check.mjs site2`, output `site2`

## Current hosting

- Cloudflare Pages project `bucklerfamily-fb` serves `site/`.
- Cloudflare Pages project `bucklerfamily-fb2` serves `site2/`.
- Both projects use this repository as their source after the 13 November 2026 source handover. Their existing custom domains and output directories are distinct.

## Split boundary still outstanding

The two applications remain in one GitHub repository because the original split retained both roots together. If the one-repository-per-webapp rule is to be completed literally, Farmbook 2 should eventually be extracted to a dedicated `unclehowell/cedwyn-fb2` repository, with the Pages project then reconnected to that repository. Until then, do not delete either source directory or merge the two Pages projects.

## Source and safety rules

- `main` is the maintained app source.
- The obsolete mirror workflow is disabled; there must be no scheduled pull from `unclehowell/cedwyn` or `datro`.
- Do not replace attributed historical sources with unqualified narrative. Where records conflict, retain the conflicting dates and source descriptions until the evidence is resolved.
