# KEV Early Warning CTI: Study 1 snapshot (Archival + RSS CTI)

> **This is a snapshot repository.** The maintained project, with full documentation and both studies, lives at **[AinfoCyberSec7/kev-early-warning-cti](https://github.com/AinfoCyberSec7/kev-early-warning-cti)**.

📄 **Paper:** *Archival CTI-Augmented Early Warning of In-the-Wild Exploitation: A Hybrid Evaluation Against the CISA KEV Catalog*, IEEE Cyber-AI 2026, Bucharest, pp. 558–563. [IEEE Xplore](https://ieeexplore.ieee.org/document/11755245) · DOI [10.1109/Cyber-AI70573.2026.11755245](https://doi.org/10.1109/Cyber-AI70573.2026.11755245)

This snapshot keeps the code and results for **study 1**, the published paper, exactly as they were produced. It measures how early open threat intelligence mentions a CVE before CISA adds it to the Known Exploited Vulnerabilities (KEV) catalog, using **14 security RSS feeds plus archival OSV advisories from the GitHub Advisory Database** as CTI sources.

## Headline results

- **170,006 CVEs** (published 2021–2025), **829** in KEV
- **478 of 806** KEV CVEs with a CTI signal (**59.3%**) appeared in CTI **before** KEV listed them
- Median lead time: **3.5 days** (90th percentile: 318 days)
- Best ranking model at disclosure time: **EPSS only** (PR-AUC 0.268)

## What's here

```
config/feeds.yml       RSS sources, tagged pre / confirm
src/                   Pipeline scripts (01 → 11)
reports/paper_assets/  Study 1 tables (CSV) and figures (PNG)
```

For setup, the full pipeline, leakage controls and limitations, see the **[main repository](https://github.com/AinfoCyberSec7/kev-early-warning-cti)**.

## Author

**Abiola A E** ([AinfoCyberSec7](https://github.com/AinfoCyberSec7)), published as Abiola Ayodele Emmanuel.
