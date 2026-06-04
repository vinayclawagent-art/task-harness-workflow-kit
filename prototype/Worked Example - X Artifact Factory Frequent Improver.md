# Worked Example: X Artifact Factory Frequent Improver

Source package: [[../../Generated-Packages/Task Harness Workflow Kit/README|Task Harness Workflow Kit]]

## Trigger
A scheduled frequent-improver run finds active artifact loops with `cadence` or `improvement_cadence` set to nightly/frequent/high and needs to make visible, bounded progress without creating new cron jobs.

## Inputs
- `Artifacts/Improvement-Loops/*.md`
- `Artifacts/Generated-Packages/*/README.md`
- Existing isolated repos under `/home/vinclaw/GitRepos/x-artifact-repos/`
- Existing GitHub auth from `gh`, `GITHUB_TOKEN`, `GH_TOKEN`, or `~/.hermes/.env`

## Context to load
- `x-artifact-factory`
- `obsidian`
- `github-auth`
- `github-repo-management`

## Allowed tools
- Filesystem: read and update only the selected package, prototype, skill draft, loop, and repo-registry files.
- Terminal/build: `git status`, `git add`, `git commit`, `git push`, and copy/sync commands for isolated repos.
- Network: GitHub push/API only for repos already linked by package frontmatter or created as isolated artifact repos.

## Steps
1. Select at most two active cadence-matching loops/packages.
2. For each item, convert one backlog line into a concrete artifact change.
3. Mirror changed package/prototype/skill/loop files into the isolated repo.
4. Commit and push each isolated repo first so visible GitHub activity exists.
5. Commit the x-intel vault with an `x-factory: improve <artifact-name>` message.
6. Report changed paths, vault SHA, repo URL, and repo SHA.

## Output contract
- Changed artifact paths
- Which TODO moved to done
- Vault commit SHA
- Per-repo commit SHA and GitHub URL

## Verification checklist
- [ ] The selected loop remains `status: active`.
- [ ] No cron files were created, updated, or removed.
- [ ] Git status was checked for the vault and each repo.
- [ ] The final report is based on real commit/push output.
