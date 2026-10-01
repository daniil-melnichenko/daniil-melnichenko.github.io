---
published: false
---

# Workshop acceptance news and vitae entry

## Context and plan

User requested a September 2026 homepage announcement for acceptance of
"Robust Many-Objective Molecular Design with Preference-Gated GFlowNets"
to the NeurIPS 2026 Workshop on AI for Drug Discovery, plus a vitae entry.
The homepage [[_pages/about.md]] has no News section. The vitae
[[_pages/cv.md]] lists three posters under Presentations and already uses
asterisks for equal contributions. No earlier progress logs or analysis
scripts exist in this project.

Add News below the homepage introduction; rename Presentations to Posters
and Workshops and prepend the accepted paper. Preserve the supplied author
order and mark Daniil Melnichenko and Seonghwan Seo as equal contributors.
Use September as the acceptance date, without assuming the workshop date.

## Verification criteria

- Homepage renders the exact title, venue, and September 2026 date.
- Vitae renders all five authors in order, with asterisks on the first two.
- Existing poster entries and the equal-contribution legend are preserved.
- Jekyll build succeeds and the progress log is excluded from publication.

## Execution and conclusion

Implemented both content changes as planned. Existing poster entries and
the equal-contribution legend remain intact. No analysis scripts were needed
for this content-only update.

Verification: `PATH="/Users/daniil/miniconda3/envs/apple/bin:$PATH" bundle exec
jekyll build --destination /tmp/daniil-site-workshop-preview` succeeded (exit
0). Inspected generated `index.html` and `cv/index.html`: the announcement,
section heading, paper, ordered authors, and equal-contribution markers
render correctly. This unpublished progress log is absent from the build.
`git diff --check` passed. The requested content is complete locally;
publication requires pushing the changes.
