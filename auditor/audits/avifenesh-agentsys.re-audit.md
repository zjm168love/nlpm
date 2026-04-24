# NLPM Re-Audit: avifenesh/agentsys

**Date**: 2026-04-24  |  **Artifacts**: 32  |  **Strategy**: batched
**NL Score**: 97/100
**Bugs**: 0  |  **Quality Issues**: 10

## NL Score Summary

| File | Type | Score | Top Issue |
|------|------|-------|-----------|
| `meta/skills/maintain-cross-platform/SKILL.md` | Skill | 90 | Body exceeds 500 lines (~1024 lines) — R05 |
| `.kiro/skills/enhance-hooks/SKILL.md` | Skill | 90 | Body exceeds 500 lines (555 lines) — R05 (new since v5.8.3) |
| `.kiro/skills/web-browse/SKILL.md` | Skill | 90 | Body exceeds 500 lines (517 lines) — R05; original hardcoded-path bug resolved |
| `CLAUDE.md` | Project memory | 92 | "non-trivial changes" vague (R01); missing prerequisites section |
| `.kiro/skills/drift-analysis/SKILL.md` | Skill | 95 | "reasonable time" vague quantifier (R01) |
| `.kiro/skills/deslop/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/consult/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-cross-file/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-prompts/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-docs/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-orchestrator/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/validate-delivery/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-agent-prompts/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/web-auth/SKILL.md` | Skill | 97 | Original hardcoded-path bug resolved; clean |
| `.kiro/skills/learn/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/debate/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-skills/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-plugins/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/enhance-claude-memory/SKILL.md` | Skill | 97 | Minor |
| `.kiro/skills/orchestrate-review/SKILL.md` | Skill | 98 | "typically indicates" vague quantifier (R01) |
| `.kiro/skills/repo-intel/SKILL.md` | Skill | 98 | "For better analysis" vague quantifier (R01) |
| `.kiro/skills/perf-code-paths/SKILL.md` | Skill | 98 | "when relevant" vague quantifier (R01) |
| `.kiro/skills/perf-benchmarker/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/sync-docs/SKILL.md` | Skill | 98 | "better doc sync accuracy" vague (R01) |
| `.kiro/skills/perf-baseline-manager/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/perf-analyzer/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/perf-theory-gatherer/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/discover-tasks/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/perf-theory-tester/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/perf-profiler/SKILL.md` | Skill | 98 | Clean |
| `.kiro/skills/perf-investigation-logger/SKILL.md` | Skill | 98 | Clean |
| `.claude-plugin/plugin.json` | Manifest | 100 | Clean |

## Bugs (PR-worthy)

| # | File | Issue | Impact |
|---|------|-------|--------|
| — | — | No bugs found | Both hardcoded-path bugs from the original audit (web-auth, web-browse) are confirmed resolved. |

## Quality Issues (informational)

| # | File | Issue | Penalty |
|---|------|-------|---------|
| 1 | `meta/skills/maintain-cross-platform/SKILL.md` | Body is ~1024 lines — well over the 500-line R05 ceiling. Release-process deep-dive and installer detail could move to a `reference/` subdirectory. | -10 |
| 2 | `.kiro/skills/enhance-hooks/SKILL.md` | Body is 555 lines — exceeds 500-line R05 ceiling. New since v5.8.3; likely grew with additional lifecycle-event reference material. | -10 |
| 3 | `.kiro/skills/web-browse/SKILL.md` | Body is 517 lines — marginally exceeds 500-line R05 ceiling. Snapshot-control section could be extracted to a `reference/` file. | -10 |
| 4 | `CLAUDE.md` | "Create PRs for non-trivial changes" — "non-trivial" is a vague quantifier (R01) without measurable criteria. Prefer "changes that touch >1 file or modify public API". | -2 |
| 5 | `CLAUDE.md` | No prerequisites section — the rubric expects a section covering required tools, versions, or setup steps. Project requires Node.js and npm; neither is documented. | -5 |
| 6 | `.kiro/skills/orchestrate-review/SKILL.md` | Line ~66: `// 20+ files typically indicates cross-module changes` — "typically" is a vague quantifier (R01). Replace with a deterministic threshold comment or remove the qualifier. | -2 |
| 7 | `.kiro/skills/repo-intel/SKILL.md` | "For better analysis, run: /repo-intel init" — "better" is a mild vague quantifier (R01). Prefer "for accurate symbol-level analysis" or similar. | -2 |
| 8 | `.kiro/skills/perf-code-paths/SKILL.md` | Line 19: "Include imports/exports or call chains when relevant" — "relevant" is a vague quantifier (R01) without criteria. Specify: "when the scenario crosses module boundaries". | -2 |
| 9 | `.kiro/skills/sync-docs/SKILL.md` | Phase 1.5 AskUserQuestion: "Install for better doc sync accuracy?" — "better" is a mild vague quantifier (R01). Prefer "for AST-level export detection instead of regex fallback". | -2 |
| 10 | `.kiro/skills/drift-analysis/SKILL.md` | "Each item should be completable in reasonable time" — "reasonable" is a vague quantifier (R01) without measurable criteria. Prefer a time bound (e.g., "within one sprint" or "<4 hours"). | -2 |

## Cross-Component

**Resolved since v5.8.3:**
- `web-auth/SKILL.md` and `web-browse/SKILL.md`: Hardcoded developer path `/Users/avifen/.agentsys/plugins/web-ctl/scripts/web-ctl.js` has been replaced throughout with `~/.agentsys/plugins/web-ctl/scripts/web-ctl.js`. Both bug findings from the original audit are verified resolved.

**Persistent observation (from original audit):**
- `enhance-orchestrator/SKILL.md` references agent names (`plugin-enhancer`, `agent-enhancer`, `claudemd-enhancer`, `docs-enhancer`, `prompt-enhancer`, `hooks-enhancer`, `skills-enhancer`, `cross-file-enhancer`) that are not declared in the audited NL artifact set. If those agents are renamed, the orchestrator will break silently. The risk is unchanged since the original audit.

**New observation:**
- `enhance-hooks/SKILL.md` has grown past 500 lines between v5.8.3 and v5.8.6. This is the only quality regression identified in the re-audit.

**Positive:**
- All 32 artifacts retain complete `name` + `description` frontmatter — no registration-breaking omissions.
- `plugin.json` version `5.8.6` is valid semver; all required fields present.
- The eight perf-* skills continue to form a coherent pipeline with `docs/perf-requirements.md` as the canonical contract.
- `CLAUDE.md` Critical Rules remain correctly positioned at the top of the file (lost-in-the-middle best practice).

## Recommendation

High quality — both PR-worthy bugs from the original audit are confirmed fixed, the overall NL score is unchanged at 97/100, and the only new regression is `enhance-hooks` growing past 500 lines. Address the three oversized skills (maintain-cross-platform, enhance-hooks, web-browse) by extracting dense reference material into `reference/` subdirectories; fix the five remaining vague quantifiers and add a prerequisites section to `CLAUDE.md` to reach a clean score.
