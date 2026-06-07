# Release Candidate Trial Packet

Use this packet during the next real Mission Control release-candidate pass. It bundles the generated workflow, the traceability table, and the promotion card into one ordered handoff so the trial produces evidence and a decision without fabricating proof.

Source package: [[../../Generated-Packages/Task Harness Workflow Kit/README|Task Harness Workflow Kit]]  
Loop: [[../../Improvement-Loops/Task Harness Workflow Kit Loop|Task Harness Workflow Kit Loop]]

## When to use

- A Mission Control release candidate is ready for release-note QA.
- The operator has the release PR, changelog, screenshots or demo notes, and known-issues list available.
- The goal is to decide whether [[Generated Workflow - Mission Control Release Notes QA]] should become a repeatable harness.

## Packet steps

| Step | Artifact | Fill during trial | Done |
| --- | --- | --- | --- |
| 1 | [[Generated Workflow - Mission Control Release Notes QA]] | Confirm trigger, inputs, allowed tools, verification commands, and output contract still fit the release candidate. | ☐ |
| 2 | [[Release Notes QA Traceability Table Template]] | Map every release-note claim to PRs, commits, screenshots, docs, or remove/soften unsupported claims. | ☐ |
| 3 | [[Harness Promotion Decision Card]] | Record promote / iterate once / retire after the traceability pass. | ☐ |
| 4 | Release handoff | Paste the copyable block below into the release handoff and link the filled evidence artifacts. | ☐ |

## Release-candidate fields

| Field | Value |
| --- | --- |
| Release candidate / PR | _TBD during live run_ |
| Release owner | _TBD_ |
| QA operator | _TBD_ |
| Changelog source | _TBD_ |
| Evidence table link | _TBD_ |
| Promotion card link | _TBD_ |
| Final decision | ☐ promote harness ☐ iterate once ☐ retire |

## Minimum evidence checklist

- [ ] Every user-visible claim links to a PR, commit, issue, screenshot, demo note, or docs page.
- [ ] Unsupported claims are removed, softened, or moved to known limitations.
- [ ] At least one verification/review action is recorded with result and timestamp.
- [ ] Known risks and owner follow-ups are included in the handoff.
- [ ] The promotion decision is filled after evidence review, not before.

## Copyable release handoff block

```markdown
### Release Notes QA Harness Trial
- Release candidate / PR:
- Workflow used: [[Generated Workflow - Mission Control Release Notes QA]]
- Evidence table: [[Release Notes QA Traceability Table Template]]
- Promotion decision: [[Harness Promotion Decision Card]]
- Claims changed or removed:
- Verification result:
- Final harness decision: promote | iterate once | retire
- Follow-up owner:
```

## Changelog line to paste after the real run

```markdown
- YYYY-MM-DD: Filled [[Task Harness Workflow Kit/Release Candidate Trial Packet]] for `<release candidate>` and recorded the harness decision in [[Task Harness Workflow Kit/Harness Promotion Decision Card]].
```

## Next action

During the next release-candidate QA run, duplicate or fill this packet, then attach the completed handoff block to the release handoff and package changelog. This artifact is ready for the next trial; no validation evidence has been invented.
