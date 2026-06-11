# Task Harness Workflow Kit Prototype

Open `workflow-template.md` as the reusable harness skeleton. For a guided fill-in form that generates `workflow.md`, open `workflow-builder.html` in a browser.

## Worked examples

- [[Worked Example - X Artifact Factory Frequent Improver]] — applies the harness shape to this cron-safe artifact improvement job, including trigger, loaded context, allowed tools, steps, output contract, and verification checklist.
- [[Generated Workflow - Mission Control Release Notes QA]] — archives the first builder-generated `workflow.md` shape for a recurring VinClawLabs release-note QA pass, including readiness scoring and trial checklist.
- [[Release Notes QA Traceability Table Template]] — supplies the first fillable claim → evidence → verification table for the next release-candidate QA handoff.
- [[Harness Promotion Decision Card]] — converts the next release-candidate trial into a promote / iterate once / retire decision for the workflow harness.
- [[Release Candidate Trial Packet]] — orders the generated workflow, traceability table, decision card, and copyable release handoff into one fillable proof packet for the next real release candidate.
- [[Release Candidate Evidence Intake Card]] — captures source links, verification checks, blockers, and handoff owner after kickoff and before the trial packet is filled.
- [[Release Candidate Post-Trial Debrief Template]] — records what worked, what failed, the evidence-backed decision, and exact patch queue after the next real release-candidate QA pass.

## Next iteration

Use [[Release Candidate Evidence Intake Card]] after the kickoff card and before [[Release Candidate Trial Packet]] on the next Mission Control release candidate, then complete [[Release Candidate Post-Trial Debrief Template]] before updating README, workflow-builder, skill-draft, or release handoff wording.

## What it demonstrates
A lightweight workflow.md template for turning recurring agent tasks into repeatable harnesses before promoting them into full Hermes skills.

## How to use
Open `workflow-builder.html`, fill the required fields until the readiness bar says the harness is ready for trial, then copy the generated markdown into the target project. Use `workflow-template.md` when a plain text-only version is preferred.

## Next iteration ideas
- Run [[Generated Workflow - Mission Control Release Notes QA]] during the next real release candidate and fill [[Release Notes QA Traceability Table Template]] for the release PR or package note.
- Complete [[Harness Promotion Decision Card]] after the traceability table so the trial has an explicit promote / iterate / retire outcome.
- Fill [[Release Candidate Trial Packet]] as the canonical release-candidate proof packet before updating the package changelog with validation evidence.
- Fill [[Release Candidate Evidence Intake Card]] first so the trial packet gets source-backed claims instead of reconstructed notes.
- Fill [[Release Candidate Post-Trial Debrief Template]] after the trial so promotion, pilot-only, iterate, hold, or retire decisions are evidence-backed and patch-ready.
- Add downloadable markdown export if browser copy/paste proves too fragile.
- Link one completed release QA run back into the package note.
