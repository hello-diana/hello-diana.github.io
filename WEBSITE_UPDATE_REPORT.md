# Website Update Report — Yiyang "Diana" Wang

Date: 2026-06-19. Hugo Blox / Hugo Academic site. Theme, modules, layouts, and deployment
workflow were preserved; all changes are in `content/`, `config/_default/`, `assets/`, and
`static/`.

## 1. Summary of changes

- **Profile / homepage**: fixed the malformed email to a working `mailto:` link, rewrote the
  bio and "My Research" statement (human-AI interaction, LLM agents, multi-agent systems,
  multimodal sensing, ubiquitous computing), updated role to "Ph.D. Student in Computer
  Science", refreshed research interests, education (Uncommon Sense Lab & Ka Moamoa Lab under
  Prof. Alexander T. Adams and Prof. Josiah Hester), experience (surfaced the Graduate Research
  Assistant role first), and awards. Removed the Hugo Blox demo CTA card and reordered sections
  (bio → research → featured projects → selected publications → experience → awards → news).
- **Navigation**: removed the dead "Talks" link; menu is now Bio · Research · Publications ·
  Experience · Teaching · News · CV (Sep. 2025), all pointing to real destinations.
- **Projects**: deleted the three Hugo demo projects (PyTorch, pandas, scikit-learn) and added
  6 real research projects.
- **Teaching**: deleted the "Learn Python"/"Learn JavaScript" tutorial demos and added 4 real
  courses from the CV.
- **News**: removed Hugo template filler from 6 existing posts and added 8 concise, dated news
  items for recent milestones.
- **Publications**: merged 6 duplicate folders down to single canonical entries, created 5 new
  2025/2026 entries, normalized metadata, and added paper-figure thumbnails to 11 of 13 entries.
- **SEO**: updated the site description.
- **Hygiene**: removed `.DS_Store`/demo media files; added a CV PDF under `static/uploads/`.

## 2. Build & validation

- Hugo version: `0.148.2+extended` (matches the pinned `netlify.toml` / workflow version).
- Commands run:
  - `hugo --gc --minify` → **success**, 150 pages, 131 processed images, no errors/warnings.
- Validation: built site served locally and inspected with headless Chrome at desktop (1440px)
  and mobile (390px). Checked homepage, `/publication/` (both pages), 5+ individual publication
  pages, `/project/`, `/teaching/`, mobile nav, and dark/light mode. Email link, CV link, and
  all nav targets resolve. Screenshots saved (not committed) under `/tmp/diana-review/`.

## 3. Publication inventory (13 canonical entries)

| Slug | Title | Source | Featured image |
|---|---|---|---|
| `mascot` | MASCOT: Towards Multi-Agent Socio-Collaborative Companion Systems | arXiv 2601.14230 | Fig. 2, p.3 (framework overview) |
| `companioncast` | CompanionCast: Toward Social Collaboration with Multi-Agent Systems in Shared Experiences | arXiv 2512.10918 · CHI 2026 Workshop | Fig. 1, p.1 (system workflow) |
| `cultivagents` | CultivAgents: Cultivating Relationship-Centered Multi-Agent Systems for Personalized Gardening | arXiv 2605.23193 | Fig. 1, p.1 (system overview) |
| `unisd` | UniSD: Towards a Unified Self-Distillation Framework for Large Language Models | arXiv 2605.06597 | Fig. 1, p.2 (framework overview) |
| `textreg` | TextReg: Mitigating Prompt Distributional Overfitting via Regularized Text-Space Optimization | arXiv 2605.21318 | Fig. 2, p.5 (method pipeline) |
| `jin-scito-2-m-2024` | Scito2M (a.k.a. SciEvo): A 2M, 30-Year Cross-disciplinary Dataset | arXiv 2410.09510 · Good Data @ AAAI 2025 (Best Paper) | Fig. 1, p.2 (keyword trajectories) |
| `emnlp24_agentreview` | AgentReview: Exploring Peer Review Dynamics with LLM Agents | arXiv 2406.12708 · EMNLP 2024 Main (Oral) | Fig. 1, p.2 (framework overview) |
| `wang-puff-em-ecigarette-sleeve-2025` | PuffEM: An E-cigarette Sleeve for Estimating User Nicotine Intake | DOI 10.1145/3721201.3721393 · CHASE 2025 | none (paywalled, no open PDF) |
| `huang-eliciting-design-guidelines-2025` | Eliciting Design Guidelines of Paper-Based Tactile Interfaces for Eyes-Free Scenarios | DOI 10.1145/3689050.3704930 · TEI 2025 | none (paywalled, no open PDF) |
| `goel-phantom-puffs-phantom` | Phantom Puffs: A Phantom Lung to Emulate Smoking Behavior | DOI 10.33552/OJRAT.2024.03.000557 | Fig. 1, p.2 (labeled phantom lung) |
| `zhang-flexible-computational-photodetectors-2022` | Flexible Computational Photodetectors for Self-Powered Activity Sensing | DOI 10.1038/s41528-022-00137-z | Fig. 1, p.2 (principle & design) |
| `zhang-optosense-2020` | OptoSense: Towards Ubiquitous Self-Powered Ambient Light Sensing Surfaces | DOI 10.1145/3411826 · IMWUT Distinguished Paper | Fig. 3, p.7 (hardware design) |
| `guo-lx-2343-2017` | LX2343 alleviates cognitive impairments in AD model rats… | DOI 10.1038/aps.2016.128 | Fig. 1, p.5 (structure + viability) |

All featured publications: MASCOT, CompanionCast, CultivAgents, UniSD, PuffEM, AgentReview.
Each publication uses `admin` for Diana so her name is highlighted; PuffEM marks Wang & Goel as
equal contributors (per the CV). Figure crops are noted on each page as "adapted from" the paper.

## 4. Duplicate folders removed / merged

| Removed folder | Merged into |
|---|---|
| `goel-phantom-nodate` | `goel-phantom-puffs-phantom` |
| `guo-lx-2343-alleviates-cognitive-2017` | `guo-lx-2343-2017` |
| `jin-scito-2-m-2-million-2024` | `jin-scito-2-m-2024` |
| `aaai25_workshop_scievo` (SciEvo dup) | `jin-scito-2-m-2024` |
| `zhang-flexible-2022` | `zhang-flexible-computational-photodetectors-2022` |
| `zhang-opto-sense-ubiquitous-self-powered-2020` | `zhang-optosense-2020` |

## 5. Projects (6) and Teaching (4)

- Projects: MASCOT, CompanionCast, CultivAgents, AgentReview (featured on homepage), plus
  PuffEM and UniSD (on the Projects page).
- Teaching: CS 8801 Designing and Building User Interfaces, CS 1301 Intro to Computing,
  CS 8803 Health Sensing and Interventions, CS 1331 Intro to Object-Oriented Programming.

## 6. Notes on tooling

- `python/` and `docs/` are git-ignored and were **not** executed; some scripts there reference
  another researcher ("Yiqiao Jin"). Figure extraction used a small purpose-built script
  (`/tmp/diana-figures/figtool.py`, PyMuPDF) with manual figure selection per paper. No paper
  PDFs were committed; pages link to the official external PDFs.

See `UNVERIFIED_ITEMS.md` for items needing owner confirmation.
