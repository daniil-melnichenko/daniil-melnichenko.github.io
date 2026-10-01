---
published: false
---

# Compact vitae spacing and education row

## Context and plan

Following [[docs/progress/261001_vitae_cleanup.md]], the user finds the CV
too spacious and requested education in a row. In [[_sass/_cv.scss]],
section gaps are 2.75em and entry gaps are 1.6em.

Reduce those gaps to 1.8em and 1.1em, tighten heading/navigation spacing,
and place three degrees in a three-column grid at widths of at least 768px.
Keep education stacked on smaller screens. Show the shared institution once
above the grid, preserving degrees, years, honors, and advisor. Verify
Jekyll compilation and generated content/styles.

## Execution and verification

Implemented the compact spacing and responsive education grid in
[[_pages/cv.md]] and [[_sass/_cv.scss]]. Jekyll build passed using the existing
conda Ruby environment, with output `/tmp/daniil-site-vitae-preview`.
Generated HTML checks confirm all three degrees, years, both honors, advisor,
and shared institution. Compiled CSS checks confirm the stacked default,
three-column layout at 768px, and reduced section/entry gaps. The progress
log is excluded from publication, and `git diff --check` passed.
Visual rendering was not verified; browser preview was unavailable in the
earlier session. Changes are local and uncommitted.

## Follow-up: compact research experience

User also requested optimizing Research Experience. Group its four roles
under three workplaces, sharing repeated institution/location/supervisor
details for the two Young Lab roles. Align each role with its date range
on wide screens and stack these on mobile. Preserve all roles, date ranges,
locations, supervisors, and external links. Verify built HTML and CSS.

Completed: three workplace groups now contain all four roles, with dates
aligned beside role names and a mobile stack below 600px. Jekyll build and
HTML/CSS checks passed: exact role/date pairs, both supervisors, locations,
three workplace links, and the education grid are preserved. The Young Lab
name is shown once. `git diff --check` passed. Visual rendering remains
unverified; changes are local and uncommitted.
