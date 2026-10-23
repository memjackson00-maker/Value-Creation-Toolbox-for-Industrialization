# Sector-specific readiness and gate criteria (Portfolio Industrialization Cockpit, rev C)

Rev B made readiness change by gate. Rev C makes it change by sector as well, while keeping the overlap:

- **Shared dimensions** (technology, quality & compliance, commercial, unit economics, funding, team, production,
  supply chain, service, integration, IP, design for manufacture, next markets) apply to every sector. Their
  **minimum scores are the same**, so companies stay comparable across the portfolio.
- What each shared dimension **must show at each gate** is written per sector. Example, Commercial traction at G3:
  energy "contracted volume or site pipeline covers 12 months"; deep tech "first series nomination or supply
  agreement signed"; circularity "offtake and channel agreements cover planned output"; autonomy "lanes or sites
  contracted for year 1"; AI "paid contracts for year 1 signed".
- Each sector can **add** dimensions only it needs, and **switch off** shared ones that don't fit.
- **Gate criteria**: the core criteria apply to every company; each sector now adds 3–4 criteria per gate
  (Must or Should) instead of one.

## What is specific to each sector

| Sector | Added dimension | Switched off | Evidence that changes most | Sector gate criteria (examples) |
|---|---|---|---|---|
| Energy & infrastructure | Grid connection & sites (every gate) | — | UN 38.3 → UN R100 rev. 3 incl. thermal propagation or IEC 61851 / ISO 15118-20 charger conformity; CCS/MCS and OCPP interoperability; Battery Regulation passport (18 Feb 2027) and due diligence (18 Aug 2027); utilization and lender-grade data | G1 grid route checked · G2 interoperability with two truck brands and OCPP backend · G3 grid connections and permits for year-1 sites, passport and due-diligence data flows, asset-financing route · G4 uptime and utilization at business-case level |
| Deep tech | Physics & scale-up risk (G1–G3) | — | Effect reproduced outside the lab (TRL 4–5) → TRL 6 in a truck or plant → automotive qualification on scale-up-line parts; tech transfer to CDMO/foundry/tier-1 (MRL 4–5 → 8 → 9); EU dual-use classification; IATF 16949 at the production site; funding the pilot-to-commercial gap | G1 effect reproduced, export-control classification · G2 TRL 6 in a host environment, non-dilutive scale-up funding · G3 process frozen and transferred, PPAP/IATF · G4 field ppm and yield stable, second application |
| Asset management & circularity | Environmental impact & claims (every gate) | Design for manufacture | Grading/condition model on real feedstock → repeatable grading standard; feedstock and offtake under contract; waste, storage and ADR transport rules for damaged batteries; Battery Regulation repurposing duties (same safety requirements as new, state-of-health evaluation); End-of-Life Vehicles Regulation 2026/1738 | G1 value loss quantified (€ and CO₂e) · G2 offtaker confirmed, LCA to ISO 14040/44 · G3 grading standard and second-life safety, approved reverse logistics · G4 recovery rate and margin at plan, ready for ELV duties |
| Autonomous & supply chain | — (safety case carried by Quality & compliance; remote supervision by Service) | — | ODD defined → supervised pilot with falling interventions → safety case accepted (ISO 26262, ISO 21448, UL 4600 structure) and approval granted (EU ADS 2022/1426 or national level-4 law, e.g. German AFGBV: KBA permit, approved operating area, technical supervision; Machinery Regulation from 20 Jan 2027 for yard robots) → in-service monitoring | G1 ODD tested · G2 safety case and hazard analysis · G3 technical supervision staffed, cybersecurity and software-update processes · G4 in-service monitoring for 3 months, insurance and liability |
| AI | — (MLOps carried by Production; data rights by IP) | — | Beats current process offline → holds in shadow mode → production release with MLOps (monitoring, rollback, retraining) → drift handled in production; TISAX level (often AL2/AL3), DPIA, EU Data Act; AI Act high-risk duties from 2 Dec 2027 (Annex III) or 2 Aug 2028 (products) | G1 model beats current process · G2 integration and hosting agreed with group IT, DPIA · G3 monitoring, rollback and retraining tested, SLA · G4 performance stable for 3 months, cost per inference in band |

The full per-gate text is in `SEC_R` (readiness evidence) and `SGATES` (gate criteria) in `portfolio-cockpit.html`.

## Notes on how ticks carry over

The first sector criterion per gate keeps its original key (`G1-sx-<sector>`), so existing ticks stay. New sector
criteria use `G1-sx-<sector>-<n>`. Removing or restoring criteria per company works for sector criteria too.
When a company's sector changes, its sector criteria and readiness evidence switch to the new sector; scores on
shared dimensions are kept.

## Sources

Energy & infrastructure
- EU Battery Regulation timelines — https://www.automotive-iq.com/electrics-electronics/articles/eu-battery-passport-explained-requirements-timeline-and-compliance-steps-to-2027 · https://dpp-tool.com/en/guide/eu-battery-regulation/ · https://www.tuv.com/landingpage/en/eu-new-battery-regulation-eu-2023-1542/
- UN R100 rev. 3 and thermal propagation — https://incompliancemag.com/testing-to-unece-regulation-100-requirements-for-electric-vehicle-batteries/ · https://www.tuvsud.com/en-us/industries/mobility-and-automotive/automotive-and-oem/automotive-testing-solutions/battery-testing/un-ece-r100
- MCS, IEC TS 63379, SAE J3271, ISO 15118-20 — https://en.wikipedia.org/wiki/Megawatt_Charging_System · https://vacleancities.org/sae-j3271-megawatt-charging-system-mcs-standard/
- Charging project finance and bankability — https://wholesale.banking.societegenerale.com/en/news-insights/clients-successes/clients-successes-details/news/accelerating-heavy-transport-electrification/ · https://txfnews.com/articles/7227/EV-Charging-A-question-of-bankability · https://www.morganlewis.com/-/media/files/publication/outside-publication/article/2026/locations-permits-and-power-are-key-in-ev-charger-projects-law360.pdf

Deep tech
- EU dual-use Regulation 2021/821 — https://eur-lex.europa.eu/EN/legal-content/summary/dual-use-export-controls.html · https://www.thetradehub.eu/en/customs/export-control/annex-i
- IATF 16949 and PPAP for new suppliers — https://en.wikipedia.org/wiki/IATF_16949 · https://flex.com/downloads/supplier-quality-requirements-automotive
- Deep-tech scale-up financing gap — https://documents1.worldbank.org/curated/en/994721636125287177/pdf/Financing-Deep-Tech.pdf · https://www.frankfurt-school.de/cms/dam/events/CfET-Events/2026-Private-Capital-Symposium/Day-1/CfET_1st-Private-Capital-Symposium_10_Key_Insights-2026.pdf

Asset management & circularity
- Battery Regulation repurposing and second life — https://www.sciencedirect.com/science/article/pii/S2950264025000802 · https://cdn.ceps.eu/2026/05/2026-05-ERCC-second-life-batteries-applications.pdf · https://www.cencenelec.eu/news-events/news/2025/brief-news/2025-09-16-ev_batteries_secondlife/
- Transport of damaged lithium batteries (BAM, ADR P908/P911) — https://tes.bam.de/fileadmin/TES/DE/Downloads/ggr-024_allgemeinverfuegung.pdf · https://umwelt-online.de/recht/gefahr.gut/tec_reg/bam/ggr024_06_24.htm
- End-of-Life Vehicles Regulation 2026/1738 — https://public.cdxsystem.com/web/cdx/w/eu-elv-regulation-officially-published-what-changed-since-council-adoption · https://www.automotivelogistics.media/sustainability/eu-end-of-life-vehicles-regulation-enters-into-force/2724484

Autonomous & supply chain
- UL 4600 and companion standards — https://www.ul.com/news/ul-4600-edition-3-updates-incorporate-autonomous-trucking · https://ulse.org/insight/safety-questions-autonomous-truck-companies-answer-before-deployment/
- EU ADS Regulation 2022/1426 — https://incompliancemag.com/eu-commission-issues-rules-for-automated-driving-systems/
- German AFGBV (level-4 operating permit and operating area) — https://www.gesetze-im-internet.de/afgbv/__4.html · https://www.gesetze-im-internet.de/afgbv/__9.html
- Machinery Regulation 2023/1230 and ISO 3691-4 — https://www.tuev-nord.de/en/services/audit-and-expertise/product-certification/maschinenverordnung/ · https://go.tuv.com/iso-3691-4-standard-for-agvs-wp
- UN R155 cybersecurity — https://www.certivo.com/frameworks/un-r155-r156-vehicle-cybersecurity-compliance

AI
- EU AI Act after the Digital Omnibus — https://www.orrick.com/en/Insights/2026/07/EU-AI-Act-Update-Digital-Omnibus-Finalizes-8-Compliance-Changes · https://www.technology.org/2026/10/13/eu-ai-act-deadlines-after-the-digital-omnibus-what-applies-from-december-2026-to-august-2028/
- TISAX levels — https://www.docusnap.com/en/it-documentation/tisax-label-level · https://www.bsigroup.com/siteassets/pdf/en/insights-and-media/insights/brochures/tisax_client_guide_feb25.pdf
- EU Data Act and vehicle data — https://www.mayerbrown.com/ja/insights/publications/2025/11/the-eu-data-act-has-taken-effect-focus-on-automotive-and-cloud-providers
- MLOps maturity and ML TRLs — https://learn.microsoft.com/it-it/azure/architecture/example-scenario/mlops/mlops-maturity-model · https://www.nature.com/articles/s41467-022-33128-9

Limits: research ran through web search summaries (direct page fetches are blocked in this environment). Several
dates depend on delegated acts or pending amendments (Battery Regulation carbon footprint and recycled content,
AI Act standards, ELV application dates). Check them with Legal and Compliance before a gate decision.
