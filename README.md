# DomainConnectSupportStatsData

**Generated data — do not edit by hand.**

This repository holds the static JSON export of the
[DomainConnectScanner](https://github.com/pawel-kow/DomainConnectScanner) statistics
(`export.py`). It is published automatically by a dedicated publisher account on the
scanner host: one commit per new export release (`Export release <generated_at>`), history
kept, no force pushes.

- Data format: see `docs/EXPORT_FORMAT.md` in DomainConnectScanner.
- Every push to `main` triggers a deploy of the statistics site
  [DomainConnectSupportStats](https://github.com/pawel-kow/DomainConnectSupportStats)
  (`.github/workflows/notify-site.yml`).

Manual changes to the data files are overwritten by the next publish. Change the scanner
or its export instead.
