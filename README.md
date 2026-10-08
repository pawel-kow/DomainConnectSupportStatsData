# DomainConnectSupportStatsData

**Generated data — do not edit by hand.**

Data behind the Domain Connect statistics site
[DomainConnectSupportStats](https://github.com/pawel-kow/DomainConnectSupportStats).
Every dataset lives in its own directory under `statsdata/` and has exactly one writer;
no writer touches another dataset's directory.

```
statsdata/
├── providers/   # DNS provider / template support statistics
│                # (static export of pawel-kow/DomainConnectScanner, export.py;
│                #  format: docs/EXPORT_FORMAT.md there)
└── templates/   # Template repository statistics (planned; from Domain-Connect/Stats)
```

- `statsdata/providers/` is published automatically by a dedicated publisher account on
  the scanner host: one commit per new export release (`Export release <generated_at>`),
  history kept, no force pushes.
- Every push to `main` that changes `statsdata/**` triggers a deploy of the statistics
  site (`.github/workflows/notify-site.yml`).

Manual changes to the data files are overwritten by the next publish. Change the
producing project instead.
