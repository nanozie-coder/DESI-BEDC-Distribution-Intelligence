# SQL Server / T-SQL — public release status

The DESI prototype was developed with Microsoft SQL Server for source ingestion, reconciliation, matching and analytical views.

The working database, recovery transactions and full analytical SQL scripts are **not public in this first version**. They will be reviewed before publication for:

- Confidential or non-reusable data
- Server names, passwords, access tokens and local file paths
- Schema portability and dependency order
- Safe behaviour when scripts are executed
- Consistency with the latest corrected Power BI figures

This repository is **documentation-first**, not a turnkey SQL deployment.
