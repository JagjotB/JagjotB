<p align="center">
  <img src="./assets/profile-banner.svg" alt="Jagjot Bisram — AI/ML Engineer building reliable intelligent systems" width="100%" />
</p>

<p align="center">
  <strong>I build AI systems that are evaluated like products, operated like infrastructure, and designed to fail safely.</strong>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/jagjotbisram"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&amp;logo=linkedin&amp;logoColor=white" alt="Connect on LinkedIn" /></a>
  <a href="mailto:bisramjagjot@gmail.com"><img src="https://img.shields.io/badge/Email-Say_Hello-111827?style=for-the-badge&amp;logo=gmail&amp;logoColor=white" alt="Send an email" /></a>
  <a href="https://sentinel-reliability.jagjot5.chatgpt.site/"><img src="https://img.shields.io/badge/Live_Project-Sentinel-0F766E?style=for-the-badge&amp;logo=kubernetes&amp;logoColor=white" alt="Open the Sentinel showcase" /></a>
</p>

## Engineering intelligent systems end to end

I am an **AI/ML Engineer** focused on the full path from an idea to a dependable system: data and model development, retrieval and ranking, agent orchestration, backend services, evaluation, deployment, observability, and operational safeguards.

My current work sits at the intersection of **production ML, AI reliability, search and ranking, backend architecture, and Kubernetes-native infrastructure**.

## Featured engineering

### [Sentinel](https://github.com/JagjotB/Sentinel) — evidence-backed Kubernetes incident investigation

<a href="https://sentinel-reliability.jagjot5.chatgpt.site/">
  <img src="https://raw.githubusercontent.com/JagjotB/Sentinel/build-sentinel/docs/assets/operator-console.png" alt="Sentinel operator console showing an evidence-backed Kubernetes incident investigation" width="100%" />
</a>

<table width="100%">
  <tr>
    <td width="25%" align="center"><strong>324</strong><br /><sub>isolated evaluation runs</sub></td>
    <td width="25%" align="center"><strong>77.8%</strong><br /><sub>root-cause accuracy</sub></td>
    <td width="25%" align="center"><strong>88.0%</strong><br /><sub>evidence recall</sub></td>
    <td width="25%" align="center"><strong>100%</strong><br /><sub>policy safety</sub></td>
  </tr>
</table>

Sentinel takes an alert from evidence collection to a cited diagnosis. Specialist agents correlate Kubernetes state, telemetry, logs, Git changes, and prior incidents; weak or contradictory evidence triggers abstention instead of a confident guess.

- Built a durable LangGraph runtime with concurrent specialists, checkpoints, budgets, retries, and traceable evidence
- Implemented typed providers for Kubernetes, Prometheus, Tempo, Git, and incident knowledge
- Combined hybrid BM25/vector retrieval, telemetry anomaly detection, and incident reranking
- Enforced policy validation and scoped human approval before any proposed change can become an artifact
- Shipped a FastAPI control plane, React operator console, PostgreSQL/Redis persistence, and OpenTelemetry instrumentation

The results above come from **nine systems evaluated across 36 seeded simulator incidents**, with a fresh repository and trace for every run. The complete protocol, raw trials, ablations, and limitations are checked into the repository.

**[Explore the architecture →](https://github.com/JagjotB/Sentinel#architecture)** &nbsp;·&nbsp; **[Inspect the evaluation →](https://github.com/JagjotB/Sentinel/blob/build-sentinel/docs/evaluation.md)** &nbsp;·&nbsp; **[Try the live showcase →](https://sentinel-reliability.jagjot5.chatgpt.site/)**

---

### [Retail Search & Ranking](https://github.com/JagjotB/retail-search) — learned ranking with a frozen benchmark

<a href="https://github.com/JagjotB/retail-search">
  <img src="https://raw.githubusercontent.com/JagjotB/retail-search/main/docs/demo/benchmark-comparison.png" alt="Retail Search and Ranking benchmark showing an 11.1832 percent relative NDCG at 10 improvement" width="100%" />
</a>

<table width="100%">
  <tr>
    <td width="33%" align="center"><strong>+11.18%</strong><br /><sub>relative NDCG@10</sub></td>
    <td width="33%" align="center"><strong>8,956</strong><br /><sub>frozen test queries</sub></td>
    <td width="34%" align="center"><strong>181,701</strong><br /><sub>test judgments</sub></td>
  </tr>
</table>

A production-oriented, two-stage search system that retrieves candidates with a dense index, reranks them with a LightGBM LambdaMART model, and serves the promoted model through FastAPI.

- Designed leakage-aware train, validation, and frozen-test boundaries around the Amazon ESCI dataset
- Versioned datasets, experiments, acceptance reports, and checksummed model artifacts for reproducibility
- Built a quality-gated Airflow retraining pipeline that promotes only candidates meeting the acceptance contract
- Packaged the serving path, browser demo, tests, and orchestration stack with Docker

**[Read the benchmark →](https://github.com/JagjotB/retail-search#retail-search--ranking-system)** &nbsp;·&nbsp; **[Review the reproduction steps →](https://github.com/JagjotB/retail-search#clean-setup-and-full-benchmark)**

## Additional work

| Project | What I built |
| --- | --- |
| **[FIFA World Cup 2026 Predictor](https://github.com/JagjotB/world-cup-2026)** | Historical match modeling, player and lineup features, and tournament-scale Monte Carlo simulation |
| **[NBA Finals Predictor 2026](https://github.com/JagjotB/nba-finals-predictor-2026)** | Game probabilities, player projections, matchup and lineup analysis, uncertainty modeling, and series simulation |
| **[Numaflow contributions](https://github.com/numaproj/numaflow/pulls?q=is%3Apr+author%3AJagjotB)** | **Four merged upstream pull requests** spanning Kubernetes image transformations, UI behavior, and product documentation |

## Technical focus

**AI, ML, and evaluation**  
`Python` `PyTorch` `scikit-learn` `LightGBM` `XGBoost` `LangGraph` `LangChain` `RAG` `embeddings` `ranking`

**Backend and product systems**  
`FastAPI` `Node.js` `TypeScript` `React` `REST` `WebSockets` `PostgreSQL` `Redis` `event-driven systems`

**Infrastructure and operations**  
`Docker` `Kubernetes` `Airflow` `OpenTelemetry` `Prometheus` `Tempo` `Grafana` `CI/CD` `AWS` `GCP` `Linux`

## How I approach engineering

- **Measure before claiming.** Define the evaluation contract, preserve the artifacts, and make the result reproducible.
- **Design for failure.** Treat abstention, retries, rollback, observability, and human approval as product behavior.
- **Own the full path.** Connect the model to the service, the service to the operator, and the benchmark to the release decision.
- **Build for inspection.** Keep evidence, provenance, model versions, and operational decisions visible and auditable.

I am especially interested in **AI infrastructure, agent reliability, production ML, search and ranking, and real-time systems**. If you are building ambitious systems in those areas, I would be glad to connect.

<p align="center">
  <strong>Build it. Measure it. Make it trustworthy.</strong>
</p>
