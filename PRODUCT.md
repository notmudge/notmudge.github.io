# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

Two audiences, weighted equally:

- **Hiring managers/recruiters** evaluating Alex Mudge for a data/insights/analytics-engineering/BI role. Success: they shortlist or reach out for an interview.
- **Freelance/contract clients** considering hiring Alex for pipeline, modelling, BI, or AI-rollout work. Success: an inbound project enquiry.

## Product Purpose

A personal portfolio site for Alex Mudge, a Data & Insights Lead based in Oxford, UK. It exists to demonstrate real, delivered data work — pipelines, dimensional models, reporting layers, data quality practice, and Copilot/AI rollout delivery — so either audience can quickly judge credibility and reach out.

## Positioning

Alex combines three things a typical data/BI candidate or consultant doesn't credibly hold together: data & insights delivery, data quality practice, and hands-on delivery of Copilot/AI rollouts. Most competing profiles are strong in one lane (pipeline engineering, or reporting, or AI enablement) — Alex's evidence spans data quality, analytics engineering, and applied AI rollout in a single track record.

## Operating Context

- Site is a static GitHub Pages deployment (Jekyll-based: `_layouts`, `_includes`, `_data`) at `https://notmudge.github.io/`.
- `index.html` is a short landing page with an embedded portfolio reel (video, in `hyperframes-portfolio-reel/`) and links through to `portfolio.html`.
- `portfolio.html` is the full portfolio: hero, about, skills, selected projects (with an architecture diagram), and a contact section. It supports dark/light theme toggling.
- Project data (`_data/projects.yml`, `_data/articles.yml`, `_data/videos.yml`) lists real, working repos: a weather data pipeline (Python/ADLS Gen2/Azure SQL/dbt/GitHub Actions), a sales data pipeline (Python/pandas/SQLite/Star Schema), a retail data warehouse (SQL/SCD Type 2/fiscal calendar), and a Spotify data warehouse (Power BI/DAX/Star Schema).
- Contact is via `mailto:alex@mudge.io`.

## Capabilities and Constraints

- Confirmed functionality: static multi-page site, embedded video reel, project/article/video data driven by YAML, theme toggle, no backend.
- No copilot/AI-rollout project evidence currently appears in `_data/*.yml` or on `portfolio.html` — the positioning above is confirmed by the user but not yet represented as visible portfolio content (case study, project entry, or bullet). Future work should surface this rather than only stating it in prose.
- Existing repo/CV content (project list, bio, claims) is confirmed accurate as-is; no overstatement constraints were raised.

## Brand Commitments

- Name: Alex Mudge / "notmudge" / domain-style wordmark "mudge.io".
- Location: Oxford, UK.
- Title in use: "Data & Insights Lead."
- Established visual language (see `hyperframes-portfolio-reel/DESIGN.md`): dark analytical canvas, precise cyan grid lines, terminal-inspired labels, Ubuntu / Ubuntu Mono typography, data-pipeline-diagram motifs. Explicitly avoid reading as generic tech-startup ad content.

## Evidence on Hand

- Real GitHub repos linked from `_data/projects.yml` (weather pipeline, sales pipeline, retail warehouse, Spotify warehouse) — genuine personal/practice projects, not disclosed as paid client work.
- Headshot/profile image at `/assets/images/me.jpeg`, currently reused as a placeholder for all project thumbnails/screenshots — real per-project screenshots are not yet on hand.
- No testimonials, case studies, or press currently exist; none should be fabricated.
- No dedicated Copilot/AI-rollout case study or repo exists yet despite it being part of confirmed positioning — treat as a gap, not evidence.

## Product Principles

1. Every claim ties to a real, inspectable artifact (a repo, a diagram, a working demo) — no invented proof.
2. Serve hiring managers and freelance clients as one audience, not two separate journeys, since both are evaluating the same evidence for different outcomes.
3. Lead with delivered breadth — data & insights, data quality, and applied AI/Copilot rollout — rather than defaulting to a single-lane "data engineer" or "BI developer" framing.
4. Keep the technical, credible, terminal/pipeline visual identity already established; new work should extend it, not soften it toward generic startup polish.
