# Value Creation Toolbox for Industrialization

Two live, team-editable cockpits, one per framework stage:

| Stage | Framework | Cockpit | File |
|---|---|---|---|
| Idea → Series A | VCF-FND-01 Idea-to-Company Toolbox | [Venture Foundation Cockpit](https://claude.ai/artifact/Ej1ep32QnTwEgSJvvccga9) | `venture-cockpit.html` |
| PoC → scale | VCF-IND-01 Pilot-to-Series Toolbox | [Portfolio Industrialization Cockpit](https://claude.ai/artifact/HXfnY8oU188JDzv2T9FWnR) | `portfolio-cockpit.html` |

A venture that passes G4 in the Venture Foundation Cockpit is added in Prove phase to the Portfolio Industrialization Cockpit.

## Venture Foundation Cockpit (`venture-cockpit.html`)

Same structure as the portfolio cockpit below, adapted to company foundation:
five phases (Explore → Validate → Found → Build → Traction), gates G1–G4,
founding model and investor stake per venture, business-unit sponsor,
runway and capital raised, sector-specific readiness dimensions and gate
must-haves, early KPIs from the sector playbook, and actions linked to the
framework's 36 tools. Data lives in the artifact's shared database
(collection `ventures`).

## Portfolio Industrialization Cockpit (`portfolio-cockpit.html`)

A live, team-editable tracker for portfolio companies, built on the
Pilot-to-Series Toolbox framework (VCF-IND-01): five phases (Prove → Pilot →
Industrialize → Launch → Scale), four gates (G1–G4), five sector lenses
(Energy & infrastructure, Deep tech, Asset management & circularity,
Autonomous & supply chain, AI).

Live page: https://claude.ai/artifact/HXfnY8oU188JDzv2T9FWnR

### Portfolio view
- Summary strip: companies tracked, on track / at risk / off track, gate decisions due within 90 days, open and overdue actions.
- Phase board: every company placed on the five-phase track, with readiness against its next gate, gate must-haves met, gate date, runway and overdue flags.
- Register table, sortable by phase, status, readiness gap, gate date or last update; filter by sector and search.
- Activity feed across the whole portfolio.

### Company view (adapt per company)
- Profile: name, sector, status (RAG), deal lead, next gate date, runway, current situation.
- Phase track: click to move the company to another phase (logged).
- TRL (1–9): set it from Company details or the TRL scale in the Phase section (both edit the same value, logged); checked against the TRL band the framework expects for the current phase and shown on the board and register.
- Readiness: 8 dimensions scored 1–5 against the framework's minimum for the next gate, radar chart, gap list pointing to framework tools, trend over time.
- Gate checklists: core criteria + the sector must-have + criteria the team adds for this company.
- KPIs: starts from the sector KPI set; edit names, units, baseline, target and direction, log readings by date, see trend and on/off target.
- Actions: owner, due date, linked framework tool, overdue highlighting.
- Activity log: every change and note, with who made it.

### How it runs
The file is a claude.ai Artifact page. It stores companies in the artifact's
shared database (`db` capability, collection `companies`, one document per
company) and updates live for everyone with the page open. Anyone with
Contributor or Editor access can edit; viewers get a read-only view.
To update the live page, republish this file to the same artifact URL.
