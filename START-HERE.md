# Start here

One profile, one question: **when an AI agent acts on a human's behalf, how do you tell a legitimate agent from fraud, without blocking the legitimate one?**

That question runs through every repo here, in three layers.

## The three layers

| Layer | Question it answers | Start with |
|---|---|---|
| Measure it | How often do fraud models fail legitimate agents? | [agentrisk](https://github.com/RishabhPande/agentrisk) |
| Fix it | How do you verify who authorized an agent, and what it may do? | [know-your-agent](https://github.com/RishabhPande/know-your-agent) |
| Evaluate it | How do you test any fraud detector, honestly, with cost in mind? | [fraud-eval](https://github.com/RishabhPande/fraud-eval) |

## If you have 30 seconds

- **First-time visitor:** read the agentrisk headline. A standard fraud model declines 94.6 percent of legitimate agent purchases. AgentGate cuts that to 1.7 percent, and stops 92.7 percent of laundering and 70.2 percent of hijacks. Those are benchmark numbers on synthetic sessions, not production numbers.
- **Hiring manager:** Sr. Director of Data Science at Socure, leading real-time fraud ML. The code here is the public, synthetic-data half of that work. The production half is not here, and is not claimed to be.
- **EB1A reviewer / peer:** 16 peer reviews completed, listed on the profile README, 15 posted on Web of Science as of Nov 10, 2026. Papers are under peer review, 0 published yet, with a goal of 2 journals plus 2 conferences. Preprints are on Zenodo, and are labeled as preprints, not as peer-reviewed work.
- **Fellow ML engineer:** everything is pure Python or numpy only where stated, with tests. GNN-fraud-ring-detection has 261 tests, fraud-eval has 25, know-your-agent has 159. Start with the quickstart in each README, it runs in under a minute.

## Repo map, no overlap hidden

- **agentrisk:** the benchmark and the paper. 9 session classes, Legacy vs AgentGate, 5 seeds.
- **know-your-agent:** the toolkit that implements the fix. Credentials, delegation chains, revocation, signed audit trail, FastAPI demo.
- **fraud-eval:** the evaluator. 20-case smoke test in v0.1.0, cost-aware metrics, counterfactual module. The 190-case version is a draft, not shipped.
- **GNN-fraud-ring-detection:** graph networks from scratch, pure Python, zero dependencies, for fraud rings. The flagship for learning GNNs.
- **fraud-rings:** the ring generator and shared-attribute linking. Pairs with the GNN repo, it makes the rings, the GNN repo learns them.
- **stream-fraud:** streaming scoring and drift detection, PSI and KS, 20 seeds.
- **Time-series-anomaly-detection:** transformer autoencoder for collective and contextual anomalies.
- **ID-document-forgery-detection-CV-:** classic image forensics on synthetic ID cards.
- **agentic-fraud-investigator:** multi-agent case investigation, offline with a mock LLM.
- **agentstats:** run-to-run variance and significance tests for agent benchmarks. A single run can crown the wrong winner.
- **agent-retry-rodeo:** agent recovery under fault injection, with replay.
- **memory-poison-lab:** agent memory poisoning, four attack classes, defenses, and repair. Open challenge in issue 1.
- **tiny-ml-lab:** one classic ML algorithm a day, numpy only, workbooks to fill in.
- **feature-contracts:** reproduction package for the feature-contracts manuscript, public datasets only.

Older repos from 2018, UFC data analysis, churn, diabetes, breast cancer, and others, are early learning work. They are left public as history, they are not the current story.

## What is not here

- No Socure production data, no real transactions, no real PII.
- No published peer-reviewed paper yet, as of Nov 5, 2026. Preprints and submissions are labeled as such.
- No stars bought, no followers bought, no bots. Stars are 0 on the six tracked repos as of Nov 1, 2026, except stream-fraud with 1 star. That is the honest baseline.

## Consistency

- Name everywhere: Rishabh Pande.
- ORCID iD wherever a field exists: 0009-0004-1901-7109.
- Paper bylines: Independent Researcher. Employment: Socure. That difference is deliberate, and is stated on the profile README.
- Hugging Face: RishabhPande, datasets fraud-eval and agentrisk, Spaces for the leaderboard, the arena, and the AgentRisk demo.
- Google Scholar: Rishabh Pande, Socure, interests Machine Learning, AI Fraud Detection, Risk and Compliance, Neural networks.
- ORCID: Rishabh Pande, Sr. Director of Data Science at Socure, peer review listed for Knowledge-Based Systems, Works include the FATT patent, the Risk DecisionAI patent, AgentRisk, and fraud-eval. GNN-fraud-ring-detection is not yet listed as an ORCID Work, that gap is known.
- Zenodo: AgentRisk DOI 10.5281/zenodo.23477625, fraud-eval v0.1.0 DOI 10.5281/zenodo.23695132, GNN v1.1.0 DOI 10.5281/zenodo.23749421.

## How to contribute

Pick a repo, read its CONTRIBUTING.md if it has one, open an issue first for anything larger than a typo. Good first places: tiny-ml-lab workbooks, memory-poison-lab issue 1 and issue 3, fraud-eval new cases once the freeze gates clear.
