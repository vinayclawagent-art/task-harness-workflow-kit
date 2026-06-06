# Harness Promotion Decision Card

Use this after [[Release Notes QA Traceability Table Template]] is filled in a real release-candidate run. It converts a one-off workflow trial into a clear promote/iterate/retire decision for the harness.

## Decision summary

| Field | Value |
| --- | --- |
| Workflow name | Mission Control Release Notes QA |
| Release candidate / PR | _TBD during live run_ |
| Evidence table link | _TBD_ |
| Harness operator | _TBD_ |
| Decision | ☐ promote to repeatable workflow ☐ iterate once ☐ retire |
| Next owner | _TBD_ |

## Promotion gates

| Gate | Pass evidence required | Status |
| --- | --- | --- |
| Trigger clarity | The release stage that should invoke the harness is explicit | ☐ pass ☐ fail ☐ n/a |
| Input completeness | Changelog, PRs, screenshots, known issues, and target audience are linked or marked absent | ☐ pass ☐ fail ☐ n/a |
| Claim traceability | Every release-note claim maps to source evidence or is removed | ☐ pass ☐ fail ☐ n/a |
| Verification command | At least one real check/review action is recorded with result | ☐ pass ☐ fail ☐ n/a |
| Handoff quality | Final notes include changes made, unresolved risks, and next owner | ☐ pass ☐ fail ☐ n/a |
| Reuse signal | The workflow saved time or prevented a likely release-note miss | ☐ pass ☐ fail ☐ n/a |

## Decision rubric

- **Promote to repeatable workflow** when the gates pass and the release handoff is clearer than the previous manual process.
- **Iterate once** when the workflow is useful but one gate needs a stronger field, instruction, or example.
- **Retire** when the harness adds process overhead without catching errors or clarifying ownership.

## Copyable handoff block

```markdown
### Harness promotion decision
- Workflow:
- Release candidate / PR:
- Evidence table:
- Gate failures:
- Decision: promote | iterate once | retire
- Harness change requested before next run:
```

## Next attachment step

During the next release-candidate QA run, fill this card after the traceability table and attach the handoff block to the release handoff or package changelog.
