# INFINIACT docs

Legal and policy pages for INFINIACT products, served via GitHub Pages.

**Live site:** https://infiniact.github.io/docs/

## Pages

| Product | Privacy | Terms |
| --- | --- | --- |
| IABar (browser extension) | [/iabar/privacy/](https://infiniact.github.io/docs/iabar/privacy/) | [/iabar/terms/](https://infiniact.github.io/docs/iabar/terms/) |
| IATerm (terminal agent) | [/iaterm/privacy/](https://infiniact.github.io/docs/iaterm/privacy/) | [/iaterm/terms/](https://infiniact.github.io/docs/iaterm/terms/) |

## Structure

Each document is a directory with an `index.html` so the URL is clean (no `.html`):

```
docs/
├── index.html            # landing page
├── assets/style.css      # shared styles (light/dark via prefers-color-scheme)
├── .nojekyll             # serve files as-is, skip Jekyll
├── iabar/{privacy,terms}/index.html
└── iaterm/{privacy,terms}/index.html
```

## Adding a product

Create `<product>/privacy/index.html` and `<product>/terms/index.html`, link
`../../assets/style.css`, and add a card to the root `index.html`.
