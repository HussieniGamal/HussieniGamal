# Portfolio review — 15 September 2026

## Recommendation
Feature Supply Chain, Repair & Return, and Pharmacy Sales on the profile. This is an editorial assessment of currently published evidence, not a hiring probability or a full validation of the underlying models.

| Project | General priority | Strongest application | Evidence available | Main limitation / next improvement |
|---|---|---|---|---|
| Supply Chain | 1 | Power BI, BI, operations analyst | PBIX, six dashboard images, DAX, data dictionary, insights | Snapshot without dates; document model grain, benchmark filter behavior and metric units |
| Repair & Return | 2 | BI, Power BI, operations reporting | Model and transformation diagrams, walkthrough, DAX examples, action plan | Presentation-only public package; no public data/PBIX for independent recalculation |
| Pharmacy Sales | 3 | Data Analyst, Python analytics, pharmacy analytics | Notebook, CSVs, requirements, charts, dictionary | Notebook has no saved outputs; improve execution evidence, period comparability and data-source attribution |
| HMC Hospital | 4 | Healthcare analyst, healthcare BI | PBIX, PDF and dashboard images | Define returning patients, case grain, period, dataset provenance; add extracted DAX and model documentation |
| Younes Store | 5 | Retail reporting, sales / receivables analytics | Screenshots with invoice, product, city and payment metrics | No PBIX or calculation code; specify currency, dates and outstanding vs overdue balance |
| Furniture Sales | 6 | Sales analyst, commercial reporting | Screenshots, insights, external Drive package link | No in-repo executable report; add period, metric definitions and evidence behind regional comparisons |
| Profile repository | Navigation | All three role families | Links to all six projects | Lead with three business cases; remove unsupported profitability claim and duplicate skill lists |

## Selection by role
| Application | Recommended order | Why |
|---|---|---|
| General Data Analyst | Pharmacy Sales → Supply Chain → Repair & Return | Code, exploratory analysis and operational decision support |
| BI Analyst | Repair & Return → Supply Chain → Pharmacy Sales | Process visibility, KPI interpretation and analytical breadth |
| Power BI | Supply Chain → Repair & Return → HMC | Inspectable PBIX and DAX, then operational modeling documentation |
| Healthcare / pharmacy | Pharmacy Sales → HMC → Supply Chain | Domain relevance backed by Python and dashboard work |
| Retail / commercial reporting | Younes Store → Furniture Sales → Supply Chain | Receivables, customer mix and inventory questions |

Suggested profile pin order: Supply Chain, Repair & Return, Pharmacy Sales, HMC, Younes Store, Furniture Sales. Pinning is a separate profile setting; these documentation changes do not alter pins.

## Changes prepared
- Replace the profile's long feature/tool lists with three concise cases and direct evidence links.
- Add a business-decision summary before the image galleries in every project.
- Separate dataset findings, proposed actions and measured business outcomes.
- Retain screenshots, existing supporting documentation and project files.
- Qualify Cairo market-size comparisons and doctor activity interpretations.
- Identify partial-year coverage in Python and snapshot limits in supply chain.
- Specify public reproducibility limits for screenshot-only projects.

## Highest-value evidence gaps
1. **SQL:** No SQL scripts were found in the seven inspected repository trees. Add a genuine SQL analysis to an existing dataset: joins, aggregations, window functions and validation queries tied to a business question. This is a future enhancement, not work demonstrated by these changes.
2. **Python execution:** All notebook code cells currently have null execution counts and empty outputs. Run in a clean environment, retain useful outputs and document results. Daily and hourly data should be analyzed at their own grain, not combined as independent sales.
3. **Time comparisons:** 2019 ends on 8 October. Compare equal periods or complete years before describing growth/decline. Review monthly category averages for incomplete months. Quantile bands divide observations into relative groups; they are not an anomaly detector.
4. **Supply chain logic:** SELECTEDVALUE assumes a unique stock/sales value per SKU. Document that assumption. Benchmark measures remove SKU filters but retain other filters; explain what the comparison population is. Confirm ties and blank values before presenting risk categories as complete classifications.
5. **Repair scope:** The displayed Total/Completed DAX filters project TSML3, whereas Upcoming in 30 Days does not show that filter or a completed-status exclusion. Check model/report context before comparing those measures. No measure changes are proposed without the underlying model.
6. **Definitions:** Document currency, reporting period, source and observation grain across sales and hospital projects. Returning-patient percentage should not be renamed readmission rate. A balance is not overdue without due dates.
7. **Outcome evidence:** If implemented, record baseline, intervention, timeframe and follow-up metric. Until then use “identified”, “flagged”, “analyzed” and “recommended”, rather than claiming savings or performance improvements.

## A recruiter-friendly case structure
1. Business question and intended decision-maker.
2. Two or three findings with units and reporting scope.
3. Recommended action and its expected benefit.
4. One representative analytical image.
5. Direct links to report, code, model and method.
6. Limitations and reproduction instructions.

## Review scope and validation
Reviewed all seven README files and repository trees, the Python notebook source and dictionary, and the supply-chain DAX document. Confirmed referenced local documentation/image paths against repository trees. The assessment does not include executing Python, opening or recalculating PBIX models, visual inspection of dashboard images, or verifying access to external Drive/portfolio pages. Numerical highlights are attributed to existing published documentation, not independently recalculated.

All changes are documentation-only drafts on separate branches. The underlying datasets, notebooks, measures and dashboards are unchanged.
