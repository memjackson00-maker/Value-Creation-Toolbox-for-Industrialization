# How readiness changes through the gates (Portfolio Industrialization Cockpit, rev B)

Readiness used to be the same eight dimensions at every gate, with only the minimum score rising.
The research below shows that mature frameworks do two different things at once:

1. **Some threads are assessed at every gate**, but the evidence asked for changes
   (the DoD MRL Deskbook scores all nine threads at every level and the lowest thread sets the level;
   TRL runs from bench to field).
2. **Some topics only belong to part of the journey.** They either have to be settled early
   (IP and data rights, interface definition, design freeze) or only become testable late
   (process capability at rate, service network, multi-market rollout).

The cockpit now uses 13 dimensions, with 8 to 11 active at each gate. Scores stay on one absolute
scale (1 not started … 5 proven at scale), so a score carries over while a dimension stays in play.

## The model

| Dimension | G1 PoC→Pilot | G2 Pilot→Industrialize | G3 Industrialize→Launch | G4 Launch→Scale | Scale review | Pattern |
|---|---|---|---|---|---|---|
| Technology & product maturity | 3 · TRL 4–6 in OEM context | 4 · TRL 7 in real operation | 4 · TRL 8, qualified design | 5 · TRL 9 in the field | 5 · next-gen roadmap | Every gate |
| IP, data rights & FTO | 3 · IP, data rights, first FTO screen | 3 · FTO for pilot markets, joint-IP terms | — | — | — | Until G2, then under Quality & compliance |
| Integration & interfaces | 2 · interfaces specified (IRL 1–3) | 3 · integrated in pilot (IRL 5–6) | 4 · verified, repeatable (IRL 7–8) | — | — | Until G3, then under Production & deployment |
| Design for manufacture | — | 3 · DfM review, production-intent design (EVT) | 4 · design frozen on production tools (DVT) | — | — | G2–G3, then change control |
| Production & deployment process | — | 2 · route defined, risks known (MRL 5–6) | 4 · pilot line or first standard sites (PVT, MRL 8) | 5 · run at rate, capable processes (MRL 9) | 5 · replicated to further sites (MRL 10) | From G2 |
| Supply chain & partners | — | 2 · critical suppliers and backups identified | 4 · contracts, supplier qualification, FAI | 4 · delivering at rate and quality | 5 · dual and regional sourcing | From G2 |
| Quality & compliance | 2 · rules mapped, export screening | 3 · compliance roadmap, pre-compliance tests | 4 · certified or homologated, VDA 6.3 / PPAP | 5 · field quality, 8D, post-market duties | 5 · new-market compliance | Every gate |
| Service & aftermarket readiness | — | — | 3 · service concept, warranty/SLA, parts plan | 4 · network trained, parts available | 5 · uptime and service revenue at target | From G3 |
| Commercial traction | 3 · value quantified, pilot funded | 3 · pilot KPIs met, LOI / conversion terms | 4 · year-1 volume contracted | 4 · repeat orders, retention | 5 · second brand / market won | Every gate |
| Unit economics & cost | 2 · value > cost hypothesis | 3 · target cost in agreed band (should-cost) | 4 · launch-volume cost quoted | 4 · positive contribution margin | 5 · cost-down delivering | Every gate |
| Funding & runway | 2 · pilot funded | 3 · industrialization funding | 4 · launch and working capital, ≥12 months | 4 · runway through ramp, path to break-even | 4 · growth or exit options | Every gate |
| Team & organization | 2 · founders, OEM sponsor, decision owners | 3 · industrialization lead | 3 · quality, supply-chain, plant/rollout roles | 4 · launch, service, customer success | 4 · professional management, board | Every gate |
| Scalability & next markets | — | — | — | 3 · second market qualified | 5 · multi-market rollout running | From G4 |

The minimum scores are starting assumptions for the team to review. Each company can still remove
dimensions that don't apply and add its own.

## What the research says, and how it shaped the model

**Persistent threads with changing evidence.** The DoD Manufacturing Readiness Level Deskbook assesses nine
threads (technology and industrial base, design, cost and funding, materials, process capability and control,
quality management, workforce, facilities, manufacturing management) at every level, and the lowest thread sets
the overall level. What each level must show changes: MRL 6 (around Milestone B) needs production-relevant
prototypes, supply-chain and supplier-quality assessments and long-lead plans; MRL 8 (LRIP entry) needs a stable
design and materials, tooling, test equipment and facilities proven on a pilot line, with supplier qualification
and first-article inspection complete; MRL 9 focuses on quality, throughput and rate for full-rate production.
This is why technology, quality, commercial, cost, funding and team stay in at every gate, and why production
and supply chain enter at G2 and peak at G3–G4.

**Hardware build stages.** EVT, DVT and PVT practice separates what is being proven: EVT proves one
production-intent design, DVT freezes the design on production parts and tools, and PVT tests the factory rather
than the product, aiming for mass-production yield and process capability (commonly Cpk ≥ 1.33 on critical
dimensions; yield figures vary by company). This is why Design for manufacture is assessed at G2 (EVT) and G3
(DVT) and then dropped, and why Production moves from "route defined" to "proven on a pilot line" to "run at rate".

**Automotive gates.** VDA Maturity Level Assurance for new parts runs eight maturity levels from innovation
release to handover to series, including supply-chain definition and award, release of technical specifications,
completed production planning, parts from series tools and product and process approval. APQP runs from planning
through product and process design to validation and launch with feedback, ending in PPAP before shipments.
Launch-readiness practice adds spare-parts availability, a tested warranty process and early warranty and
field-quality tracking. This is why Service & aftermarket enters at G3 and Quality shifts to field quality and
post-market duties at G4.

**Integration.** Integration readiness levels (Sauser et al.) rate the maturity of the connections between
technologies, from an identified interface (IRL 1) to an integration verified in the system environment (IRL 8)
and proven in operation (IRL 9). System readiness depends on both TRL and IRL. For trucks, depots, plants, TMS and
IT systems the interfaces are often the main risk, so Integration is its own dimension until G3.

**Machine learning.** MLTRL (Lavin et al., Nature Communications 2022) treats proof of concept, productization,
systems integration and deployment with monitoring as distinct levels, and a system's level is set by its least
mature component. This supports the same pattern for AI companies: integration and product architecture early,
monitoring and post-deployment duties later.

**Regulation that only bites at certain gates.** UN R155 requires a certified cybersecurity management system
before vehicle type approval and continues into post-production monitoring; suppliers must evidence their part.
EU Regulation 2022/1426 covers ADS type approval, including functional and operational safety, cybersecurity and
data requirements. This is why Quality & compliance moves from mapping (G1) to certification (G3) to post-market
monitoring (G4).

**Commercial and innovation readiness.** The KTH Innovation Readiness Level scores customer, technology, business
model, IP, team and funding separately, each on its own 1–9 path. ARENA's Commercial Readiness Index adds
regulatory environment, stakeholder acceptance, technical and financial performance, supply chain and skills, and
market opportunities, running from a hypothetical commercial proposition to a bankable asset class. Both support
keeping commercial, business-model (unit economics), IP, team and funding as separate dimensions, and having the
commercial bar move from willingness to pay to contracts, repeat orders and new markets.

**Why startups fail in scale-up.** A study of 14 hardware start-ups and 7 production experts (Sefton, Rönkkö and
Bellgran, 2020) groups scale-up challenges into financing, market analysis and feasibility, production competence
and team building, prototype development, production process understanding, suppliers and manufacturers, and
support from the innovation system. That supports keeping Team (production competence) and Supply chain explicit
from G2, before the company commits to tooling.

**Stage-gate practice.** Stage-gate guidance tightens financial criteria at later gates as commitments grow,
while must-meet criteria such as strategic fit apply throughout. That is reflected in Unit economics moving from a
hypothesis to quoted cost and real margin.

## Sources

- DoD Manufacturing Readiness Level Deskbook, 2025 edition — https://firebasestorage.googleapis.com/v0/b/manufacturing-readiness-levels.firebasestorage.app/o/MRL%20Deskbook%20V2025%20July%20Final.pdf?alt=media&amp=&token=8f77f199-42f5-488f-a3bf-28fbfde58270
- DoD MRL Deskbook 2022 — https://firebasestorage.googleapis.com/v0/b/manufacturing-readiness-levels.firebasestorage.app/o/MRL_Deskbook_2022_Final.pdf?alt=media&amp=&token=cf45fd7d-171a-45be-becd-360608258ab1
- DoD MRL and TRL definitions — https://at.dod.mil/Portals/129/Atch%202_MRL_TRL_Definitions.pdf
- MRL Deskbook v2.4 (2015) — https://www.acqnotes.com/wp-content/uploads/2014/09/Manufacturing-Readiness-Level-Deskbook-v2.4-Aug-15.pdf
- NDIA briefing on MRL threads — https://ndia.dtic.mil/wp-content/uploads/2011/system/12956_ChristianWednesday.pdf
- VDA QMC, Reifegradabsicherung für Neuteile (Maturity Level Assurance) — https://webshop.vda.de/qmc/de/reifegradabsicherung-f%C3%BCr-neuteile-2-auflage
- VDA QMC, Maturity Level Assurance 06/2022 — https://webshop.vda.de/QMC/en/maturity-level-assurance_062022
- APQP phases overview — https://www.net-inspect.com/blog/5-apqp-phases/
- EVT / DVT / PVT — https://instrumental.com/wp-content/uploads/2020/10/EVT-DVT-PVT-Whitepaper.pdf and https://embeddedartistry.com/fieldmanual-terms/production-validation-and-test/
- Sauser et al., system and integration readiness — https://ndia.dtic.mil/wp-content/uploads/2006/systems/Thursday/sauser.pdf and https://www.dair.nps.edu/bitstream/123456789/106/1/NPS-AM-08-060.pdf
- Lavin et al., Technology readiness levels for machine learning systems (Nature Communications, 2022) — https://www.nature.com/articles/s41467-022-33128-9
- KTH Innovation Readiness Level — https://www.inside.dtu.dk/en/research/commercialisation-and-patenting/patents-and-software/kth-innovation-readiness-level
- ARENA, Commercial Readiness Index for Renewable Energy Sectors (2014) — https://arena.gov.au/assets/2014/02/Commercial-Readiness-Index.pdf
- Sefton, Rönkkö, Bellgran, Hardware start-ups in the scale-up process of production (2020) — https://ebooks.iospress.nl/doi/10.3233/ATDE200175
- Hardware start-ups and manufacturing innovation (2023) — https://www.tandfonline.com/doi/full/10.1080/21693277.2023.2246537
- UN R155 / ISO/SAE 21434 overview — https://www.certivo.com/frameworks/un-r155-r156-vehicle-cybersecurity-compliance
- EU Regulation 2022/1426 overview — https://incompliancemag.com/eu-commission-issues-rules-for-automated-driving-systems/
- Launch-readiness criteria (practitioner) — https://resources.skill-lync.com/branches/automobile-engineering/questions/manufacturing-auto/launch-readiness-assessment
- Stage-gate criteria (secondary summary) — https://resources.rework.com/libraries/project-management/stage-gate-process

Limits: the research was done through web search summaries; several primary documents (the VDA band, the AIAG
manuals, the full MRL sub-thread matrix) are paid or could not be opened from this environment. Thresholds such
as Cpk ≥ 1.33 and the minimum scores are common practice, not mandated values.
