# OpenJev homepage showcase

## Approved scope
The user requested OpenJev on the personal homepage, accepted “~26 ms” instead of a percentage speedup, and supplied the 1,000-question benchmark image. Add a compact featured project inside the existing NOW / AGENTS entry; retain the timeline, charcoal/lime styling and static HTML/CSS delivery.

## Content and architecture
Identity → current Agent Native work → OpenJev showcase → HF models / technical report / full-size supplied image. No API, JavaScript, new dependencies or analytics.

- Co-author credit; APUS AI-LAB model family: 4B, 9B and 35B-A3B.
- 1,000-question expanded development panel: 35B-A3B 82.2%, 9B 81.1%, 4B 80.5%, Jev API 77.0%, Laya 50.5%.
- Metric: valid and correct / all questions; base + adapter, step5949, full depth. Not a sealed final test. Jev had972 valid responses/1000; the supplied image includes this scope.
- Selectable dynamic-depth computation: jointly trained early/full paths; applications choose effort low/high. Do not claim automatic stopping or complete vLLM low/high support.
- ~26ms is rounded9B local HTTP P50 on one RTX PRO6000 from a separate serving run; not TTFT or matched-hardware superiority.
- Use the supplied PNG bytes unchanged, meaningful alt text, full-size link, and a short readable caption.
- No “world first”, “200%+”, or “500%” claim.

## Files
index.html; styles.css; assets/openjev/benchmark-1000.png; docs/feat-openjev-showcase/{design,validation}.md; tasks/todo.md; tasks/feat-openjev-showcase/{handoff,lessons}.md.

## Validation and release
Inspect320/768/1024/1440px; no horizontal overflow; readable metrics; image loads at its native size and links to full resolution; keyboard focus/link labels; reduced-motion/print preserved. Verify source image SHA. Run git diff --check, ruff check ., ruff format --check . before push. Push isolated feature branch, merge only against inspected main, verify GitHub Pages build and live DOM/image.

## Final editorial direction
The user clarified that the central message is a Jev reproduction model series that exceeds the recorded Jev baseline. Lead with that contribution and scope the comparison to the shared 1,000-question development panel. Do not imply access to Jev’s unpublished training or architecture.
