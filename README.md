# Longevity 2031 Scenarios Wiki

A curated wiki distilling:

> David Wood (LEV Foundation / London Futurists), "Anticipating the state of the longevity community and longevity science in 2031" — presentation at the International Longevity Summit, Madrid, 30 September (extended video: London Futurists, YouTube).
> Video: https://www.youtube.com/watch?v=aRADAMzHVEk
> More about LEVF and Robust Mouse Rejuvenation (RMR): https://www.levf.org/

**Public copy:** https://iamflipse.github.io/longevity-scenarios-2031-wiki/ (read-only; static build served from the `gh-pages` branch)

## Layout

- `src/` — wiki pages as markdown (`index.md`, `about.md`, `concepts/`, `sources/`)
- `book/` — mdbook-generated static site (committed for GitHub Pages)
- `tools/mdbook` — mdbook v0.4.21 binary (aarch64 Linux, built from source)

## Rebuild + republish

```sh
./tools/mdbook build -d book
git add -A && git commit -m "update" && git push origin main
# republish gh-pages: check out orphan branch, copy book/* to root, add .nojekyll, force push
```
