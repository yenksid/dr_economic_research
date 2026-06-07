# Slice 16I — GitHub Pages Assets/Data Path Hotfix v1

status=SLICE16I_GITHUB_PAGES_ASSETS_DATA_HOTFIX_CREATED
created_utc=2026-06-07T22:43:00.052868+00:00

## Problem

GitHub Pages publishes the `/docs` folder as the site root. Public data files were in repository-root `/data`, so page links to supporting CSVs returned 404. The homepage also linked to visuals but did not embed a chart preview.

## Fix

- Copied public CSVs into `docs/data/`.
- Added `docs/data/index.md`.
- Patched Spanish and English source pages to link to `../data/...`.
- Patched Spanish and English landing pages to link to the published data folder.
- Embedded visual thesis maps on both landing pages.
- Added project `baseurl` and site `url` to `docs/_config.yml`.

## Boundary preservation

No evidence was added.
No NOT_PROVEN claim was upgraded.
No REJECTED_BOUNDARY claim was changed.

## North Star

Spanish: Ni colapso. Ni comodidad. Una presión selectiva.

English: Not collapse. Not comfort. A selective squeeze.
