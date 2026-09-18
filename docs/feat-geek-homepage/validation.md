# Validation — 2026-09-18

## Local checks

- Static HTML parsing: one h1, unique IDs, valid internal anchors, no empty links.
- XML parsing: valid favicon SVG and sitemap.
- Local stylesheet and entry document: HTTP 200.
- Responsive browser checks: 320, 768, 1024 and 1440px, no horizontal overflow; all four timeline entries present.
- Keyboard: first Tab reaches visible skip link with focus outline; Enter moves focus to the experience section.
- Contrast against background: text 15.97:1, muted 8.66:1, secondary 6.47:1, accent 15.43:1.
- No console errors on local page.
- Print PDF: two readable A4 pages; summary retains line breaks, entries remain together.
- Independent static review: no blocking issues; print line-break issue fixed.
- No runtime JavaScript, third-party fonts or analytics requests.

## Link checks

- Three selected Hugging Face model pages: HTTP 200.
- `cryptoSUN2049/xDAN-DSH-uni-agent`: HTTP 200; labeled as a fork.
- `www.xdan.ai` and `cloud.openfinclaw.ai`: HTTP 502 during checks. Omitted from navigation; company and project names preserved.
- Company contact address comes from the supplied company introduction; no email was sent.
- New homepage and source repository will be checked after publication.

## Workflow gates

- `git diff --check`: pass.
- `ruff check .`: pass (no Python files).
- `ruff format --check .`: pass (no Python files).
- No build step or application logic requiring unit tests; browser checks cover the actual static deliverable.

## Live checks

- GitHub Pages status: built, HTTPS enforced, main / root.
- Content deployment commit: `e40c7d979eeac81f3567b10dc597789fac5bd9c1`.
- Live URL https://cryptosun2049.github.io/ returns HTTP 200 with the expected title, one h1, four timeline entries and the production stylesheet.
- Live 320px and 1440px checks: viewport width equals document width; no horizontal overflow.
- Fresh live reload: no console errors.
- GitHub account bio and blog now match the approved copy and the Pages URL.
- Profile README rendered on the actual GitHub profile; its remote blob matches local `e11a63dd41da1095c9b0e2fc5844c802b7b6ca07`.
