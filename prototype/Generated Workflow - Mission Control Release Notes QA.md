# Generated Workflow: Mission Control Release Notes QA

Source package: [[../../Generated-Packages/Task Harness Workflow Kit/README|Task Harness Workflow Kit]]
Generated from: `workflow-builder.html`
Date: 2026-06-05

## Purpose
Turn each Mission Control release candidate into a consistent release-notes QA pass before publishing or posting about it.

## Trigger
Run when a release branch, changelog draft, or public launch note is ready for final review.

## Inputs
- Release branch or commit range
- Draft release notes / changelog
- Linked issues, PRs, demos, or screenshots
- Test/build output from the release candidate
- Any public proof artifacts that should be referenced

## Required context
- Product promise for the release
- Known user-facing changes
- Risky migrations, auth changes, or background-agent behavior changes
- Previous release-note style examples

## Allowed tools
- Read-only repo inspection for commits, diffs, and test output
- Markdown editing for release notes
- Git commands for status, diff, and commit SHA capture
- Screenshot/demo link inspection when already available locally or in the vault

## Steps
1. Confirm the exact commit range and release branch with `git status --short --branch` and `git rev-parse HEAD`.
2. Map every public-facing changelog bullet to a commit, PR, issue, or artifact.
3. Flag bullets that overclaim, lack proof, or mention implementation details without user value.
4. Rewrite the release note into three sections: `What changed`, `Why it matters`, and `Proof / verification`.
5. Capture verification commands, exit codes, and unresolved risk notes.
6. Produce a final handoff with changed paths, release SHA, proof links, and go/no-go recommendation.

## Output contract
- Clean release-notes markdown
- Traceability table from note bullet → source evidence
- Verification command output summary
- Go/no-go recommendation with remaining risks

## Readiness score
| Dimension | Score | Evidence |
| --- | ---: | --- |
| Trigger clarity | 5/5 | Release branch or changelog-ready event is explicit. |
| Inputs | 5/5 | Commit range, draft notes, linked proof, and test output are listed. |
| Tool boundaries | 4/5 | Allows inspection/editing only; publishing remains outside this harness. |
| Verification | 5/5 | Requires command output, commit SHA, and proof links. |
| Reuse potential | 5/5 | Can run on every Mission Control release candidate. |

Total: **24/25 — ready for trial.**

## First trial checklist
- [ ] Run this against the next Mission Control release candidate.
- [ ] Attach the generated traceability table to the release PR or package note.
- [ ] If the same gaps repeat twice, convert this workflow into a promoted skill or Mission Control checklist.
