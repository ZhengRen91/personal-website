# Personal Academic Website

A modern, dark-themed personal academic website built with vanilla HTML, CSS, and JavaScript.

## Files

- `index.html` — main page structure with all content sections
- `styles.css` — dark theme styling and responsive layout
- `script.js` — navigation, filter, and scroll animations

## Sections

1. **Hero** — Name, title, affiliation, CV link
2. **About** — Bio + stats (publications, citations, h-index)
3. **Research** — Three research interest cards with tags
4. **Publications** — Filterable list (All / Journal / Conference / Preprint)
5. **Links** — Google Scholar, GitHub, ResearchGate, ORCID, LinkedIn, Twitter
6. **Contact** — Email and address

## How to preview

Just open `index.html` in any modern browser. Double-click it from File Explorer, or:

```powershell
start index.html
```

For a local server (recommended for testing relative links):

```powershell
# Python 3
python -m http.server 8000

# Then open http://localhost:8000
```

## Placeholders to replace

All placeholders use `[...]` brackets. Search for `[` in `index.html` and replace:

### Personal info
- `[Your Name]` — your full name (appears in title, hero, footer)
- `[YN]` — your initials for the nav logo
- `[Your Title]` — e.g., "PhD Candidate", "Assistant Professor"
- `[Your Department]`, `[Your University/Institution]`
- `[your.email@example.com]` — contact email (2 places: link and display text)
- `[Your Office Address]`

### Links / URLs
- `[CV URL]` — link to your CV PDF
- `[Google Scholar URL]`
- `[GitHub URL]`
- `[ResearchGate URL]`
- `[ORCID URL]`
- `[LinkedIn URL]`
- `[Twitter/X URL]`

### Stats
- `[XX]` next to "Publications", "h-index", "Projects"
- `[XXX]` next to "Citations"

### Research
- `[Research Area 1/2/3]` — section titles
- Description paragraphs and keyword tags

### Publications
For each `<article class="publication">`:
- `[Year]`, `[Paper Title N]`, `[Co-author]` list
- `[Journal/Conference Name]`, `[Volume/Issue]`, `[Pages]`
- `[PDF URL]`, `[DOI URL]`, `[Code URL]`, `[BibTeX URL]`, `[Slides URL]`, `[arXiv URL]`

To add more papers, copy any `<article class="publication" data-type="...">...</article>` block and edit. The `data-type` attribute (`journal` / `conference` / `preprint`) controls the filter.

### Footer
- `[Month Year]` — last updated date

## Deployment

### GitHub Pages
1. Create a public repo, push these files to the root.
2. Settings → Pages → deploy from `main` branch root.
3. Site will be live at `https://<username>.github.io/<repo>`.

### Other static hosts
Drop the folder onto Netlify, Vercel, or Cloudflare Pages — no build step needed.
