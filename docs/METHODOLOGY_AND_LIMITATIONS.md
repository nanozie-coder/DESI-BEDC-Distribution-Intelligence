# Methodology and analytical limitations

## Scope

- **Source:** Public NERC monthly BEDC estimated-billing energy-cap publications, October and November 2026.
- **Extract:** Delta and Edo State publication records.
- **Analytical coverage:** 21 reporting business units and 240 distinct feeder identities after reconciliation.
- **Unit of analysis:** Publication source row, feeder identity, service-band classification or feeder-band cap group, depending on the measure.
- **Period definition:** The November 2026 cap publication identifies **October 2026 as the consumption reference month**.

## Workflow

1. Collect and preserve the official publication and reporting-period metadata.
2. Extract and standardise state, business unit, feeder name, service band and published cap (kWh).
3. Reconcile ingestion counts against the actual publication **before** trend calculation.
4. Match normalised feeder identities across reporting months.
5. Compare reported service bands and business-unit coverage.
6. Classify duplicate cap groups with inconsistent values as requiring review.
7. Display results through FCI, SBTI, EDI and FECI Power BI pages.

## November 2026 composition

| State | Band A | Band B | Band C | Band D | Band E | Total |
|---|---:|---:|---:|---:|---:|---:|
| Delta | 12 | 15 | 36 | 27 | 38 | **128** |
| Edo | 5 | 20 | 38 | 31 | 18 | **112** |
| **Total** | **17** | **35** | **74** | **58** | **56** | **240** |

A state-specific service-band percentage equals that state's service-band count divided by that state's total distinct published feeder identities.

## Boundaries and cautions

- The extract does **not** establish all BEDC network assets, customers, or operating geography.
- Classification changes in public records do **not** directly measure changes in supply hours.
- Monthly estimated-billing energy caps are **not** actual energy delivered, consumed, lost, or sold.
- Conflicting published cap values flag source-data inconsistency; they are **not** proof of customer overbilling or regulatory noncompliance.
- No BEDC internal operational, customer billing, smart-meter, outage, or feeder telemetry systems are connected to this public-source prototype.
- Revenue uplift, reduced losses, measured consumer benefits, and integration feasibility remain **unverified**.
- Future publisher amendments or better source parsing may change the findings.

## Reproducibility status

The methodology and summary arithmetic are documented. The full SQL implementation, underlying raw extracts and Power BI binary are withheld from the public repository pending completeness, portability, provenance, licensing and security review. This is a documented **portfolio proof of concept**, not a packaged production system.
