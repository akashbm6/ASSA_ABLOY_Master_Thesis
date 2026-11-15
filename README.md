# The Generation Planning Foresight Canvas

An interactive prototype for the ASSA ABLOY Master's thesis application:
**Product Management – Generation Planning & Technology Foresight**.

It shows how scattered signals (technology, market, customers, supply, regulation) can be
structured and turned into generation-planning discussions, options and priorities:

```
SIGNAL → INSIGHT → DISCUSSION → OPTION → PRIORITY (Gen 1 / Gen 2 / Gen 3)
```

## Authors

- **Murtaza**: supply chain planning
- **Akash Busunur Mallikarjuna**: design engineering and product data

## Repository structure

```
.
├── index.html      # The canvas: one self-contained page (inline CSS and JS)
├── .github/workflows/pages.yml  # Publishes index.html to GitHub Pages on push to main
├── CHANGELOG.md    # One entry per tagged version
├── README.md
├── LICENSE         # MIT
└── .gitignore
```

## How to run it

Open `index.html` in a current browser (Chrome, Safari, Firefox or Edge). No build step is needed.

- Fonts and the chart and animation libraries load from pinned CDNs (Google Fonts, cdnjs).
  Without internet the page still works: charts fall back to readable data tables.
- Add `?dev=1` to the address to run the built-in self-test (results print in the browser console).

## Live site (GitHub Pages)

Every push to `main` publishes `index.html` through GitHub Actions to:
https://akashbm6.github.io/ASSA_ABLOY_Master_Thesis/

One-time setup: in the repo, go to **Settings → Pages → Build and deployment** and set **Source** to **GitHub Actions**.

## Editing content

All text, ratings and numbers live in one `DATA` object at the top of the script in `index.html`.
Change them there; the page renders everything from it.

## Labels used on the page

| Label | Meaning |
| --- | --- |
| PUBLIC | Taken from public ASSA ABLOY or industry material |
| OUR WORK | Results from the applicants' own case work |
| ILLUSTRATIVE | Made up for demonstration; not a forecast and not company data |

## AI use

The code for this page was written and debugged with Claude (Anthropic) from the authors' written
specification. The signals, ratings, themes, futures, scoring rule and literature were chosen by the
authors. See the "How we used AI" panel on the page for details.

## License

MIT. See [LICENSE](LICENSE).
