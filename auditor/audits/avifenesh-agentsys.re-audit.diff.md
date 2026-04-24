# Re-Audit: avifenesh/agentsys

**Date**: 2026-04-24  |  **Before**: `unknown` (97/100)  |  **After**: `fd7f8f6` (97/100)

## Summary

| Outcome | Count |
|---------|------:|
| fixed — upstream, not via our PR | 12 |
| newly introduced (regressions) | 11 |

## Original findings — verification

| # | File | Line | Rule | Pattern | Outcome | PR |
|---|------|------|------|---------|---------|----|
| 1 | `.kiro/skills/web-auth/SKILL.md` | — | BUG-broken-reference | `hardcoded-path` | fixed — upstream, not via our PR |  |
| 2 | `.kiro/skills/web-browse/SKILL.md` | — | BUG-unclassified | `same-hardcoded-users-avifen-agentsys-pat` | fixed — upstream, not via our PR |  |
| 3 | `package.json` | — | SEC-unknown | `prepare-script-installs-git-hooks-silent` | fixed — upstream, not via our PR |  |
| 4 | `scripts/dev-install.js` | — | SEC-unknown | `npm-install-production-with-no-registry` | fixed — upstream, not via our PR |  |
| 5 | `package.json` | — | SEC-unknown | `version-script-uses-git-add-a` | fixed — upstream, not via our PR |  |
| 6 | `package.json` | — | SEC-unknown | `unpinned-dependency-versions` | fixed — upstream, not via our PR |  |
| 7 | `.kiro/skills/web-auth/SKILL.md` | — | SEC-unknown | `hardcoded-users-avifen-home-path` | fixed — upstream, not via our PR |  |
| 8 | `.kiro/skills/web-browse/SKILL.md` | — | SEC-unknown | `hardcoded-users-avifen-home-path` | fixed — upstream, not via our PR |  |
| 9 | `meta/skills/maintain-cross-platform/SKILL.md` | — | UNCLASSIFIED | `skill-exceeds-500-lines-1000-lines-the-e` | fixed — upstream, not via our PR |  |
| 10 | `.kiro/skills/orchestrate-review/SKILL.md` | 63 | R01 | `vague-quantifiers` | fixed — upstream, not via our PR |  |
| 11 | `.kiro/skills/repo-intel/SKILL.md` | — | R01 | `vague-quantifiers` | fixed — upstream, not via our PR |  |
| 12 | `.kiro/skills/sync-docs/SKILL.md` | — | R01 | `vague-quantifiers` | fixed — upstream, not via our PR |  |

## Findings introduced since audit

These findings appear in the re-audit but were not in the original audit. They may be true regressions (new commits introduced them) or artifacts of scoring drift.

| # | File | Line | Rule | Pattern | Description |
|---|------|------|------|---------|-------------|
| 1 | `meta/skills/maintain-cross-platform/SKILL.md` | — | R05 | `body-over-500-lines` | Body is ~1024 lines — well over the 500-line R05 ceiling. Release-process deep-dive and installer detail could move to a reference/ subdirectory. |
| 2 | `.kiro/skills/enhance-hooks/SKILL.md` | — | R05 | `body-over-500-lines` | Body is 555 lines — exceeds 500-line R05 ceiling. New regression since v5.8.3; likely grew with additional lifecycle-event reference material. |
| 3 | `.kiro/skills/web-browse/SKILL.md` | — | R05 | `body-over-500-lines` | Body is 517 lines — marginally exceeds 500-line R05 ceiling. Snapshot-control section could be extracted to a reference/ file. |
| 4 | `CLAUDE.md` | — | R01 | `vague-quantifier-non-trivial` | 'Create PRs for non-trivial changes' — 'non-trivial' is a vague quantifier without measurable criteria. |
| 5 | `CLAUDE.md` | — | R05 | `missing-prerequisites-section` | No prerequisites section — the rubric expects a section covering required tools, versions, or setup steps. Project requires Node.js and npm; neither is documented. |
| 6 | `.kiro/skills/orchestrate-review/SKILL.md` | 66 | R01 | `vague-quantifier-typically` | '20+ files typically indicates cross-module changes' — 'typically' is a vague quantifier without deterministic criteria. |
| 7 | `.kiro/skills/repo-intel/SKILL.md` | — | R01 | `vague-quantifier-better` | 'For better analysis, run: /repo-intel init' — 'better' is a vague quantifier. |
| 8 | `.kiro/skills/perf-code-paths/SKILL.md` | 19 | R01 | `vague-quantifier-relevant` | 'Include imports/exports or call chains when relevant' — 'relevant' is a vague quantifier without criteria. |
| 9 | `.kiro/skills/sync-docs/SKILL.md` | — | R01 | `vague-quantifier-better` | Phase 1.5 AskUserQuestion: 'Install for better doc sync accuracy?' — 'better' is a vague quantifier. |
| 10 | `.kiro/skills/drift-analysis/SKILL.md` | — | R01 | `vague-quantifier-reasonable` | 'Each item should be completable in reasonable time' — 'reasonable' is a vague quantifier without measurable criteria. |
| 11 | `.kiro/skills/enhance-orchestrator/SKILL.md` | — | CC-orphan-component | `undeclared-agent-references` | References agent names (plugin-enhancer, agent-enhancer, claudemd-enhancer, docs-enhancer, prompt-enhancer, hooks-enhancer, skills-enhancer, cross-file-enhancer) not declared in the audited NL artifact set. If those agents are renamed, the orchestrator will break silently. |

