# LinkedIn launch checklist

Everything here is limited to what the repositories show. Do not add user counts, customers or revenue: none are documented.

## Before posting

- [ ] Merge the profile pull request and the project README pull requests you approve.
- [ ] Set the GitHub display name to "Yassine Aqejjaj" and pin: `agentic-sdlc`, `NOVA`, `ORBIT`, `FORGE`, `TrustRail`, `CarePilot`.
- [ ] Upload the 1280x640 social preview image for each repository (Settings, Social preview).
- [ ] Open each demo link below in a private window and confirm it loads.
- [ ] Check the CI badge of each project you will mention. At audit time Fencing Intelligence and TRAIL Academy had failing or unfinished runs: do not feature them until green.
- [ ] Decide whether to publish the Vita case study (private repository) at all.

## Priority projects and the proof to cite

| Order | Project | Message | Proof to cite | Verified demo |
|---|---|---|---|---|
| 1 | Profile and ecosystem (NOVA, ORBIT, FORGE) | "I turn AI strategy into working products" | NOVA's implemented / tested / deployed matrix; ecosystem diagram | https://nova-six-orcin-96.vercel.app · https://orbit-virid-psi-70.vercel.app · https://forge-pied-rho.vercel.app |
| 2 | TrustRail | "Let agents act. Keep control." | Real Docker and CI runs documented in the build status; signed receipts; synthetic sandboxes only | https://trustrail-mu.vercel.app |
| 3 | Agentic SDLC framework | Autonomy is earned by evidence | Ten case studies with cited commits; defects found only by running the real system | https://github.com/yassineaqejjaj/agentic-sdlc |
| 4 | Healthcare: MedGuard AI and M3aya Santé (CarePilot) | AI in healthcare with declared limits | Synthetic data, human approval, explicit "not for real patients" statements | https://carepilot-maroc.vercel.app |
| 5 | Books and TRAIL Academy | The leadership view and the applied training | Book links; platform live in test mode, real payments not open | https://trailacademy.fr |

## Visuals you can use

- Profile banner and ecosystem diagram: `docs/assets/profile-banner.svg` and the Mermaid block in the profile README.
- Lifecycle diagram: `docs/assets/agentic-lifecycle.svg` in `agentic-sdlc`.
- Real screenshots exist for NOVA, TRAIL Academy, CarePilot, MedGuard AI, SimuLearn and ClassMind (each repository's `docs/screenshots`).
- None exist yet for ORBIT, FORGE and TrustRail: capture them from the live demos before posting about them.
- Social preview images: `social-previews/` (generated for this session, one per repository).

## Suggested order

1. Day 1: positioning post with the ecosystem diagram and the three demos.
2. Day 3: TrustRail, with one concrete bug found by a real Docker run.
3. Day 5: Agentic SDLC, with the autonomy levels and one case study.
4. Day 8: healthcare projects, led by the limits, not the features.
5. Day 10: books and TRAIL Academy.

## Wording rules

- Say "prototype", "public beta" or "MVP" exactly as the repository does.
- Say "synthetic data" for every health and education demo.
- Quote the case studies for lessons; do not claim time or cost savings that are not measured.
