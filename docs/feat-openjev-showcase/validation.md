# Validation · 2026-09-22

- Supplied PNG copied unchanged: 1600 × 1000, 87,532 bytes; SHA256 ea7983d5b98e0a984ccc1e980a458972ebc1328f5f7b2dd383ebd74b53a14c4e.
- Local browser checked at 320, 768, 1024 and 1440 px: no horizontal overflow; original image loads; links and focus checked. Desktop/mobile screenshots inspected.
- After final editorial revision, repeated 320/1440 DOM checks: no overflow; image natural width 1600; console has no errors.
- HTML IDs and internal anchors checked; benchmark image has descriptive alternative text and a full-size link.
- Claims distinguish the 1,000-question development panel from the separate 9B local HTTP latency run. All three series variants exceed the recorded Jev API score on that panel.
- git diff --check, ruff check . and ruff format --check . are required immediately before push. Ruff has no Python files to inspect in this static site.
- Live deployment verification pending; final receipt is recorded after publication.

Initial Pages build 49035b4 completed. Live verification caught stale unversioned CSS (metrics display:block and overflow). Added a stylesheet version query; final deployed verification required.
