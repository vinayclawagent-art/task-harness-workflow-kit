# Release Candidate Evidence Intake Card

Source package: [[../../Generated-Packages/Task Harness Workflow Kit/README|Task Harness Workflow Kit]]
Loop: [[../../Improvement-Loops/Task Harness Workflow Kit Loop|Task Harness Workflow Kit Loop]]

## When to use

Use this card immediately after [[Release Candidate Trial Kickoff Card]] and before filling [[Release Candidate Trial Packet]] during the next real Mission Control release-candidate QA pass.

This is a blank intake card. It is ready for the next trial; no release evidence has been invented.

## Intake fields

| Field | Fill during live release-candidate pass |
| --- | --- |
| Release candidate / branch | _TBD during live run_ |
| Handoff owner | _TBD during live run_ |
| Source docs reviewed | _TBD during live run_ |
| Claims needing proof | _TBD during live run_ |
| Verification commands or checks | _TBD during live run_ |
| Screenshots / artifacts to attach | _TBD during live run_ |
| Blocking unknowns | _TBD during live run_ |

## Source-link ledger

| Claim or release note line | Required source link | Verification state | Packet destination |
| --- | --- | --- | --- |
| _TBD during live run_ | _Issue / PR / commit / package note_ | _unverified / verified / blocked_ | [[Release Candidate Trial Packet]] |
| _TBD during live run_ | _Issue / PR / commit / package note_ | _unverified / verified / blocked_ | [[Release Candidate Trial Packet]] |
| _TBD during live run_ | _Issue / PR / commit / package note_ | _unverified / verified / blocked_ | [[Release Candidate Trial Packet]] |

## Minimum evidence before packet fill

- [ ] Every public-facing claim has a source URL or explicit blocker.
- [ ] At least one verification command/check is recorded with expected output.
- [ ] Any skipped claim is marked `blocked`, not silently omitted.
- [ ] The handoff owner is named before the trial packet is filled.
- [ ] The promotion card remains blank until the live QA pass completes.

## Copyable handoff block

```markdown
Release Candidate Evidence Intake Card status: ready for packet fill
Release candidate / branch: _TBD during live run_
Claims with source links: _TBD during live run_
Verification checks: _TBD during live run_
Blocked claims: _TBD during live run_
Next artifact: [[Release Candidate Trial Packet]]
No validation evidence was invented in the cron preparation run.
```

## Next action

During the next real release-candidate QA pass, fill this intake card first, then copy its ledger into [[Release Candidate Trial Packet]] and complete [[Harness Promotion Decision Card]] only after the evidence is attached.
