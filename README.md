# Rishabh Pande

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rishabhpande/)
[![ORCID](https://img.shields.io/badge/ORCID-iD-A6CE39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0004-1901-7109)
![Peer Reviewer](https://img.shields.io/badge/Peer_Reviewer-IEEE_Access_%7C_KBS-00629B?style=flat-square)

**Sr. Director of Data Science @ Socure.** I lead ML teams building real-time fraud and risk machine learning models operating at massive scale.

I work on fraud ML, agent identity and evaluation. My repos include a fault-injection test range, statistics for repeated benchmark runs, and signed credentials with delegation and revocation.

## Try something

- **Test an agent.** [Agent Retry Rodeo](https://github.com/RishabhPande/agent-retry-rodeo) runs your adapter against failed tools and ambiguous writes. Start with the offline replay; connecting a model is a separate step.
- **Compare repeated runs.** [agentstats](https://github.com/RishabhPande/agentstats) checks run-to-run variance and pairwise differences. Install from Git; the PyPI namesake is unrelated.
- **Verify delegation.** [Know Your Agent](https://github.com/RishabhPande/know-your-agent) checks signed credentials, delegation chains and revoked permissions. Demo only; no payments.
- **Read the research.** [AgentRisk](https://github.com/RishabhPande/agentrisk) measures fraud-policy behavior on a semi-synthetic benchmark. Its rates are benchmark results, not production estimates. Preprint, not peer-reviewed.

Everything here is synthetic data or public data. No Socure production data, no real transactions, no real PII, anywhere on this profile.

## See it run

<p align="center"><a href="https://github.com/RishabhPande/agentstats"><img src="https://raw.githubusercontent.com/RishabhPande/agentstats/main/docs/leaderboard_uncertainty.png" alt="Ten repeated runs of the same 12 agent configurations on SWE-bench Verified: the top spot changes between runs" width="100%"></a><br><sub><b><a href="https://github.com/RishabhPande/agentstats">agentstats</a></b>: Ten repeated runs of the same 12 agent configurations. Two statistically tied agents swap first place, so a single published run can crown either one. Real data from ASSERT-KTH (CC-BY-4.0).</sub></p>

<p align="center"><a href="https://github.com/RishabhPande/fraud-rings"><img src="https://raw.githubusercontent.com/RishabhPande/fraud-rings/main/docs/rings.png" alt="Fraud rings found by exact address match versus normalized address match" width="100%"></a><br><sub><b><a href="https://github.com/RishabhPande/fraud-rings">fraud-rings</a></b>: Address normalization recovers 2 of 3 planted rings that exact matching misses. The ring spread across several apartment units stays split on purpose. Synthetic data.</sub></p>

<p align="center"><a href="https://github.com/RishabhPande/stream-fraud"><img src="https://raw.githubusercontent.com/RishabhPande/stream-fraud/main/docs/drift_replay.png" alt="Drift replay: rolling score, PSI and KS statistics, and alarm delays over 20 seeds" width="100%"></a><br><sub><b><a href="https://github.com/RishabhPande/stream-fraud">stream-fraud</a></b>: Drift replay over 20 seeds. PSI alarmed earlier than a KS test here, and neither is false-alarm free. Synthetic data.</sub></p>

## This week in the lab: November 20, 2026

[fraud-eval](https://github.com/RishabhPande/fraud-eval/pull/3) now reports caught detector exceptions beside its metrics. A failed call can still count as a true negative under the existing fallback policy; the error count makes that visible. Exception text stays out of the results.

[Feature Contracts](https://github.com/RishabhPande/feature-contracts/pull/6) keeps positive-infinite evidence in its top-feature explanations instead of dropping the feature that broke the contract. Detection flags and calibration are unchanged.

[agentstats](https://github.com/RishabhPande/agentstats/pull/10) counts leaderboard pair flips one sampled leaderboard at a time, cutting temporary pair-array allocation. Same statistics and tie handling; pair comparisons still grow quadratically.

I also fixed [Tiny ML Lab](https://github.com/RishabhPande/tiny-ml-lab/pull/6)'s spectral-clustering failure demo. It now checks the erased graph, not an arbitrary bad accuracy from a degenerate eigenspace. The clustering algorithm and learner workbook are unchanged. All 116 tests pass.

## Fork this if

- **... you want to beat a seed sweep.** In [GNN-fraud-ring-detection](https://github.com/RishabhPande/GNN-fraud-ring-detection)'s synthetic demo setup, mean aggregation drops to AUC 0.728 / 0.539 on seeds 8-9 while max-pool, LSTM and GIN aggregators hold 1.000. Synthetic data, three seeds: a demo result, not a benchmark. Add your own aggregator and run the sweep. Pure Python, zero dependencies.
- **... you want a workbook, not a gallery.** [tiny-ml-lab](https://github.com/RishabhPande/tiny-ml-lab) is built to be forked: fill in each workbook.py, check days off in your own PROGRESS.md, add a row to the SHOWCASE.md hall of fame, and vote the next algorithm up the queue in REQUESTS.md.
- **... you want an unclaimed task.** [Time-series-anomaly-detection](https://github.com/RishabhPande/Time-series-anomaly-detection) has four on its roadmap: multivariate series with cross-channel attention, Informer-style sparse attention for long windows, streaming inference without re-encoding the window, and learned threshold calibration. Pick one and open a PR.

## Projects

**Evaluation, statistics and benchmarks**

| Repo | What it is |
|------|------------|
| [agentstats](https://github.com/RishabhPande/agentstats) | Run-to-run variance, significance tests and minimum-runs planning for AI agent benchmarks. Install from Git (the PyPI name belongs to another package). |
| [fraud-eval](https://github.com/RishabhPande/fraud-eval) | Open benchmark for LLM-based fraud and abuse detectors. v0.1.0 is a 20-case smoke test with a Hugging Face dataset and leaderboard. Listed in awesome-ai-security-tools (merged Nov 14, 2026). |
| [agentrisk](https://github.com/RishabhPande/agentrisk) | Benchmark and code for the preprint "Automation Is Not Intent": how fraud models treat legitimate AI shopping agents. |
| [feature-contracts](https://github.com/RishabhPande/feature-contracts) | Reproduction package for the feature-contracts manuscript, using public datasets. |

**Fraud and anomaly detection, from scratch in pure Python (synthetic data)**

| Repo | What it is |
|------|------------|
| [GNN-fraud-ring-detection](https://github.com/RishabhPande/GNN-fraud-ring-detection) | GraphSAGE, GAT and other graph networks with no dependencies, applied to fraud rings in transaction networks. |
| [fraud-rings](https://github.com/RishabhPande/fraud-rings) | Synthetic ring generator plus shared-attribute linking with union-find. |
| [stream-fraud](https://github.com/RishabhPande/stream-fraud) | Streaming scoring pipeline demo: velocity features, rule-based scorer, PSI and KS drift detection. |
| [Time-series-anomaly-detection](https://github.com/RishabhPande/Time-series-anomaly-detection) | Transformer autoencoder for collective and contextual anomalies. |
| [ID-document-forgery-detection-CV-](https://github.com/RishabhPande/ID-document-forgery-detection-CV-) | Classic image forensics on synthetic ID cards with planted forgeries. |
| [agentic-fraud-investigator](https://github.com/RishabhPande/agentic-fraud-investigator) | Multi-agent case investigation: triage, evidence, risk score, analyst-style report. Runs offline with a mock LLM by default. |

**Agents**

| Repo | What it is |
|------|------------|
| [know-your-agent](https://github.com/RishabhPande/know-your-agent) | Scoped, session-limited, revocable agent credentials signed with Ed25519, with delegation chains, a signed hash-chained audit trail, a benchmark hook, and a FastAPI demo. v0.2.0. |
| [agent-retry-rodeo](https://github.com/RishabhPande/agent-retry-rodeo) | Local test range for agent recovery: watch "done" fail against a fault, then replay a recovery-aware baseline. |

**Learning**

| Repo | What it is |
|------|------------|
| [tiny-ml-lab](https://github.com/RishabhPande/tiny-ml-lab) | One classic ML algorithm a day, numpy only, with a workbook to fill in. |

Presented as separate projects; no integrated pipeline is claimed here.

## Research and service

- **Peer review, 27 completed:** IEEE Access (2), Knowledge-Based Systems (4), Pattern Recognition (5), IEEE Transactions on Big Data (1), Expert Systems with Applications (2), Data Mining and Knowledge Discovery (1), Computers and Security (1), ACM Transactions on Knowledge Discovery from Data (1), FAccT 2027 (5), plus conference and workshop reviews for WWW 2027, SPF-LLM at AAAI 2027 and FinFM 2027. 22 posted on Web of Science as of Nov 25, 2026. Peer reviewer badge above names two venues only, the full list is here.
- **First acceptance:** "A Confidence Interval That Starts Above Its Own Estimate", Correspondence in JAMIA (Journal of the American Medical Informatics Association), accepted Nov 19, 2026, amiajnl-2026-021460. Accepted, not yet published.
- **Papers under peer review:** FATT, IEEE Access, Access-2026-52664; Feature Contracts, EAAI, EAAI-26-34856; Counterfactual Evaluation, SN Computer Science, SNCS-D-26-10446; Same Transactions, Different Frauds, ACM Transactions on Knowledge Discovery from Data, TKDD-2026-11-0976; Frozen-Detector Failure Under Controlled Attacker-Capability Shifts, Information Sciences, INS-D-26-15738; Selection-Aware Certification, IEEE Access, Access-2026-60783 (invited resubmission, in review from Nov 24, 2026). Goal: 2 peer-reviewed journals plus 2 peer-reviewed conferences.
- **Revising:** Testing published state-of-the-art claims, after an editorial decision at Science and AI (Nov 9, 2026), not currently under review.
- **Preprints, not peer-reviewed:** AgentRisk, Zenodo DOI 10.5281/zenodo.23477625; fraud-eval, Zenodo DOI 10.5281/zenodo.23695132.
- **Conferences:** ICMI2027 submitted, CMT Paper ID 157; SAI Computing Conference 2027 submitted, Paper ID COMPUTING-2027-105; CODASPY 2027 submitted, Paper ID 148; AgentRisk submitted to PoPETs 2027 Issue 3, Paper ID 42; Feature Contracts accepted at IEEE CCWC 2027, EDAS Paper ID 1571381470, accepted Nov 23, 2026.
- Program Committee: **IJCNN 2027**
- Co-inventor on U.S. Patent No. 12,810,299 (FATT: detecting and mitigating real-time fraud attacks using aggregated consortium data), granted November 24, 2026, plus further pending applications in AI-driven fraud detection (US + EP).

## Connect

- [LinkedIn](https://www.linkedin.com/in/rishabhpande/)
- [ORCID](https://orcid.org/0009-0004-1901-7109)
- [Hugging Face](https://huggingface.co/RishabhPande)
- [Google Scholar](https://scholar.google.com/citations?user=wt7gBXEAAAAJ)
- [Zenodo](https://zenodo.org/search?q=creator%3A%22Rishabh%20Pande%22)

Name on all of them: Rishabh Pande. ORCID iD wherever a field exists: 0009-0004-1901-7109. Paper bylines use Independent Researcher, employment is Socure, that difference is deliberate.

*Currently building in public. New commits land daily.*
