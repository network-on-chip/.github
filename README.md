# Organization Profile & NoC Paper Map (`.github`)

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-green?logo=creativecommons&logoColor=white)](https://creativecommons.org/licenses/by/4.0/)
[![GitHub Pages](https://img.shields.io/badge/Pages-NoC%20Paper%20Map-181717?logo=github)](https://network-on-chip.github.io/.github/)
[![Parent Monorepo](https://img.shields.io/badge/Monorepo-noc--lab-blue?logo=github)](https://github.com/network-on-chip/noc-lab)
[![Corpus: 541+ Papers](https://img.shields.io/badge/Corpus-541%2B%20Papers-2563eb)](https://github.com/network-on-chip/noc-lab)

Special GitHub organization repository for **[network-on-chip](https://github.com/network-on-chip)**:
- [`profile/README.md`](profile/README.md) renders as the organization's public landing page at `https://github.com/network-on-chip`.
- [`docs/`](docs/) deploys automatically via GitHub Actions to **GitHub Pages** at `https://network-on-chip.github.io/.github/` as an interactive, client-side searchable NoC Paper Map covering 541+ curated research papers.

## Quick Links

- **Organization Homepage**: https://github.com/network-on-chip
- **Interactive Paper Map**: https://network-on-chip.github.io/.github/
- **Parent Monorepo**: https://github.com/network-on-chip/noc-lab
- **License**: [CC BY 4.0](LICENSE)

## Project Layout

```text
.github/
├── .github/
│   └── workflows/
│       └── deploy-pages.yml      # GitHub Actions auto-deployment to GitHub Pages
├── docs/
│   ├── .nojekyll                 # Disables Jekyll processing on GitHub Pages
│   ├── index.html                # Interactive NoC Paper Map single-page app
│   └── papers.json               # 541+ structured paper catalog database
├── profile/
│   └── README.md                 # Public GitHub org homepage
├── LICENSE                       # CC BY 4.0 license deed notice
└── README.md                     # Repository documentation
```

## Features

- **Zero-Dependency Interactive Map**: Built with pure HTML5, vanilla CSS3, and JavaScript — no heavy build frameworks or npm dependencies required.
- **Instant Search**: Real-time filtering across titles, authors, venues, years, DOIs, and abstracts.
- **Domain Filter Pills**: Filter across 11 NoC research domains with live counter badges.
- **Abstract & BibTeX Modal**: 1-click BibTeX copy with clipboard confirmation and direct DOI resolver access.
- **Dark/Light Theme**: Sleek ambient dark theme with high-contrast light theme switch, persisted in `localStorage`.

## Synchronization

This repository is maintained and synchronized from the monorepo [network-on-chip/noc-lab](https://github.com/network-on-chip/noc-lab):

```bash
# In noc-lab
python scripts/export_papers_catalog.py
bash share/sync_github_org.sh
```

## License

Licensed under [Creative Commons Attribution 4.0 International](LICENSE).
