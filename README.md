# Niyobyose Paulin — Personal Profile

A static personal profile website built from `NIYOBYOSE_Paulin_CV.pdf`.

## Content

All copy is taken from the CV: profile, professional experience, skills, projects
(Ranga, Zero QS), education, languages, hobbies and references. The portrait is the
photo embedded in page 1 of the PDF (`public/images/profile.png`, copied into
`images/profile.png`).

## Structure

```
index.html      single page, all sections
styles.css      design system (dark navy + cyan, responsive, print styles)
script.js       mobile menu, scroll reveal, counters, anchor offset
render.yaml     Render Blueprint (static site)
images/         portrait
robots.txt
```

No build step and no dependencies — it is plain HTML, CSS and JS.

## Preview locally

```bash
npx --yes serve -l 4173 .
# open http://localhost:4173
```

Or just open `index.html` in a browser.

## Deploy to Render

Blueprint (recommended): push this folder to a Git repository, then in Render choose
**New → Blueprint** and point it at the repo. `render.yaml` describes the static site.

Manual: **New → Static Site**, connect the repo, set **Publish directory** to `.`
and leave the build command empty.

## Editing

- Text: `index.html`
- Colours, spacing, type: the `:root` variables at the top of `styles.css`
- Photo: replace `images/profile.png` (square image, 600×600 or larger)
