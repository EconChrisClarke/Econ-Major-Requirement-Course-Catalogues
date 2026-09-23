# Econ Major Requirement & Course Catalogue Research

An interactive chart tracking how **ECONS 101/102** shows up in the degree requirements of every Washington State University bachelor's major, for every catalog year **2013–2025** — merged with a second research pass on what fills the UCORE Social Science [SSCI] slot for majors that don't use econs at all.

**[Open the chart](./index.html)** (or enable GitHub Pages on this repo to view it at a shareable URL).

## What this is

Each major/option is sorted into one of six categories, weighted by actual bachelor's degrees awarded that year (NCES IPEDS Completions data), not just by major count:

**Econ categories**
1. Requires both ECONS 101 & 102 — no substitution
2. Requires one ECONS course (or an explicit 101-or-102 choice) — mandatory either way
3. Lists econ as one option among several UCORE electives, or only recommends it

**No-Econ categories**
4. Requires a different, specific non-econ Social Science course instead
5. Mixed — some options/tracks in the major require a specific course (sometimes even econ itself, in just one track), others leave the slot open
6. No course named for the slot — genuinely open

An outer ring groups the six into a binary **Econ vs. No Econ** split.

## Methodology

- Every year 2014–2024 (2013 and 2025 researched in an earlier pass) got the same full major-by-major catalog research — roughly 90 majors/options checked per year against the actual printed WSU catalog (rendered PDF pages plus `pdftotext -layout` extraction), across 77 research passes. Not an interpolation or change-detection shortcut.
- Sizes are annual bachelor's degrees awarded, from NCES IPEDS Completions data matched to each major via its CIP code (a handful of majors' CIP classification drifts between adjacent codes across years — e.g. Economics reported under 45.0601 in most years but 45.0603 in others — both are summed for those majors). A major with no matched size data is excluded from that year's percentages, not counted as zero.
- Some majors split across categories by option/track (e.g. Mathematics & Statistics: Actuarial Science requires ECONS 101 & 102 flatly, while Applied/Theoretical Math and Statistics leave the slot open, and Secondary Teaching requires PSYCH 105) — these are coded **Mixed** rather than forced into one bucket.
- Two corrections caught during re-research: the 2016 Carson College of Business majors were initially misread as requiring only one econ course (the schedule actually lists ECONS 101/102 as two separate first-year term slots); and the Murrow College cluster's treatment of COM 101 required a judgment call, documented on the chart itself and resolved by the year COM 101 first carries a catalog [SSCI] tag (2015) rather than by year alone.
- The Murrow College's eight sub-tracks (Strategic Communication ×4, Journalism & Media Production ×4) are collapsed into one combined row each year to avoid one college's internal restructuring from swinging the chart.

Full methodology notes, including the source citations for every judgment call, are in the chart itself (see "Methodology & notes on data quality").

## Files

- `index.html` — the interactive chart (self-contained; open directly in a browser, or serve via GitHub Pages)
- `data/data.json` — the underlying dataset (per-year category totals, percentages, and the full major-by-major breakdown), same JSON embedded in the chart

## Sources

- WSU General Catalog PDFs, 2013–2025 (Schedule of Studies per major, and Description of Courses for UCORE tags)
- NCES IPEDS Completions data (CIP-code-matched bachelor's degrees awarded per major, per year)
