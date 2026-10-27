---
charter_schema: 1
written_by: cadre 0.2.0
skill_pack: mattpocock-skills
---

# Charter

## Tracker
GitHub: host `github.com`, owner `jeredleisey`, repo `cadre-scratch`.

## Owners
| Path | Owner | Note |
| --- | --- | --- |
| `/` | Breck | All of the repo. |

When code moves to another repo, its ownership moves with it to the orchestrator of that repo.

## Merge and deploy
- Merge: the owner (jeredleisey), method `merge`, after review of the pull request. The orchestrator merges only with a grant in the ledger.
- Deploy: none.

## Extra cards
The orchestrator reads this list, so it is prose and not front matter.

| Name | Job | When to use |
| --- | --- | --- |

## Documentation
None. The repo has no docs folder.

## Only the human
- Log in to the tracker command line tool, or switch its account.
- Create, change, or read the value of a secret.
- Delete a repo, a remote tag, or a release.
- Weaken a ruleset or a branch protection, or turn a guard off.
- Change the visibility of the repo.
- Do anything in billing or DNS.

## Needs a grant
- A release tag.
- A change to a repo setting (also a Pages setting) that does not weaken protection.
- A change to a ruleset that keeps or makes stronger the protection.

## Secrets
None.

## Traps
- `main`: no rule requires a pull request. Fix: the human adds a ruleset that requires one.
- `main`: no review is required. Fix: the human requires a review in the ruleset.
- `main`: force push is allowed. Fix: the human blocks force push.
- `main`: the branch can be deleted. Fix: the human blocks deletion.
- `main`: no required status check. Fix: the human adds one when CI exists.
- The hooks guard the Bash tool only, so the branch policy above is the guard that holds.

## Live clones
None.
