# OpenJev showcase handoff

## 1. TL;DR
- Personal homepage now includes an APUS-OpenJev reproduction-series showcase.
- Published and verified at content commit b60f416; Pages built and live mobile/desktop checks passed.
- Central message: all three variants exceed the recorded Jev API baseline on the shared 1,000-question development panel.
- Broader model serving/engine parity work is separate and remains unfinished.

## 2. 本轮交付物
| File | Lines | Purpose |
| --- | ---: | --- |
| index.html | 126 | Series narrative, metrics, original benchmark, model/report links |
| styles.css | 166 | Responsive showcase and print rules |
| assets/openjev/benchmark-1000.png | binary | Exact supplied chart |
| docs/feat-openjev-showcase/design.md | 24 | Approved scope and final editorial direction |
| docs/feat-openjev-showcase/validation.md | 10 | Validation evidence |
| tasks/todo.md | 22 | Delivery checklist |
| tasks/feat-openjev-showcase/lessons.md | 7 | User corrections and lessons |
| tasks/feat-openjev-showcase/handoff.md | under 100 | Cold-start entry |

## 3. 设计约束
- Preserve static HTML/CSS, existing charcoal/lime timeline and co-author attribution.
- Reproduction of the Jev approach does not imply access to unpublished Jev internals.
- Scope superiority to the shared development panel. Do not claim world-first or unmeasured speedups.
- ~26ms is separate 9B local HTTP median latency, one RTX PRO 6000.
- Dynamic-depth paths are application-selectable; do not invent automatic stopping.

## 4. 已踩坑 / 已发现的真实行为
- Browse js accepts expressions; eval accepts a file path. viewport accepts WxH.
- Local preview processes can stop across session interruptions; restart port8767 when needed.
- Supplied chart has white bottom padding; retain original bytes.
- Pages initially delivered cached old CSS with new HTML. Stylesheet now carries a version query; verify computed display:grid and no overflow.
- A follow-up push did not immediately trigger a Pages run; POST pages/builds queued the rebuild.
- Ruff is mandatory but finds no Python files; browser checks validate actual content.

## 5. 下一里程碑任务清单
- [x] Commit/push after required lint gates.
- [x] Verify Pages build and live DOM/image.
- [x] Record publication receipt.

## 6. 分支 / 部署状态
- Repo cryptoSUN2049/cryptoSUN2049.github.io; isolated branch feat-openjev-showcase.
- Inspected base and fetched origin/main: 8cccbe2d8e0ac26495266467f6c62d43ca4d00c7.
- GitHub Pages serves remote main/root. Root local main checkout remains unchanged.
- Local preview http://127.0.0.1:8767/#openjev. Worktree retained.

## 7. 冷启动 checklist
1. Read this handoff, design and validation.
2. Inspect status, remote main and worktrees; preserve concurrent changes.
3. Run local preview and browse from this worktree to isolate browser state.
4. Run git diff --check and both Ruff gates before every push.
5. Verify https://cryptosun2049.github.io/#openjev and Pages commit after publication.

Final receipt: b60f4166552a0c93816cd81a8d410b8b9a95f8e8 built; live320/1440 no overflow, metrics grid, image1600px, console clean. Delivery complete. Evidence-only follow-up commit is retained on the feature branch.
