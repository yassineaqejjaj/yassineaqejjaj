# GitHub portfolio: settings that need GitHub's web UI

The README and static portfolio files have been committed. The items below are repository/profile **settings**, not text files. The current connected GitHub actions can read these settings but do not expose the administrative operations needed to change them.

## 1. Activate the portfolio site

1. Open [profile repository Pages settings](https://github.com/yassineaqejjaj/yassineaqejjaj/settings/pages).
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Select branch **main** and folder **/docs**, then **Save**.
4. Check the deployment status in the Pages settings and GitHub Actions before publishing a public site link.
5. Once activated, the expected default GitHub Pages URL is `https://yassineaqejjaj.github.io/yassineaqejjaj/` (verify that it resolves before using it).

Source file: [docs/index.html](index.html). It has responsive layouts, accessible navigation and existing product imagery; no tracking scripts.

## 2. Pin six representative repositories

On [the GitHub profile](https://github.com/yassineaqejjaj), select **Customize your pins**. Recommended order:

1. NOVA — platform engineering and agent orchestration
2. ORBIT — governed context, memory, RAG
3. FORGE — evaluation and testing
4. medguard-ai — regulated-industry testing product
5. SimuLearn — voice simulation and human review
6. ClassMind — education AI and deterministic validation

The full ten projects remain linked from the README; pinning is for fast scanning, not a complete inventory.

## 3. Set repository descriptions and topics

On each repo, use the **About** edit control to set description, topics and a website URL where a verified deployed preview exists. The descriptions must remain faithful to the code and its current maturity.

| Repo | Suggested description | GitHub topics |
|---|---|---|
| NOVA | Multi-agent AI product orchestration with versioned skills, human approval and structured artifacts | `agentic-ai` `multi-agent-systems` `langgraph` `ai-agents` `product-engineering` |
| ORBIT | Governed context and versioned memory for agents: hybrid RAG, ACLs and traceability | `context-engineering` `rag` `ai-memory` `vector-search` `access-control` |
| FORGE | Reproducible AI agent evaluations, benchmarks, human review and regression gates | `llm-evaluation` `ai-testing` `llm-as-a-judge` `agent-evaluation` `observability` |
| medguard-ai | Healthcare AI assurance MVP for synthetic testing, human review and release gates | `healthcare-ai` `ai-evaluation` `llm-testing` `human-in-the-loop` `healthtech` |
| SimuLearn | Synthetic patient simulation MVP for conversational healthcare training | `healthcare-training` `voice-ai` `simulation` `education` `mvp` |
| ClassMind | Teacher-reviewed skill analytics and adaptive mathematics exercises (French collège MVP) | `edtech` `education-ai` `adaptive-learning` `fastapi` `react` |
| CarePilot | Administrative patient journey coordination with human-reviewed AI suggestions | `healthtech` `patient-journey` `workflow-automation` `fastapi` `human-in-the-loop` |
| TRAIL-Academy | Professional AI learning platform under development; live integrations not validated | `ai-education` `elearning` `nextjs` `learning-management-system` `typescript` |
| fencing-intelligence | Experimental fencing video analysis and human-validated statistics | `computer-vision` `sports-analytics` `fencing` `video-analysis` `python` |
| apex-f1-pitwall | Independent F1 telemetry, race replay and deterministic strategy what-if simulations | `formula-one` `telemetry` `sports-analytics` `openf1` `javascript` |

Set URLs only for repos with confirmed deployment. A local demo is **not** a hosted product.

## 4. Social preview images

Repository **Settings > Social preview** accepts image uploads. A Markdown/SVG banner in a README does not update this setting. Use a 1280×640 PNG image with the name, one-sentence outcome and one readable visual for each priority platform. Only use authentic product screenshots for product previews, and avoid logos of client organizations without permission.

## 5. Owner decisions needed

- Check ownership and license rights before applying an open-source license to a repo. Visibility **public** is not itself an open-source license.
- Turn on security/secret scanning features that are available to the account, enable branch protection/rulesets where appropriate, and verify dependencies are free of unresolved critical advisories before shipping.
- For Fencing Intelligence, track the current remediation in [security issue #2](https://github.com/yassineaqejjaj/fencing-intelligence/issues/2).
- Record demos (screen + narration) and attach their actual URLs; do not write placeholders pretending the video exists.

## 6. Keep it current

Every release: update the status, link the tested commit and CI run, publish any benchmark with its inputs and ground truth, and review broken preview URLs. Do not change mock/demo labels until live integrations are tested.
