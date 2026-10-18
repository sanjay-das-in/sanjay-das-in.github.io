# Sanjay Das — personal research website

Buildless HTML/CSS/JavaScript for GitHub Pages. Original blue/teal identity and section navigation are retained, with a full-width layout, natural scrolling, a larger About portrait, and larger type. The former sidebar information is preserved in the header and About profile links.

## Preview

Run `python3 -m http.server 8000` from this directory and open http://localhost:8000.

## Content and styling

- `index.html`: biography, research, 13 selected papers/preprints, education, experience, teaching, six supplied awards, news, service, and photography.
- `assets/modern.css`: portfolio layout and section-specific refinements.
- `blog/index.html`: notebook listing with five research notes and the existing photography post.
- `blog/<slug>/index.html`: standalone, directly linked research notes.
- `content/posts.json`: reference copy of the five notes; keep matching HTML in sync when editing.
- `assets/style.css`, `assets/notebook.css`: notebook and article styling.
- `assets/figures/*-paper.png`: original paper figures downloaded from arXiv; corresponding WebP files are smaller display copies.
- `assets/figures/sources.json`: figure sources, paper links, and credits. Figures in articles link to full-resolution originals.
- `resume_1page.pdf`, `profile.jpeg`, `photos/`: existing personal assets.

## Research sources

ResearchGate, OpenReview, ORNL, Google Scholar, Semantic Scholar, ORCID, DBLP, GitHub, and LinkedIn are linked directly. No profile scraping or live synchronization is used. Scholar was inaccessible during this update; new paper records were checked against original arXiv records instead. Existing venues come from the original repository; new additions are explicitly labeled preprints.

The six new award entries and dates were supplied by the site owner. No grant funding amounts or unsupported impact metrics were added.

## Verification

Checked desktop and mobile layouts with Firefox screenshots. Real-browser checks passed for tab switching, all six awards, all thirteen papers, title search, empty search results, accessible active sections, removal of the sidebar, and retention of all nine research/profile links. Local links, source JavaScript syntax, and assets were also checked.

Publication is managed through this repository’s GitHub Pages configuration. Pushing source changes does not by itself verify that a Pages deployment has completed.

## Expanded research notes

Each of the five research articles now includes roughly 250 words covering the motivation, method, findings, and limits. Read times are derived from the article text. Paper figures and attribution remain intact. The portfolio and notebook use layered blue/teal backgrounds with a static research-inspired line pattern; fixed empty panel height has been removed.

## News and certificates

`content/news.json` records the 16 updates rendered in the News tab. Keep the matching HTML in sync when editing. Category filters cover papers, awards, talks, and service. Certificate dates correct ORPEX to September 24, 2026, the ORPA poster award to May 6–7, 2026, and ISVLSI to July 5, 2022. The original certificate photographs must be saved using the filenames in `assets/awards/README.md` before their prepared gallery can display them.

## Consistency pass

Navigation uses equal-size cells with colorful SVG icons and matching section accents (`assets/consistency.css`). All ten section buttons and the Blog link share the same spacing. Dates, role wording, section headings, and paper links are normalized. Seven awards are recorded newest first in `content/awards.json`. The antenna-design paper now also appears in Publications, and ORCHID’s workshop status matches News. Degree wording follows the ORNL staff profile: Ph.D. in Computer Engineering. Browser checks covered all sections, selection state, tab geometry, paper search, News filters, and desktop/mobile layouts.

## Visitor statistics

Both MapMyVisitors widgets are isolated in the gray Statistics tab (`#statistics`). About and blog pages no longer contain visitor panels. Notebook/article navigation links to the Statistics tab. The two provider IDs are retained and the map statistics link is https://mapmyvisitors.com/web/1c8y8. Styling is in `assets/visitors.css`. Widgets initialize once when the Statistics tab is first opened, after its container becomes visible. The standalone blog pages no longer load tracking scripts. The map occupies the full content width, with equal-width globe and explanatory panels below.

Local previews (`file:`, localhost, and loopback addresses) do not execute visitor tracking widgets, preventing development checks from adding visits. Widget scripts are prefetched for faster opening on the live website. The compact Statistics view is side by side; the map text rows remain visible and the globe is enlarged.
