# Portfolio audit

Date: 2026-10-31. Scope: the public GitHub profile `yassineaqejjaj` and its 12 public repositories. One private repository exists and was **not read for publication and not modified**.

Method: README and metadata read through the GitHub API and local clones; every URL in the profile README requested over HTTP; CI status read from GitHub Actions; demo URLs requested; repositories scanned for secret patterns and tracked `.env` files. Nothing was executed from the repositories. Items not checked are listed as such.

## Summary

| Area | Finding | Severity |
|---|---|---|
| Profile README | All 35 links return HTTP 200. Structure was long and had no quick path for a 30-second reader. Fixed in this change set. | Medium |
| Naming | GitHub display name is "iaseen"; README says "Yassine Aqejjaj". Commercial names differ from repository names (CarePilot is branded "M3aya Santé"; ORBIT and FORGE are referred to as "Nova Context" and "Nova Evals" only in NOVA's README). | Medium |
| CI | `fencing-intelligence` fails CI on its three latest runs (pytest collection error in `test_intelligence.py`). `TRAIL-Academy` shows failures on recent runs. NOVA and TRAIL had runs still in progress at audit time. | High |
| Screenshots | Real screenshots exist for NOVA, TRAIL Academy, CarePilot, MedGuard AI, SimuLearn, ClassMind. None found for ORBIT, FORGE, TrustRail (empty screenshots folder), Fencing Intelligence, APEX F1. | Medium |
| Demos | All six homepage demo URLs return HTTP 200. Whether each demo is feature-complete was not verified. | Low |
| Secrets | No private keys, cloud keys or live tokens found by pattern scan. See "Secret-like content" below. | Low |
| Licences | Present on MedGuard AI, Fencing Intelligence (Apache-2.0) and agentic-sdlc (MIT). Absent on the other nine. Choosing a licence is the owner's decision. | Medium |
| Discoverability | Topics were missing on every repository and three descriptions were empty. Fixed. | Medium |
| Documentation | Several READMEs are strong (MedGuard, SimuLearn, ClassMind, TRAIL Academy) and several are thin (Fencing, APEX). Language is mixed French and English across repositories. | Medium |

## Repository inventory

| Repository | Status claimed in repo | Demo | Latest CI at audit | Screenshots | Licence |
|---|---|---|---|---|---|
| NOVA | Prototype | Yes (200) | In progress; previous run cancelled | Yes | None |
| ORBIT | Prototype | Yes (200) | Success | No | None |
| FORGE | Prototype | Yes (200) | Success | No | None |
| TrustRail | Prototype, synthetic sandboxes | Yes (200) | Success | No | None |
| TRAIL Academy | In development; live payments not validated | Yes (200) | In progress; recent failures | Yes | None |
| CarePilot (M3aya Santé) | MVP, fictional data | Yes (200) | Success | Yes | None |
| MedGuard AI | MVP | No | Success | Yes | Apache-2.0 |
| SimuLearn | Mock-mode MVP | No | Success | Yes | None |
| ClassMind | MVP, fictitious data | No | Success | Yes | None |
| Fencing Intelligence | Experimental | Yes (200) | **Failure** | No | Apache-2.0 |
| APEX F1 Pitwall | Estimates, not predictions | Yes (200) | Success | No | None |
| agentic-sdlc | Working framework v0.1 | n/a | No workflow | n/a | MIT |

"Status claimed" is taken from each README. No status was upgraded to Beta or Production, because no repository documents production use, users or customers.

## Secret-like content

- `NOVA` and `ORBIT` contain `contracts/claims/case_administrator.json` with JWT-shaped strings. The issuer is an `.test` domain, the subject is an example address and the key id is a test key, so these look like **test fixtures** signed with a test key and already expired. They should be confirmed as fixtures by the owner and, ideally, generated at test time instead of committed.
- `NOVA` has a fake GitHub-token-shaped string in an end-to-end test (`engineering.spec.ts`). It is a test value.
- No tracked `.env` files were found in any repository.
- This was a pattern scan, not a full secret audit. History was not scanned.

## Stale or inconsistent information found

- TrustRail's `docs/BUILD_STATUS.md` says the repository was pushed as **private**; it is public today. The `package.json` licence field says `UNLICENSED` and there is no LICENSE file.
- TrustRail's README refers to the repository as `yassineaqejjaj/trustrail` in places; the actual name is `TrustRail`.
- TRAIL Academy documents two different live URLs (`trail-academy.vercel.app` in repository metadata, `trailacademy.fr` in the README). Both return HTTP 200.
- TRAIL Academy's test counts differ between documents; the README states 514 unit tests and 23 end-to-end flows, which were not re-run.
- NOVA's status matrix is dated 13 October 2026 and notes a deployment freeze; it should be read as of that date.

## Claims that were not verified

- Test counts and coverage quoted in READMEs were not re-run.
- Demo functionality beyond HTTP 200 was not exercised.
- No metric about users, customers or revenue is present in any repository, and none was added.

## Recommendations and status

| # | Recommendation | Status |
|---|---|---|
| 1 | Rebuild the profile README around positioning, featured projects, ecosystem, method, evidence, publications | Done in this change set |
| 2 | Add topics and descriptions | Done earlier |
| 3 | Add cross-links between projects and the framework | Done earlier |
| 4 | Harmonize project READMEs without removing existing content | Done on branches, pull requests pending review |
| 5 | Fix failing CI on Fencing Intelligence and TRAIL Academy | **Not done**: this changes code, outside the scope of documentation work |
| 6 | Add real screenshots for ORBIT, FORGE, TrustRail, Fencing, APEX | **Not done**: requires running or capturing real interfaces |
| 7 | Choose licences for the nine unlicensed repositories | Owner decision |
| 8 | Confirm the JWT-shaped fixtures and regenerate them at test time | Owner decision |
| 9 | Align the GitHub display name, then pin six repositories | Manual on GitHub |
| 10 | Decide whether to rename repositories to match commercial names | Not done on purpose; no rename without instruction |

## Pinned repositories (recommended)

`agentic-sdlc`, `NOVA`, `ORBIT`, `FORGE`, `TrustRail`, `CarePilot`.

## Topics

See the table in `docs/PORTFOLIO_CHANGELOG.md`.
