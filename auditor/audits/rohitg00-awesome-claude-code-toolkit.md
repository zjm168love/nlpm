# NLPM Audit: rohitg00/awesome-claude-code-toolkit
**Date**: 2026-04-16  |  **Artifacts**: 558  |  **Strategy**: progressive
**NL Score**: 55/100
**Security**: REVIEW
**Bugs**: 265  |  **Quality Issues**: 447  |  **Security Findings**: 13

---

## NL Score Summary

> Scored 439 NL markdown artifacts (agents, commands, skills). ~119 JSON config files (plugin.json, hooks.json) are inventoried separately and not scored as NL artifacts.

| File | Type | Score | Top Issue |
|------|------|-------|-----------|
| plugins/model-evaluator/commands/compare-models.md | command | 21 | Missing frontmatter + no format + vague x2 |
| plugins/responsive-designer/commands/test-responsive.md | command | 21 | Missing frontmatter + no format + vague x2 |
| plugins/responsive-designer/commands/add-breakpoints.md | command | 21 | Missing frontmatter + no format + vague x2 |
| plugins/readme-generator/commands/generate-readme.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/azure-helper/commands/setup-functions.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/azure-helper/commands/configure-blob.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/model-evaluator/commands/evaluate-model.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/complexity-reducer/commands/analyze-complexity.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/complexity-reducer/commands/simplify-fn.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/onboarding-guide/commands/create-guide.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/schema-designer/commands/design-schema.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/android-developer/commands/add-viewmodel.md | command | 23 | Missing frontmatter + no format + vague |
| plugins/visual-regression/commands/capture-baseline.md | command | 25 | Missing frontmatter + no format |
| plugins/visual-regression/commands/compare.md | command | 25 | Missing frontmatter + no format |
| plugins/bundle-analyzer/commands/tree-shake.md | command | 25 | Missing frontmatter + no format |
| plugins/bundle-analyzer/commands/analyze-bundle.md | command | 25 | Missing frontmatter + no format |
| plugins/license-checker/commands/generate-notice.md | command | 25 | Missing frontmatter + no format |
| plugins/license-checker/commands/check-licenses.md | command | 25 | Missing frontmatter + no format |
| plugins/gcp-helper/commands/configure-gcs.md | command | 25 | Missing frontmatter + no format |
| plugins/gcp-helper/commands/setup-cloud-run.md | command | 25 | Missing frontmatter + no format |
| plugins/rag-builder/commands/index-docs.md | command | 25 | Missing frontmatter + no format |
| plugins/rag-builder/commands/create-retriever.md | command | 25 | Missing frontmatter + no format |
| plugins/helm-charts/commands/create-chart.md | command | 25 | Missing frontmatter + no format |
| plugins/helm-charts/commands/upgrade-chart.md | command | 25 | Missing frontmatter + no format |
| plugins/ci-debugger/commands/fix-pipeline.md | command | 25 | Missing frontmatter + no format |
| plugins/ci-debugger/commands/analyze-ci-failure.md | command | 25 | Missing frontmatter + no format |
| plugins/github-issue-manager/commands/create-issue.md | command | 25 | Missing frontmatter + no format |
| plugins/github-issue-manager/commands/triage-issues.md | command | 25 | Missing frontmatter + no format |
| plugins/mutation-tester/commands/mutate.md | command | 25 | Missing frontmatter + no format |
| plugins/screen-reader-tester/commands/test-sr.md | command | 25 | Missing frontmatter + no format |
| plugins/screen-reader-tester/commands/fix-aria.md | command | 25 | Missing frontmatter + no format |
| plugins/slack-notifier/commands/send-update.md | command | 25 | Missing frontmatter + no format |
| plugins/slack-notifier/commands/create-thread.md | command | 25 | Missing frontmatter + no format |
| plugins/seed-generator/commands/generate-seeds.md | command | 25 | Missing frontmatter + no format |
| plugins/contract-tester/commands/create-contract.md | command | 25 | Missing frontmatter + no format |
| plugins/contract-tester/commands/verify-contract.md | command | 25 | Missing frontmatter + no format |
| plugins/import-organizer/commands/organize.md | command | 25 | Missing frontmatter + no format |
| plugins/env-sync/commands/diff-env.md | command | 25 | Missing frontmatter + no format |
| plugins/env-sync/commands/sync-env.md | command | 25 | Missing frontmatter + no format |
| plugins/embedding-manager/commands/search-similar.md | command | 25 | Missing frontmatter + no format |
| plugins/embedding-manager/commands/generate-embeddings.md | command | 25 | Missing frontmatter + no format |
| plugins/schema-designer/commands/generate-erd.md | command | 25 | Missing frontmatter + no format |
| plugins/css-cleaner/commands/consolidate.md | command | 25 | Missing frontmatter + no format |
| plugins/css-cleaner/commands/find-unused-css.md | command | 25 | Missing frontmatter + no format |
| plugins/android-developer/commands/create-activity.md | command | 25 | Missing frontmatter + no format |
| plugins/regex-builder/commands/build-regex.md | command | 25 | Missing frontmatter + no format |
| plugins/regex-builder/commands/test-regex.md | command | 25 | Missing frontmatter + no format |
| plugins/test-data-generator/commands/generate-data.md | command | 25 | Missing frontmatter + no format |
| plugins/test-data-generator/commands/seed-db.md | command | 25 | Missing frontmatter + no format |
| plugins/query-optimizer/commands/optimize-query.md | command | 25 | Missing frontmatter + no format |
| plugins/query-optimizer/commands/explain-plan.md | command | 25 | Missing frontmatter + no format |
| plugins/api-reference/commands/generate-api-ref.md | command | 25 | Missing frontmatter + no format |
| plugins/linear-helper/commands/update-status.md | command | 25 | Missing frontmatter + no format |
| plugins/linear-helper/commands/create-ticket.md | command | 25 | Missing frontmatter + no format |
| plugins/api-benchmarker/commands/report.md | command | 25 | Missing frontmatter + no format |
| plugins/api-benchmarker/commands/benchmark.md | command | 25 | Missing frontmatter + no format |
| plugins/type-migrator/commands/migrate-file.md | command | 25 | Missing frontmatter + no format |
| plugins/type-migrator/commands/add-types.md | command | 25 | Missing frontmatter + no format |
| commands/refactoring/simplify.md | command | 25 | Missing frontmatter + no format |
| commands/architecture/refactor.md | command | 25 | Missing frontmatter + no format |
| commands/architecture/plan.md | command | 25 | Missing frontmatter + no format |
| commands/architecture/migrate.md | command | 25 | Missing frontmatter + no format |
| commands/documentation/doc-gen.md | command | 25 | Missing frontmatter + no format |
| commands/testing/tdd.md | command | 25 | Missing frontmatter + no format |
| commands/testing/test-coverage.md | command | 25 | Missing frontmatter + no format |
| commands/testing/e2e.md | command | 25 | Missing frontmatter + no format |
| commands/devops/ci-pipeline.md | command | 25 | Missing frontmatter + no format |
| commands/devops/dockerfile.md | command | 25 | Missing frontmatter + no format |
| commands/security/hardening.md | command | 25 | Missing frontmatter + no format |
| commands/security/audit.md | command | 25 | Missing frontmatter + no format |
| plugins/web-dev/commands/add-page.md | command | 28 | Missing name + hollow steps + vague |
| plugins/rapid-prototyper/commands/mockup.md | command | 28 | Missing name + hollow steps + vague |
| plugins/desktop-app/commands/scaffold-desktop.md | command | 28 | Missing name + hollow steps + vague |
| plugins/fix-github-issue/commands/fix-issue.md | command | 28 | Missing name + hollow steps + vague |
| plugins/technical-sales/commands/write-proposal.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/technical-sales/commands/create-demo.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/devops-automator/commands/health-check.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/devops-automator/commands/automate.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/fix-pr/commands/fix-comments.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/openapi-expert/commands/validate-spec.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/openapi-expert/commands/generate-spec.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/dependency-manager/commands/update-deps.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/dependency-manager/commands/audit-deps.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/security-guidance/commands/security-check.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/security-guidance/commands/fix-vulnerability.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/performance-monitor/commands/profile-api.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/performance-monitor/commands/benchmark.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/flutter-mobile/commands/platform-channel.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/flutter-mobile/commands/create-widget.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/migrate-tool/commands/code-migrate.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/migrate-tool/commands/db-migrate.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/changelog-gen/commands/generate-changelog.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/smart-commit/commands/changelog.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/react-native-dev/commands/native-module.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/react-native-dev/commands/create-screen.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/analytics-reporter/commands/report.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/analytics-reporter/commands/dashboard.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/accessibility-checker/commands/a11y-scan.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/accessibility-checker/commands/aria-fix.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/python-expert/commands/refactor-py.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/python-expert/commands/type-hints.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/experiment-tracker/commands/track.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/experiment-tracker/commands/compare.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/pr-reviewer/commands/review-pr.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/pr-reviewer/commands/approve-pr.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/release-manager/commands/release.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/release-manager/commands/bump-version.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/docker-helper/commands/build-image.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/docker-helper/commands/optimize-dockerfile.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/code-guardian/commands/security-scan.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/debug-session/commands/bisect.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/debug-session/commands/debug.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/model-context-protocol/commands/create-server.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/model-context-protocol/commands/add-tool.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/ai-prompt-lab/commands/test-prompt.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/ai-prompt-lab/commands/improve-prompt.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/infrastructure-maintainer/commands/audit-infra.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/infrastructure-maintainer/commands/update-infra.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/update-branch/commands/rebase.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/workflow-optimizer/commands/suggest-improvements.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/workflow-optimizer/commands/analyze-workflow.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/test-results-analyzer/commands/analyze-failures.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/context7-docs/commands/fetch-docs.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/commit-commands/commands/amend.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/test-writer/commands/unit-test.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/test-writer/commands/integration-test.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/product-shipper/commands/ship.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/vision-specialist/commands/analyze-screenshot.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/vision-specialist/commands/extract-text.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/discuss/commands/discuss.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/explore/commands/explore.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/explore/commands/map.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/database-optimizer/commands/analyze-query.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/k8s-helper/commands/generate-manifest.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/k8s-helper/commands/debug-pod.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/monitoring-setup/commands/create-dashboard.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/monitoring-setup/commands/setup-monitoring.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/ultrathink/commands/think.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/content-creator/commands/write-post.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/content-creator/commands/social-media.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/git-flow/commands/flow-start.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/code-review-assistant/commands/review.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/frontend-developer/commands/create-component.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/frontend-developer/commands/style.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/tool-evaluator/commands/evaluate.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/tool-evaluator/commands/compare-tools.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/feature-dev/commands/implement.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/feature-dev/commands/complete.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/double-check/commands/verify.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/code-architect/commands/diagram.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/code-architect/commands/architect.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/backend-architect/commands/add-endpoint.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/backend-architect/commands/design-service.md | command | 35 | Missing frontmatter (name+desc) |
| commands/refactoring/rename.md | command | 35 | Missing frontmatter (name+desc) |
| commands/refactoring/dead-code.md | command | 35 | Missing frontmatter (name+desc) |
| commands/refactoring/cleanup.md | command | 35 | Missing frontmatter (name+desc) |
| commands/refactoring/extract.md | command | 35 | Missing frontmatter (name+desc) |
| commands/workflow/checkpoint.md | command | 35 | Missing frontmatter (name+desc) |
| commands/workflow/wrap-up.md | command | 35 | Missing frontmatter (name+desc) |
| commands/workflow/orchestrate.md | command | 35 | Missing frontmatter (name+desc) |
| commands/architecture/diagram.md | command | 35 | Missing frontmatter (name+desc) |
| commands/architecture/adr.md | command | 35 | Missing frontmatter (name+desc) |
| commands/architecture/design-review.md | command | 35 | Missing frontmatter (name+desc) |
| commands/documentation/update-codemap.md | command | 35 | Missing frontmatter (name+desc) |
| commands/documentation/api-docs.md | command | 35 | Missing frontmatter (name+desc) |
| commands/documentation/onboard.md | command | 35 | Missing frontmatter (name+desc) |
| commands/documentation/memory-bank.md | command | 35 | Missing frontmatter (name+desc) |
| commands/testing/snapshot-test.md | command | 35 | Missing frontmatter (name+desc) |
| commands/testing/test-fix.md | command | 35 | Missing frontmatter (name+desc) |
| commands/testing/integration-test.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/release.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/worktree.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/commit.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/changelog.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/pr-review.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/pr-create.md | command | 35 | Missing frontmatter (name+desc) |
| commands/git/fix-issue.md | command | 35 | Missing frontmatter (name+desc) |
| commands/devops/k8s-manifest.md | command | 35 | Missing frontmatter (name+desc) |
| commands/devops/deploy.md | command | 35 | Missing frontmatter (name+desc) |
| commands/devops/monitor.md | command | 35 | Missing frontmatter (name+desc) |
| commands/security/csp.md | command | 35 | Missing frontmatter (name+desc) |
| commands/security/dependency-audit.md | command | 35 | Missing frontmatter (name+desc) |
| commands/security/secrets-scan.md | command | 35 | Missing frontmatter (name+desc) |
| plugins/unit-test-generator/commands/generate-tests.md | command | 33 | Missing frontmatter + vague |
| plugins/commit-commands/commands/commit-push.md | command | 33 | Missing frontmatter + vague |
| plugins/product-shipper/commands/launch-checklist.md | command | 33 | Missing frontmatter + vague |
| plugins/database-optimizer/commands/add-index.md | command | 33 | Missing frontmatter + vague |
| plugins/git-flow/commands/flow-release.md | command | 33 | Missing frontmatter + vague |
| plugins/create-worktrees/commands/worktree-clean.md | command | 50 | Missing name + hollow steps |
| plugins/create-worktrees/commands/worktree-create.md | command | 50 | Missing name + hollow steps |
| plugins/n8n-workflow/commands/create-workflow.md | command | 50 | Missing name + hollow steps |
| plugins/web-dev/commands/scaffold-app.md | command | 50 | Missing name + hollow steps |
| plugins/sprint-prioritizer/commands/plan-sprint.md | command | 50 | Missing name + hollow steps |
| plugins/sprint-prioritizer/commands/prioritize.md | command | 50 | Missing name + hollow steps |
| plugins/rapid-prototyper/commands/prototype.md | command | 50 | Missing name + hollow steps |
| plugins/finance-tracker/commands/track-cost.md | command | 50 | Missing name + hollow steps |
| plugins/finance-tracker/commands/report-cost.md | command | 50 | Missing name + hollow steps |
| plugins/codebase-documenter/commands/document-all.md | command | 50 | Missing name + hollow steps |
| plugins/data-privacy/commands/audit-pii.md | command | 50 | Missing name + hollow steps |
| plugins/data-privacy/commands/anonymize.md | command | 50 | Missing name + hollow steps |
| plugins/optimize/commands/optimize-size.md | command | 50 | Missing name + hollow steps |
| plugins/optimize/commands/optimize-perf.md | command | 50 | Missing name + hollow steps |
| plugins/compliance-checker/commands/check-soc2.md | command | 50 | Missing name + hollow steps |
| plugins/compliance-checker/commands/check-gdpr.md | command | 50 | Missing name + hollow steps |
| plugins/plan/commands/plan.md | command | 50 | Missing name + hollow steps |
| plugins/plan/commands/estimate.md | command | 50 | Missing name + hollow steps |
| plugins/ui-designer/commands/implement-design.md | command | 50 | Missing name + hollow steps |
| plugins/smart-commit/commands/commit.md | command | 45 | Missing frontmatter (name+desc) — best in batch |
| plugins/code-guardian/commands/review.md | command | 45 | Missing frontmatter (name+desc) — best in batch |
| plugins/env-manager/commands/env-validate.md | command | 45 | Missing frontmatter (name+desc) |
| plugins/env-manager/commands/env-setup.md | command | 45 | Missing frontmatter (name+desc) |
| plugins/api-tester/commands/test-endpoint.md | command | 56 | Missing name + vague x2 |
| plugins/refactor-engine/commands/extract-fn.md | command | 58 | Missing name + vague |
| plugins/ios-developer/commands/create-view.md | command | 59 | Excessive vague quantifiers (8 hits) |
| plugins/bug-detective/commands/debug.md | command | 60 | Missing name (no H1) |
| plugins/bug-detective/commands/trace.md | command | 60 | Missing name (no H1) |
| plugins/code-explainer/commands/annotate.md | command | 60 | Missing name (no H1) |
| plugins/code-explainer/commands/explain.md | command | 60 | Missing name (no H1) |
| plugins/project-scaffold/commands/scaffold.md | command | 60 | Missing name (no H1) |
| plugins/project-scaffold/commands/add-feature.md | command | 60 | Missing name (no H1) |
| plugins/monorepo-manager/commands/sync-versions.md | command | 60 | Missing name (no H1) |
| plugins/monorepo-manager/commands/affected.md | command | 60 | Missing name (no H1) |
| plugins/api-tester/commands/load-test.md | command | 60 | Missing name (no H1) |
| plugins/refactor-engine/commands/simplify.md | command | 60 | Missing name (no H1) |
| plugins/ios-developer/commands/add-model.md | command | 61 | Excessive vague quantifiers (7 hits) |
| plugins/aws-helper/commands/setup-lambda.md | command | 67 | No format + vague x4 |
| plugins/prompt-optimizer/commands/analyze-prompt.md | command | 69 | No format + vague x3 |
| plugins/color-contrast/commands/check-contrast.md | command | 71 | No format + vague x2 |
| plugins/adr-writer/commands/write-adr.md | command | 71 | No format + vague x2 |
| plugins/e2e-runner/commands/record-test.md | command | 71 | No format + vague x2 |
| plugins/terraform-helper/commands/create-module.md | command | 71 | No format + vague x2 |
| plugins/a11y-audit/commands/run-audit.md | command | 71 | No format + vague x2 |
| plugins/cron-scheduler/commands/create-cron.md | command | 71 | No format + vague x2 |
| plugins/memory-profiler/commands/find-leaks.md | command | 71 | No format + vague x2 |
| plugins/dead-code-finder/commands/find-dead-code.md | command | 73 | No format + vague |
| plugins/prompt-optimizer/commands/optimize-prompt.md | command | 73 | No format + vague |
| plugins/e2e-runner/commands/run-e2e.md | command | 73 | No format + vague |
| plugins/migration-generator/commands/rollback.md | command | 73 | No format + vague |
| plugins/migration-generator/commands/create-migration.md | command | 73 | No format + vague |
| plugins/terraform-helper/commands/plan-apply.md | command | 73 | No format + vague |
| plugins/a11y-audit/commands/generate-report.md | command | 73 | No format + vague |
| plugins/cron-scheduler/commands/validate-schedule.md | command | 73 | No format + vague |
| plugins/lighthouse-runner/commands/fix-issues.md | command | 73 | No format + vague |
| plugins/color-contrast/commands/suggest-colors.md | command | 75 | No format, no empty-input handling |
| plugins/aws-helper/commands/configure-s3.md | command | 75 | No format |
| plugins/adr-writer/commands/list-adrs.md | command | 75 | No format |
| plugins/load-tester/commands/generate-report.md | command | 75 | No format |
| plugins/load-tester/commands/run-load-test.md | command | 75 | No format |
| plugins/dead-code-finder/commands/remove-dead-code.md | command | 75 | No format |
| plugins/changelog-writer/commands/write-changelog.md | command | 75 | No format |
| plugins/memory-profiler/commands/profile-memory.md | command | 75 | No format |
| plugins/lighthouse-runner/commands/run-audit.md | command | 75 | No format |
| plugins/deploy-pilot/commands/k8s-manifest.md | command | 79 | No empty-input handling + vague x3 |
| plugins/deploy-pilot/commands/dockerfile.md | command | 79 | No empty-input handling + vague x3 |
| plugins/perf-profiler/commands/optimize.md | command | 79 | No empty-input handling + vague x3 |
| plugins/doc-forge/commands/generate-docs.md | command | 79 | No empty-input handling + vague x3 |
| plugins/doc-forge/commands/update-readme.md | command | 81 | No empty-input handling + vague x2 |
| plugins/api-architect/commands/design-api.md | command | 81 | No empty-input handling + vague x2 |
| plugins/doc-forge/commands/api-docs.md | command | 83 | No empty-input handling + vague |
| plugins/deploy-pilot/commands/ci-pipeline.md | command | 83 | No empty-input handling + vague |
| plugins/perf-profiler/commands/profile.md | command | 83 | No empty-input handling + vague |
| plugins/api-architect/commands/generate-openapi.md | command | 83 | No empty-input handling + vague |
| agents/orchestration/context-manager.md | agent | 61 | No examples + 7 vague words |
| agents/orchestration/workflow-director.md | agent | 63 | No examples + 6 vague words |
| agents/data-ai/feature-engineer.md | agent | 65 | No examples + 5 vague words |
| agents/business-product/legal-advisor.md | agent | 65 | No examples + 5 vague words |
| agents/business-product/customer-success.md | agent | 65 | No examples + 5 vague words |
| agents/research-analysis/patent-analyst.md | agent | 65 | No examples + 5 vague words |
| agents/research-analysis/search-specialist.md | agent | 65 | No examples + 5 vague words |
| agents/specialized-domains/geospatial-engineer.md | agent | 67 | No examples + 4 vague words |
| agents/specialized-domains/blockchain-developer.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/seo-specialist.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/voice-assistant.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/healthcare-engineer.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/education-tech.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/payment-integration.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/fintech-engineer.md | agent | 69 | No examples + 3 vague |
| agents/business-product/technical-writer.md | agent | 69 | No examples + 3 vague |
| agents/business-product/growth-engineer.md | agent | 69 | No examples + 3 vague |
| agents/research-analysis/benchmarking-specialist.md | agent | 69 | No examples + 3 vague |
| agents/language-experts/rust-systems.md | agent | 69 | No examples + 3 vague |
| agents/language-experts/typescript-specialist.md | agent | 69 | No examples + 3 vague |
| agents/data-ai/recommendation-engine.md | agent | 69 | No examples + 3 vague |
| agents/specialized-domains/robotics-engineer.md | agent | 71 | No examples + 2 vague |
| agents/data-ai/vector-database-engineer.md | agent | 71 | No examples + 2 vague |
| agents/data-ai/data-visualization.md | agent | 71 | No examples + 2 vague |
| agents/data-ai/etl-specialist.md | agent | 71 | No examples + 2 vague |
| agents/business-product/business-analyst.md | agent | 71 | No examples + 2 vague |
| agents/business-product/content-strategist.md | agent | 71 | No examples + 2 vague |
| agents/orchestration/error-coordinator.md | agent | 71 | No examples + 2 vague |
| agents/research-analysis/market-researcher.md | agent | 71 | No examples + 2 vague |
| agents/research-analysis/technology-scout.md | agent | 71 | No examples + 2 vague |
| agents/research-analysis/data-researcher.md | agent | 71 | No examples + 2 vague |
| agents/research-analysis/security-researcher.md | agent | 71 | No examples + 2 vague |
| agents/language-experts/clojure-developer.md | agent | 71 | No examples + 2 vague |
| agents/language-experts/swift-developer.md | agent | 71 | No examples + 2 vague |
| agents/language-experts/ocaml-developer.md | agent | 71 | No examples + 2 vague |
| agents/core-development/mobile-developer.md | agent | 73 | No examples + 1 vague |
| agents/quality-assurance/qa-automation.md | agent | 73 | No examples + 1 vague |
| agents/quality-assurance/performance-engineer.md | agent | 73 | No examples + 1 vague |
| agents/infrastructure/kubernetes-specialist.md | agent | 73 | No examples + 1 vague |
| agents/infrastructure/network-engineer.md | agent | 73 | No examples + 1 vague |
| agents/developer-experience/dependency-manager.md | agent | 73 | No examples + 1 vague |
| agents/developer-experience/tooling-engineer.md | agent | 73 | No examples + 1 vague |
| agents/developer-experience/vscode-extension.md | agent | 73 | No examples + 1 vague |
| agents/developer-experience/git-workflow-manager.md | agent | 73 | No examples + 1 vague |
| agents/business-product/marketing-analyst.md | agent | 73 | No examples + 1 vague |
| agents/business-product/project-manager.md | agent | 73 | No examples + 1 vague |
| agents/business-product/scrum-master.md | agent | 73 | No examples + 1 vague |
| agents/orchestration/agent-installer.md | agent | 73 | No examples + 1 vague |
| agents/orchestration/knowledge-synthesizer.md | agent | 73 | No examples + 1 vague |
| agents/orchestration/performance-monitor.md | agent | 73 | No examples + 1 vague |
| agents/orchestration/task-coordinator.md | agent | 73 | No examples + 1 vague |
| agents/orchestration/multi-agent-coordinator.md | agent | 73 | No examples + 1 vague |
| agents/research-analysis/academic-researcher.md | agent | 73 | No examples + 1 vague |
| agents/language-experts/haskell-developer.md | agent | 73 | No examples + 1 vague |
| agents/language-experts/django-developer.md | agent | 73 | No examples + 1 vague |
| agents/language-experts/golang-developer.md | agent | 73 | No examples + 1 vague |
| agents/language-experts/scala-developer.md | agent | 73 | No examples + 1 vague |
| agents/specialized-domains/game-developer.md | agent | 73 | No examples + 1 vague |
| agents/specialized-domains/media-streaming.md | agent | 73 | No examples + 1 vague |
| agents/developer-experience/api-documentation.md | agent | 73 | No examples + 1 vague |
| agents/specialized-domains/embedded-systems.md | agent | 75 | No examples, no output format |
| agents/specialized-domains/real-estate-tech.md | agent | 75 | No examples, no output format |
| agents/specialized-domains/e-commerce-engineer.md | agent | 75 | No examples, no output format |
| agents/specialized-domains/iot-engineer.md | agent | 75 | No examples, no output format |
| agents/business-product/sales-engineer.md | agent | 75 | No examples, no output format |
| agents/business-product/product-manager.md | agent | 75 | No examples, no output format |
| agents/business-product/ux-researcher.md | agent | 75 | No examples, no output format |
| agents/research-analysis/competitive-analyst.md | agent | 75 | No examples, no output format |
| agents/research-analysis/research-analyst.md | agent | 75 | No examples, no output format |
| agents/research-analysis/trend-analyst.md | agent | 75 | No examples, no output format |
| agents/language-experts/nim-developer.md | agent | 75 | No examples, no output format |
| agents/language-experts/java-architect.md | agent | 75 | No examples, no output format |
| agents/language-experts/php-developer.md | agent | 75 | No examples, no output format |
| agents/language-experts/lua-developer.md | agent | 75 | No examples, no output format |
| agents/language-experts/zig-developer.md | agent | 75 | No examples, no output format |
| agents/language-experts/rails-expert.md | agent | 75 | No examples, no output format |
| agents/language-experts/python-engineer.md | agent | 75 | No examples, no output format |
| agents/language-experts/nextjs-developer.md | agent | 75 | No examples, no output format |
| agents/core-development/fullstack-engineer.md | agent | 75 | No examples, no output format |
| agents/core-development/backend-developer.md | agent | 75 | No examples, no output format |
| agents/core-development/api-gateway-engineer.md | agent | 75 | No examples, no output format |
| agents/core-development/monorepo-architect.md | agent | 75 | No examples, no output format |
| agents/core-development/ui-designer.md | agent | 75 | No examples, no output format |
| agents/core-development/event-driven-architect.md | agent | 75 | No examples, no output format |
| agents/core-development/frontend-architect.md | agent | 75 | No examples, no output format |
| agents/core-development/electron-developer.md | agent | 75 | No examples, no output format |
| agents/quality-assurance/chaos-engineer.md | agent | 75 | No examples, no output format |
| agents/quality-assurance/error-detective.md | agent | 75 | No examples, no output format |
| agents/quality-assurance/test-architect.md | agent | 75 | No examples, no output format |
| agents/quality-assurance/compliance-auditor.md | agent | 75 | No examples, no output format |
| agents/quality-assurance/accessibility-specialist.md | agent | 75 | No examples, no output format |
| agents/quality-assurance/code-reviewer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/devops-engineer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/cloud-architect.md | agent | 75 | No examples, no output format |
| agents/infrastructure/deployment-engineer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/sre-engineer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/incident-responder.md | agent | 75 | No examples, no output format |
| agents/infrastructure/security-engineer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/terraform-engineer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/platform-engineer.md | agent | 75 | No examples, no output format |
| agents/infrastructure/database-admin.md | agent | 75 | No examples, no output format |
| agents/developer-experience/monorepo-tooling.md | agent | 75 | No examples, no output format |
| agents/developer-experience/cli-developer.md | agent | 75 | No examples, no output format |
| agents/developer-experience/mcp-developer.md | agent | 75 | No examples, no output format |
| agents/developer-experience/documentation-engineer.md | agent | 75 | No examples, no output format |
| agents/developer-experience/legacy-modernizer.md | agent | 75 | No examples, no output format |
| agents/developer-experience/build-engineer.md | agent | 75 | No examples, no output format |
| agents/developer-experience/developer-portal.md | agent | 75 | No examples, no output format |
| agents/developer-experience/testing-infrastructure.md | agent | 75 | No examples, no output format |
| agents/developer-experience/dx-optimizer.md | agent | 75 | No examples, no output format |
| agents/developer-experience/refactoring-specialist.md | agent | 75 | No examples, no output format |
| agents/language-experts/svelte-developer.md | agent | 83 | 1 example only, no output format, 1 vague |
| agents/language-experts/csharp-developer.md | agent | 83 | 1 example only, no output format, 1 vague |
| agents/language-experts/flutter-expert.md | agent | 83 | 1 example only, no output format, 1 vague |
| agents/language-experts/elixir-expert.md | agent | 83 | 1 example only, no output format, 1 vague |
| agents/language-experts/vue-specialist.md | agent | 83 | 1 example only, no output format, 1 vague |
| agents/quality-assurance/security-auditor.md | agent | 83 | No examples, 1 vague |
| agents/data-ai/database-optimizer.md | agent | 81 | 1 code example, no output format, 2 vague |
| agents/data-ai/prompt-engineer.md | agent | 81 | 1 code example, no output format, 2 vague |
| agents/data-ai/data-scientist.md | agent | 81 | 1 code example, no output format, 2 vague |
| agents/data-ai/llm-architect.md | agent | 81 | 1 code example, no output format, 2 vague |
| agents/data-ai/ml-engineer.md | agent | 79 | 1 code example, no output format, 3 vague |
| agents/core-development/microservices-architect.md | agent | 85 | 1 example, no output format |
| agents/core-development/graphql-architect.md | agent | 85 | 1 example, no output format |
| agents/core-development/websocket-engineer.md | agent | 85 | 1 example, no output format |
| agents/core-development/api-designer.md | agent | 85 | 1 example, no output format |
| agents/quality-assurance/penetration-tester.md | agent | 85 | No examples, reporting section present |
| agents/data-ai/nlp-engineer.md | agent | 85 | 1 code example, no output format |
| agents/data-ai/ai-engineer.md | agent | 85 | 1 code example, no output format |
| agents/data-ai/data-engineer.md | agent | 85 | 1 code example, no output format |
| agents/data-ai/autoresearch-agent.md | agent | 85 | 1 code example, no output format |
| agents/data-ai/mlops-engineer.md | agent | 85 | 1 code example, no output format |
| agents/language-experts/react-specialist.md | agent | 85 | 1 example, no output format |
| agents/language-experts/angular-architect.md | agent | 85 | 1 example, no output format |
| agents/language-experts/kotlin-specialist.md | agent | 85 | 1 example, no output format |
| plugins/code-guardian/agents/reviewer.md | agent | 85 | No examples |
| plugins/api-architect/agents/api-expert.md | agent | 85 | No examples |
| skills/mobile-development/SKILL.md | skill | 90 | No output format specification |
| skills/devops-automation/SKILL.md | skill | 90 | No output format specification |
| skills/frontend-excellence/SKILL.md | skill | 90 | No output format specification |
| skills/git-advanced/SKILL.md | skill | 90 | No output format specification |
| skills/docker-best-practices/SKILL.md | skill | 90 | No output format specification |
| skills/nextjs-mastery/SKILL.md | skill | 90 | No output format specification |
| skills/performance-optimization/SKILL.md | skill | 90 | No output format specification |
| skills/websocket-realtime/SKILL.md | skill | 90 | No output format specification |
| skills/data-engineering/SKILL.md | skill | 90 | No output format specification |
| skills/aws-cloud-patterns/SKILL.md | skill | 90 | No output format specification |
| skills/testing-strategies/SKILL.md | skill | 90 | No output format specification |
| skills/prompt-engineering/SKILL.md | skill | 90 | No output format specification |
| skills/security-hardening/SKILL.md | skill | 90 | No output format specification |
| skills/database-optimization/SKILL.md | skill | 90 | No output format specification |
| skills/kubernetes-operations/SKILL.md | skill | 90 | No output format specification |
| skills/mcp-development/SKILL.md | skill | 90 | No output format specification |
| skills/accessibility-wcag/SKILL.md | skill | 90 | No output format specification |
| skills/react-patterns/SKILL.md | skill | 90 | No output format specification |
| skills/tdd-mastery/SKILL.md | skill | 90 | No output format specification |
| skills/typescript-advanced/SKILL.md | skill | 90 | No output format specification |
| skills/authentication-patterns/SKILL.md | skill | 90 | No output format specification |
| skills/monitoring-observability/SKILL.md | skill | 90 | No output format specification |
| skills/golang-idioms/SKILL.md | skill | 90 | No output format specification |
| skills/ci-cd-pipelines/SKILL.md | skill | 90 | No output format specification |
| skills/redis-patterns/SKILL.md | skill | 90 | No output format specification |
| skills/graphql-design/SKILL.md | skill | 90 | No output format specification |
| skills/django-patterns/SKILL.md | skill | 90 | No output format specification |
| skills/springboot-patterns/SKILL.md | skill | 90 | No output format specification |
| skills/postgres-optimization/SKILL.md | skill | 90 | No output format specification |
| skills/llm-integration/SKILL.md | skill | 90 | No output format specification |
| skills/rust-systems/SKILL.md | skill | 90 | No output format specification |
| skills/microservices-design/SKILL.md | skill | 90 | No output format specification |
| skills/python-best-practices/SKILL.md | skill | 90 | No output format specification |
| skills/continuous-learning/SKILL.md | skill | 100 | None |
| skills/api-design-patterns/SKILL.md | skill | 100 | None |
| skills/manage-skills/SKILL.md | skill | 100 | None |

---

## Security Scan

| Severity | Count |
|----------|-------|
| Critical | 0 |
| High | 0 |
| Medium | 6 |
| Low | 7 |

### Execution Surface Inventory

| Surface | Files |
|---------|-------|
| Hooks config | hooks/hooks.json (25 hook entries, 7 event types) |
| Hook scripts | hooks/scripts/auto-test.js, lint-fix.js, post-edit-check.js, type-check.js, session-start.js, session-end.js, suggest-compact.js, pre-compact.js, learning-log.js, notification-log.js, stop-check.js, smart-approve.py, block-dev-server.js, block-md-creation.js, commit-guard.js, bundle-check.js, pre-push-check.js, prompt-check.js, context-loader.js, secret-scanner.js (20 files) |
| MCP configs | None found |
| Package manifests | None found (no package.json or requirements.txt) |

### Security Findings

| # | Severity | File | Line | Pattern | Description |
|---|----------|------|------|---------|-------------|
| 1 | MEDIUM | hooks/scripts/session-start.js | 5 | File write outside repo | Writes session context to `~/.claude/session-context.json` on every SessionStart event |
| 2 | MEDIUM | hooks/scripts/session-end.js | 5 | Unsanitized stdin → home dir write | Stores `notes` field from stdin directly into `~/.claude/session-context.json` without sanitization |
| 3 | MEDIUM | hooks/scripts/suggest-compact.js | 5 | File write outside repo | Mutates `~/.claude/session-context.json` on every PostToolUse(Bash) call |
| 4 | MEDIUM | hooks/scripts/pre-compact.js | 5–6 | File writes outside repo | Writes two files (`session-context.json`, `compact-log.json`) in `~/.claude/` on every PreCompact event |
| 5 | MEDIUM | hooks/scripts/learning-log.js | 5–6 | File write outside repo + path leak | Writes daily learning logs to `~/.claude/learnings/<date>.json` including absolute cwd path; executes two git child processes |
| 6 | MEDIUM | hooks/scripts/notification-log.js | 5 | Unsanitized stdin → home dir write | Appends raw notification content (unsanitized stdin) to `~/.claude/notification-log.json` |
| 7 | LOW | hooks/scripts/stop-check.js | 5 | File read outside repo | Reads `~/.claude/session-context.json`; read-only but relies on externally-controlled state file |
| 8 | LOW | hooks/scripts/lint-fix.js | 4–37 | Unvalidated path to execFileSync | `filePath` from hook input passed directly to eslint/ruff/gofmt/rustfmt/prettier without path containment check; no shell injection risk but path traversal possible |
| 9 | LOW | hooks/scripts/post-edit-check.js | 4–32 | Unvalidated path to execFileSync | Same concern as lint-fix.js — `filePath` passed to eslint/ruff/go vet/cargo clippy without validation |
| 10 | LOW | hooks/scripts/type-check.js | 23–29 | Derived binary path from input | Resolves `node_modules/.bin/tsc` by walking up from hook-supplied `filePath`; a crafted path could cause attacker-controlled binary to execute |
| 11 | LOW | hooks/scripts/auto-test.js | 5–46 | Unvalidated path in child process | `filePath` drives test discovery and runner selection, passed to execFileSync without repo-boundary validation |
| 12 | LOW | hooks/scripts/smart-approve.py | 45 | Environment variable as config source | Reads `CLAUDE_PROJECT_DIR`, `CLAUDE_SETTINGS_PATH` to load allow/deny patterns; tampered env could redirect to malicious settings file |
| 13 | LOW | hooks/hooks.json | 100–103 | High-frequency hook side effects | `suggest-compact.js` fires on every Bash tool call, performing file I/O on `~/.claude/session-context.json` on each invocation |

---

## Bugs (PR-worthy)

| # | File | Issue | Impact |
|---|------|-------|--------|
| 1 | ALL 223 plugin command files (plugins/**/commands/*.md) | Missing YAML frontmatter — no `name` or `description` fields in `---` blocks | Commands cannot be formally registered; name/description are inferred heuristically from H1 headings or prose |
| 2 | ALL 42 commands/ files (commands/**/*.md) | Same — no YAML frontmatter for name, description, or allowed-tools | Same registration breakage as above |
| 3 | plugins/create-worktrees/commands/worktree-clean.md | Hollow numbered steps — steps 2–4 contain only header labels with no content | Command body is non-functional; provides no actionable instructions to the model |
| 4 | plugins/create-worktrees/commands/worktree-create.md | Hollow numbered steps — steps 1–4 empty | Same — command body is non-functional |
| 5 | plugins/n8n-workflow/commands/create-workflow.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 6 | plugins/web-dev/commands/scaffold-app.md | Hollow numbered steps — steps 1–4 empty | Non-functional command body |
| 7 | plugins/sprint-prioritizer/commands/plan-sprint.md | Hollow numbered steps — steps 1–6 empty | Non-functional command body |
| 8 | plugins/sprint-prioritizer/commands/prioritize.md | Hollow numbered steps — steps 1–6 empty | Non-functional command body |
| 9 | plugins/rapid-prototyper/commands/prototype.md | Hollow numbered steps — steps 1–6 empty | Non-functional command body |
| 10 | plugins/finance-tracker/commands/track-cost.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 11 | plugins/finance-tracker/commands/report-cost.md | Hollow numbered steps — steps 1–6 empty | Non-functional command body |
| 12 | plugins/codebase-documenter/commands/document-all.md | Hollow numbered steps — steps 2–3 empty | Non-functional command body |
| 13 | plugins/data-privacy/commands/audit-pii.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 14 | plugins/data-privacy/commands/anonymize.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 15 | plugins/optimize/commands/optimize-size.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 16 | plugins/optimize/commands/optimize-perf.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 17 | plugins/compliance-checker/commands/check-soc2.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 18 | plugins/compliance-checker/commands/check-gdpr.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |
| 19 | plugins/plan/commands/plan.md | Hollow numbered steps — steps 2–4 empty | Non-functional command body |
| 20 | plugins/plan/commands/estimate.md | Hollow numbered steps — steps 2–4 empty | Non-functional command body |
| 21 | plugins/fix-github-issue/commands/fix-issue.md | Hollow numbered steps — steps 2, 3, 5, 6 empty | Non-functional command body |
| 22 | plugins/ui-designer/commands/implement-design.md | Hollow numbered steps — steps 1–5 empty | Non-functional command body |

---

## Security Fixes (PR-worthy, Medium/Low only)

| # | File | Issue | Suggested Fix |
|---|------|-------|---------------|
| 1 | hooks/scripts/session-end.js | Unsanitized `notes` field from stdin stored in `~/.claude/session-context.json` | Validate/sanitize the `notes` field before writing; strip or truncate to known safe length and character set |
| 2 | hooks/scripts/notification-log.js | Raw stdin notification content appended to home-dir JSON without sanitization | Parse stdin as JSON first, reject entries with unexpected fields; cap log file size explicitly |
| 3 | hooks/scripts/lint-fix.js | `filePath` from hook input passed to linter binaries without path containment | Add `path.resolve()` + check that result starts with `process.cwd()` before passing to execFileSync |
| 4 | hooks/scripts/post-edit-check.js | Same unvalidated path issue as lint-fix.js | Same fix: validate `filePath` is within repo root |
| 5 | hooks/scripts/type-check.js | `tscBin` derived from hook-supplied path may resolve to attacker-controlled binary | After computing `tscBin`, verify it resolves within a known-safe directory (e.g., `node_modules/.bin` under the project root, not an arbitrary parent) |
| 6 | hooks/scripts/auto-test.js | Test file path discovery driven by unvalidated `filePath` | Validate `filePath` is within repo boundary before computing `testFile` |
| 7 | hooks/scripts/smart-approve.py | `CLAUDE_SETTINGS_PATH` env var used to load settings without validation | Verify the resolved path is within `~/.claude/` or the project directory before loading |
| 8 | hooks/scripts/learning-log.js | Writes absolute cwd path in log entries, leaking filesystem layout | Emit relative path or project name rather than absolute `process.cwd()` in log entries |
| 9 | hooks/hooks.json | `suggest-compact.js` fires on every Bash call, causing repeated home-dir I/O | Debounce: check elapsed time since last write before mutating the session context file |

---

## Quality Issues (informational)

| # | File | Issue | Penalty |
|---|------|-------|---------|
| 1 | ALL ~140 agent files | No output format specification in any agent definition | -10 per file |
| 2 | ~120 agent files (all except those with embedded code blocks) | Zero example blocks — no demonstration of expected agent input/output | -15 per file |
| 3 | ~20 agent files (those with only 1 embedded code snippet) | Only one partial example (inline code block, not a full interaction example) | -5 per file |
| 4 | ~265 command files | No `allowed-tools` declaration | -5 per file |
| 5 | ~200 command files | No empty/missing input handling (no branch for "what if user provides nothing") | -10 per file |
| 6 | ~130 command files | No output format specification (no `## Format` or `## Output` section) | -10 per file |
| 7 | agents/orchestration/context-manager.md | 7 vague quantifiers ("relevant" x4, "appropriate" x2, "necessary" x1) | -14 |
| 8 | agents/orchestration/workflow-director.md | 6 vague quantifiers ("relevant" x3, "appropriate" x2, "necessary" x1) | -12 |
| 9 | plugins/ios-developer/commands/create-view.md | 8 vague quantifiers (highest count in command set) | -16 |
| 10 | plugins/ios-developer/commands/add-model.md | 7 vague quantifiers | -14 |
| 11 | agents/data-ai/feature-engineer.md | 5 vague quantifiers | -10 |
| 12 | agents/business-product/legal-advisor.md | 5 vague quantifiers | -10 |
| 13 | agents/business-product/customer-success.md | 5 vague quantifiers | -10 |
| 14 | agents/research-analysis/patent-analyst.md | 5 vague quantifiers | -10 |
| 15 | agents/research-analysis/search-specialist.md | 5 vague quantifiers | -10 |
| 16 | agents/aws-helper/commands/setup-lambda.md | 4 vague quantifiers ("appropriate" x4) | -8 |
| 17 | 33 skill files | No output format specification (continuous-learning, api-design-patterns, manage-skills are the exceptions) | -10 per file |

---

## Cross-Component

**Plugin.json ↔ Command file references**: Each plugin's `.claude-plugin/plugin.json` declares a `commands` array referencing its command `.md` files. These references are consistent — no orphaned plugin.json entries were found pointing to non-existent command files.

**Agent ↔ Skill references**: The 15 specialized-domain agents and most developer-experience agents do not reference any skill files by name. The `manage-skills/SKILL.md` describes the skill system but no agent definitions include an explicit `skills:` field in frontmatter (the field doesn't exist in Claude Code's schema — skills are loaded by name at invocation time). No broken skill references detected.

**Hook ↔ Script references**: `hooks/hooks.json` references all 20 scripts in `hooks/scripts/`. All referenced script files exist. No broken references.

**Hollow command cluster**: 22 command files (mostly in `plugins/plan/`, `plugins/optimize/`, `plugins/compliance-checker/`, `plugins/finance-tracker/`, `plugins/sprint-prioritizer/`, etc.) have numbered steps that are empty placeholder headers. These appear to be a second generation of commands written in a different authoring style than the older, fully-implemented commands. The inconsistency creates a two-tier quality split within the same plugin ecosystem.

**Naming pattern divergence**: Older plugin commands use `# /command-name - Title` H1 as command identifier. Newer commands (batch 1/2, score 25–35) use fully plain text with no H1. Both styles lack YAML frontmatter. The doc-forge, deploy-pilot, and perf-profiler plugins break from this pattern and have proper H1 + ## Output sections, scoring 79–83. These three plugins represent the quality ceiling for command files in the repo.

---

## Recommendation

Security is **REVIEW** — no Critical or High findings. The 6 Medium findings involve home-directory state files accumulating unsanitized data from hook inputs, and the 7 Low findings involve unvalidated file paths passed to linter/test tools. None are immediately exploitable in a standard workflow but represent hardening gaps worth addressing.

NL quality score is **55/100** — below the default threshold of 70. The dominant cause is structural: every one of the 265 command files (plugins and commands/) is missing YAML frontmatter, which applies a -50 penalty to each. A single mechanical fix (adding `---\nname: ...\ndescription: ...\nallowed-tools: [...]\n---` to each command file) would raise the command average from ~38 to ~88 and push the overall score well above 70.

The 22 hollow-step commands are a separate quality gap requiring real content authoring, not just structural fixes.

**REVIEW — submit NL fix PRs for the frontmatter bug (highest impact single fix in the repo) and the hollow-step commands. Flag Medium security findings (unsanitized home-dir writes) in a dedicated issue.**

### Priority Fix Order
1. **Add YAML frontmatter to all command files** — recovers ~50 points per file, ~265 files affected. Template: `---\nname: <command-name>\ndescription: <first-line prose>\nallowed-tools: Bash, Read, Write, Edit, Glob, Grep\n---`
2. **Fill in hollow numbered steps** — 22 commands are non-functional; needs content authoring
3. **Add `## Format` sections** to ~130 commands that lack output format specification
4. **Add example blocks to agents** — all 140 agents lack structured input/output examples; even one example per agent would recover 10 points per file
5. **Sanitize hook stdin writes** — session-end.js and notification-log.js write unsanitized content to home directory (Medium security)
6. **Add path containment checks** to lint-fix.js, post-edit-check.js, type-check.js, auto-test.js (Low security)
