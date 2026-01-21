# Resume Website

Personal resume as a static HTML site, hosted on GitHub Pages.

## Intent

- **Web view**: Rich, interactive design with expandable sections
- **PDF download**: ATS-compliant print stylesheet (Cmd+P → Save as PDF)
- **Single source**: One HTML file serves both purposes

## Key Design Decisions

- **HTML over Markdown**: Full control over structure and styling
- **Print via CSS `@media print`**: No separate PDF generation—browser print handles it
- **Accordion sections**: Jobs expand/collapse on web, all expanded in print
- **Portfolio URL in print header**: So recruiters can find the web version from ATS uploads

## Files

- `index.html` - Resume content and structure
- `styles.css` - Web styling + print styles (via `@media print`)

## Variants

Additional resume variants go in the root as `v2.html`, `v3.html`, etc. (neutral names to avoid revealing targeting).

## Deploying

Push to `main` branch. GitHub Pages serves from root.

```
https://ostegm.github.io/resume
```

## Printing Tips

When saving PDF via browser print:
- Uncheck "Headers and footers"
- Margins: Default
- Background graphics: OFF
