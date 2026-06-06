# Release Notes QA Traceability Table Template

Source package: [[../../Generated-Packages/Task Harness Workflow Kit/README|Task Harness Workflow Kit]]
Use with: [[Generated Workflow - Mission Control Release Notes QA]]
Date created: 2026-06-05

## Purpose

This template is the missing handoff artifact for the first real Mission Control release-notes QA trial. It turns each public-facing claim into proof before a release note ships.

## Traceability table

| Release-note claim | User-facing value | Source evidence | Verification output | Risk / rewrite decision |
| --- | --- | --- | --- | --- |
| `<paste bullet>` | `<why users care>` | `<commit/PR/issue/demo>` | `<command + exit code or proof link>` | Keep / rewrite / cut |
| `<paste bullet>` | `<why users care>` | `<commit/PR/issue/demo>` | `<command + exit code or proof link>` | Keep / rewrite / cut |
| `<paste bullet>` | `<why users care>` | `<commit/PR/issue/demo>` | `<command + exit code or proof link>` | Keep / rewrite / cut |

## Go/no-go rubric

- **Go:** every public claim has source evidence and at least one verification/proof link.
- **Go with edits:** evidence exists, but wording overclaims or hides user value.
- **No-go:** any major claim lacks evidence, test output is missing, or unresolved risk would surprise users.

## Copyable handoff block

```markdown
### Release notes QA handoff — <release candidate>
- Release branch / SHA:
- Claims reviewed:
- Claims kept:
- Claims rewritten:
- Claims cut:
- Verification commands:
- Remaining risks:
- Recommendation: Go / Go with edits / No-go
```

## Next action

Attach one filled version of this table to the next Mission Control release candidate, then decide whether the release-notes QA workflow should be promoted into a reusable Mission Control checklist or Hermes skill draft.
