# Runbook

This repository exists solely as an end-to-end lifecycle test target.

## What was verified

1. **Repository creation** — `e2e-pipeline-check` was created public, initialized with a README, and left in place for inspection.
2. **Workflow file** — `.github/workflows/e2e-check.yml` with display name "E2E Check" was committed to `main`.
3. **Workflow execution** — the workflow was triggered by pushes to `main` and the resulting runs were polled until completion.
4. **Evidence gathering** — run id, conclusion, job names/outcomes, log output, and the head commit SHA + message were captured.
5. **Log deletion** — the logs for the final run were deleted after evidence capture.
6. **Collaboration pass** — this branch (`update-runbook`) adds this runbook file, and a pull request titled "Update runbook with audit notes" was opened into `main`, carrying a comment review with a line-anchored note beginning "Verified end-to-end:".
7. **Report** — a gist named `e2e-report.md` was created and then updated with the final completed checklist.

## Notes

- This runbook was added specifically so the pull request diff has a concrete line to anchor the review comment against.
