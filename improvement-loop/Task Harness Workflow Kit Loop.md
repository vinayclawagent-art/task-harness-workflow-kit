---
type: improvement-loop
status: active
package: "[[Task Harness Workflow Kit]]"
github_repo: "https://github.com/vinayclawagent-art/task-harness-workflow-kit"
cadence: nightly
last_improved: 2026-06-08
next_focus: Use the kickoff card, then fill [[Release Candidate Evidence Intake Card]] during the next release-candidate QA pass before copying source-backed claims into the trial packet.
tags: [improvement-loop, x-artifact-factory, agent-workflows]
---

# Task Harness Workflow Kit Loop

## Current objective
Turn [[Claude Code Workflows as Task Harnesses]] into a reusable, inspectable artifact package that can improve VinClawLabs agent workflows.

## Latest improvement
- 2026-06-04: Created package, markdown prototype, skill draft, and repo mirror.
- 2026-06-04: Added [[../Prototypes/Task Harness Workflow Kit/Worked Example - X Artifact Factory Frequent Improver]] so the harness has a real cron-safe artifact-factory example.
- 2026-06-04: Added `workflow-builder.html`, a browser form that generates a copyable `workflow.md` harness with readiness scoring.
- 2026-06-05: Archived [[../Prototypes/Task Harness Workflow Kit/Generated Workflow - Mission Control Release Notes QA]] as the first builder-generated workflow for a recurring VinClawLabs release-note QA pass.
- 2026-06-05: Added [[../Prototypes/Task Harness Workflow Kit/Release Notes QA Traceability Table Template]] so the first real release-candidate pass has a ready claim-to-evidence handoff artifact.
- 2026-06-06: Added [[../Prototypes/Task Harness Workflow Kit/Harness Promotion Decision Card]] so the first release-candidate trial produces a promote / iterate once / retire decision.
- 2026-06-06: Added [[../Prototypes/Task Harness Workflow Kit/Release Candidate Trial Packet]] to sequence the generated workflow, traceability table, decision card, and copyable release handoff for the next real trial.

- 2026-06-07: Added [[../Prototypes/Task Harness Workflow Kit/Release Candidate Trial Kickoff Card]] so the next real trial starts with scope, guardrails, evidence expectations, and a no-fabrication handoff prompt.
- 2026-06-08: Added [[../Prototypes/Task Harness Workflow Kit/Release Candidate Evidence Intake Card]] to capture source links, verification checks, blockers, and handoff owner before the release trial packet is filled.

## Next focus
- Use the kickoff card, then fill [[../Prototypes/Task Harness Workflow Kit/Release Candidate Evidence Intake Card]] during the next release-candidate QA pass before copying source-backed claims into the trial packet.
- Keep the card blank until a real trial fills actual outputs.