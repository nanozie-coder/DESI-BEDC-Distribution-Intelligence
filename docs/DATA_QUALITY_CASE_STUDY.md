# Data quality case study — why completeness matters

## The apparent trend

A preliminary import of the **October 2026** BEDC publication omitted **114 source rows**. Because November was more complete, a month-to-month comparison initially displayed **87.5% feeder-coverage growth**.

This was **not** evidence of new physical feeders or real expansion in the operating network.

## Investigation and resolution

1. Reconciled October analytical rows against the source regulatory publication.
2. Identified the missing Edo publication records.
3. Corrected two affected October source-row ordering issues.
4. Recovered **114 missing October source records** and corrected associated state mappings.
5. Revalidated unique identities, 21 business units, service-band distribution, and reporting-month totals.

## Before and after

| Indicator | Preliminary | Reconciled |
|---|---:|---:|
| Apparent Oct–Nov published feeder growth | 87.5% | **0.0%** |
| October distinct published feeder identities | 128 | **240** |
| November distinct published feeder identities | 240 | **240** |
| Observed new feeder identities | Misleading due to incomplete ingestion | **0** |

The **114 recovered source rows** and the **240 distinct feeder identities** are different measures and must not be conflated.

## Executive relevance

Incomplete data can create a convincing but false trend. The proof of concept demonstrates **data assurance, reconciliation, and exception-based reporting**. It does not claim verified asset additions, realised savings, or real-time operating visibility.

For the public-source limitations, see [Methodology and limitations](METHODOLOGY_AND_LIMITATIONS.md).
