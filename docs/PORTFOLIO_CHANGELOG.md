# Portfolio changelog

Date: 2026-10-31. Nothing in the pull requests below is merged. Application code, workflows and tests were not modified anywhere, so application tests were not run; verification was limited to documentation checks.

## Repository overview

| Repository | Description | Topics | Status (from the repo) | Demo |
|---|---|---|---|---|
| NOVA | Personal AI product agent: orchestration | agentic-ai, ai-agents, fastapi, langgraph, llm, orchestration | Public beta | https://nova-six-orcin-96.vercel.app |
| ORBIT | Governed context and memory engine | ai-agents, agent-memory, context-engineering, rag, access-control, llm | Public beta, not validated for production | https://orbit-virid-psi-70.vercel.app |
| FORGE | AI agent evaluation platform | ai-agents, llm-evaluation, evals, benchmarking, observability, llm | Public beta | https://forge-pied-rho.vercel.app |
| TrustRail | Policies, approvals and signed receipts for agent actions | ai-agents, agent-security, authorization, audit, mcp, nextjs | Prototype (synthetic sandboxes) | https://trustrail-mu.vercel.app |
| TRAIL Academy | AI training platform | ai-education, edtech, nextjs, supabase, stripe | Prototype, live in test mode | https://trailacademy.fr |
| CarePilot (M3aya Santé) | Patient-journey coordination | healthcare-ai, patient-journey, human-in-the-loop, nextjs, typescript | MVP, fictional data | https://carepilot-maroc.vercel.app |
| MedGuard AI | Healthcare AI assurance | healthcare-ai, ai-safety, llm-evaluation, ai-governance, responsible-ai | MVP | none |
| SimuLearn | Healthcare training simulations | healthcare-education, simulation, voice-ai, ai-education, fastapi | Mock-mode MVP | none |
| ClassMind | Teacher-reviewed learning analytics | ai-education, edtech, learning-analytics, nextjs, typescript | MVP, fictitious data | none |
| Fencing Intelligence | Fencing video analysis | fencing, computer-vision, sports-analytics, video-analysis, self-hosted | Experimental | https://fencing-intelligence.vercel.app |
| APEX F1 Pitwall | Race data and strategy simulation | formula1, data-visualization, sports-analytics, strategy-simulation | Estimates, not predictions | https://apex-f1-pitwall.vercel.app |
| agentic-sdlc | Framework for AI-assisted delivery | agentic-ai, sdlc, ai-coding-agents, software-engineering, ai-governance, framework | Working v0.1 | n/a |

Recommended pins: `agentic-sdlc`, `NOVA`, `ORBIT`, `FORGE`, `TrustRail`, `CarePilot`. Repository names were not changed.

## Changes by repository

All project pull requests change **only `README.md`**, by addition: an "At a glance" block and the missing standard sections. Existing content was kept. Fencing Intelligence and APEX F1 had thin READMEs, so their headings were reorganized (a few lines replaced).

| Repository | Pull request | Added | Checks done | Remaining |
|---|---|---|---|---|
| Profile (`yassineaqejjaj`) | [#2](https://github.com/yassineaqejjaj/yassineaqejjaj/pull/2) | New README: hero, about, six featured projects, ecosystem diagram, evidence, capabilities, publications, connect. `docs/PORTFOLIO_AUDIT.md`, `docs/LINKEDIN_LAUNCH.md`, this file | 44 URLs return 200; Mermaid parses; local assets exist | Review wording |
| NOVA | [#67](https://github.com/yassineaqejjaj/NOVA/pull/67) | At a glance, stack, status, limits, roadmap link, licence note | Links and 1 Mermaid block | No licence file; test fixtures to confirm |
| ORBIT | [#31](https://github.com/yassineaqejjaj/ORBIT/pull/31) | At a glance, stack, screenshots note, limits, licence note (French) | Links and 1 Mermaid block | No screenshots; no licence file |
| FORGE | [#25](https://github.com/yassineaqejjaj/FORGE/pull/25) | At a glance, tests and quality, status, limits, roadmap note (French) | Links and 1 Mermaid block | No screenshots; no licence file |
| TrustRail | [#1](https://github.com/yassineaqejjaj/TrustRail/pull/1) | CI badge, at a glance, problem, solution, features, architecture, stack, tests, status, limits, roadmap | Links resolve | No screenshots; package.json says UNLICENSED |
| TRAIL Academy | [#1](https://github.com/yassineaqejjaj/TRAIL-Academy/pull/1) | CI badge, short French summary and section map | Links; 4 Mermaid blocks parse | CI had failing runs; no licence |
| CarePilot | [#2](https://github.com/yassineaqejjaj/CarePilot/pull/2) | CI badge, at a glance with the M3aya Santé mapping, section map | Links, images; 1 Mermaid block | No licence file |
| MedGuard AI | [#1](https://github.com/yassineaqejjaj/medguard-ai/pull/1) | At a glance | Links and images | None noted |
| SimuLearn | [#1](https://github.com/yassineaqejjaj/SimuLearn/pull/1) | At a glance (French) | Links and images | No licence file |
| ClassMind | [#2](https://github.com/yassineaqejjaj/ClassMind/pull/2) | CI badge, at a glance (French) | Links and images | No licence file |
| Fencing Intelligence | [#3](https://github.com/yassineaqejjaj/fencing-intelligence/pull/3) | Full standard structure; CI failure stated honestly | Mermaid parses; paths exist | **CI fails** (pytest collection error); not fixed |
| APEX F1 Pitwall | [#1](https://github.com/yassineaqejjaj/apex-f1-pitwall/pull/1) | Full standard structure | Mermaid parses; cover exists | No licence file; roadmap not documented |

## Done directly earlier in this session (already on `main`)

- Repository descriptions and topics (table above), `agentic-sdlc` marked as a template.
- A footer linking each project to the Agentic SDLC framework and its case study.
- The `agentic-sdlc` repository: framework, templates, ten case studies, companion page for the books.
- The NOVA architecture diagram fix (reserved Mermaid word `graph`).
- Two book cards and the books section in the profile README.

## Not done

- CI on TRAIL Academy (not investigated).
- Fencing Intelligence CI is fixed in [pull request #4](https://github.com/yassineaqejjaj/fencing-intelligence/pull/4), not merged. It updates Next.js to 16.4.1 for critical advisories, so it changes the deployed app and deserves a review.
- Real screenshots for ORBIT, FORGE, TrustRail, Fencing, APEX.
- Choosing licences; confirming the JWT-shaped test fixtures in NOVA and ORBIT.
- GitHub display name, pinning, social preview upload, release `v0.1.0`.
- The Vita case study (private repository): withheld pending the owner's decision.
- No merge, deployment or rename was performed.
