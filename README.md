# Gumpcheng — personal homepage

**[cryptosun2049.github.io](https://cryptosun2049.github.io/)**

A resume-style timeline: cloud systems → LLM training → Agent Native → self-improving models.

Plain HTML and CSS. No JavaScript, dependencies, analytics or build step.

## Preview

```sh
python3 -m http.server 8766 --bind 127.0.0.1
```

Open http://127.0.0.1:8766. The page includes mobile and print layouts.

## Maintain

- Edit `index.html` for content and `styles.css` for styling.
- Attribute model releases to the xDAN AI team.
- Keep future interests distinct from current accomplishments.
- Use only supported dates and source links; avoid unverified ranking claims.
- Check keyboard navigation and widths 320, 768, 1024 and 1440px before publishing.

## Publish

GitHub Pages serves `main` from the repository root. `.nojekyll` disables Jekyll processing.
Before each push, run `git diff --check`, `ruff check .` and `ruff format --check .`.
Ruff is a repository workflow gate; HTML/CSS validation is performed separately in the browser.

After pushing, verify Pages build status and the live page.

[GitHub profile](https://github.com/cryptoSUN2049) · [Team models](https://huggingface.co/xDAN-AI)
