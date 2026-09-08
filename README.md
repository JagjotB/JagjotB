<h1 align="center">Jagjot Bisram</h1>

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

My core focus is **production AI/ML, reliable agent systems, model evaluation, backend architecture, MLOps, and cloud-native infrastructure**.

## Experience highlights

### [Numaflow](https://github.com/numaproj/numaflow) — Open Source Contributor

- Currently developing native **AWS SQS dead-letter queue support** in Numaflow's Rust data plane, including per-queue configuration, validation, failure-path testing, and API/schema updates
- Shipped **four merged upstream pull requests** across Kubernetes image transformations ([#3382](https://github.com/numaproj/numaflow/pull/3382), [#3389](https://github.com/numaproj/numaflow/pull/3389)), the React Errors interface ([#3392](https://github.com/numaproj/numaflow/pull/3392)), and HTTP-source documentation ([#3376](https://github.com/numaproj/numaflow/pull/3376))

### Riipen Level UP — Software & AI Engineering Internships

- Built Node.js and Python services for a real-time voice AI system, streaming live Twilio call audio over WebSockets for inference and response delivery
- Built a multi-tenant FastAPI backend for an LLM-powered voice agent, using Supabase/PostgreSQL row-level security to isolate client workspaces and support tool calling
- Built a deterministic scheduling engine with milestone dependencies, calendar intersections, capacity constraints, timezone-aware allocation, and idempotent regeneration

## Featured engineering

### [Sentinel](https://github.com/JagjotB/Sentinel) — evidence-backed Kubernetes incident investigation

<a href="https://sentinel-reliability.jagjot5.chatgpt.site/">
  <img src="https://raw.githubusercontent.com/JagjotB/Sentinel/build-sentinel/docs/assets/operator-console.png" alt="Sentinel operator console showing an evidence-backed Kubernetes incident investigation" width="100%" />
</a>

<table width="100%">
  <tr>
    <td width="25%" align="center"><strong>324</strong><br /><sub>isolated benchmark runs</sub></td>
    <td width="25%" align="center"><strong>90.3%</strong><br /><sub>selective root-cause accuracy</sub></td>
    <td width="25%" align="center"><strong>13.9%</strong><br /><sub>abstention rate</sub></td>
    <td width="25%" align="center"><strong>100%</strong><br /><sub>policy safety</sub></td>
  </tr>
</table>

Sentinel takes an alert from evidence collection to a cited diagnosis. Specialist agents correlate Kubernetes state, telemetry, logs, Git changes, and prior incidents; weak or contradictory evidence triggers abstention instead of a confident guess.

- Built a durable LangGraph runtime with concurrent specialists, checkpoints, budgets, retries, and traceable evidence
- Implemented typed providers for Kubernetes, Prometheus, Tempo, Git, and incident knowledge
- Combined hybrid BM25/vector retrieval, telemetry anomaly detection, and incident reranking
- Enforced policy validation and scoped human approval before any proposed change can become an artifact
- Shipped a FastAPI control plane, React operator console, PostgreSQL/Redis persistence, and OpenTelemetry instrumentation

The evaluation contains **324 isolated runs: nine systems across 36 seeded simulator incidents**. On the full system, Sentinel reached **77.8% overall accuracy (28/36)** and **90.3% selective accuracy (28/31 non-abstained)** at **13.9% abstention**, with **88.0% evidence recall**, **90.3% remediation accuracy**, and **100% policy safety**. Every run used a fresh repository and trace; the complete protocol, raw trials, ablations, and limitations are checked into the repository.

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

## Additional applied ML

### [NBA Finals Predictor 2026](https://github.com/JagjotB/nba-finals-predictor-2026) — probabilistic ML under changing evidence

An end-to-end prediction and decision-support system that models individual games before simulating possible paths through a best-of-seven series.

- Built a historical pregame dataset and chronological walk-forward validation across **915 playoff games**, comparing trained models with Elo and net-rating baselines
- Combined player projections, rotations, matchups, lineup strength, uncertainty, and game-level win probabilities in a Monte Carlo series simulator
- Shipped immutable pregame snapshots, post-game model updates, scenario analysis, calibration reports, and an interactive Streamlit dashboard

`Python` `scikit-learn` `XGBoost` `calibration` `Monte Carlo simulation` `Streamlit`

**[Explore the prediction engine →](https://github.com/JagjotB/nba-finals-predictor-2026)**

## Technical focus

**Languages**  
`Python` `TypeScript` `JavaScript` `SQL` `Rust` `Go` `C++`

**AI and agentic systems**  
`LLMs` `LangChain` `LangGraph` `RAG` `tool calling` `multi-agent systems` `LLM evaluation` `embeddings`

**Machine learning**  
`PyTorch` `scikit-learn` `XGBoost` `LightGBM` `Hugging Face Transformers` `NumPy` `Pandas` `learning-to-rank`

**Backend and distributed systems**  
`FastAPI` `Node.js` `React` `REST` `WebSockets` `PostgreSQL` `SQLAlchemy` `Redis` `distributed systems` `event-driven architecture`

**Infrastructure and observability**  
`Docker` `Kubernetes` `Airflow` `GitHub Actions` `CI/CD` `OpenTelemetry` `Prometheus` `Tempo` `Grafana` `Linux`

**Cloud and messaging**  
`AWS` `SQS` `EC2` `S3` `GCP` `Vertex AI` `BigQuery`

## Education

**Western University** — Bachelor of Science (BSc), Computer Science · 2025

## How I approach engineering

- **Measure before claiming.** Define the evaluation contract, preserve the artifacts, and make the result reproducible.
- **Design for failure.** Treat abstention, retries, rollback, observability, and human approval as product behavior.
- **Own the full path.** Connect the model to the service, the service to the operator, and the benchmark to the release decision.
- **Build for inspection.** Keep evidence, provenance, model versions, and operational decisions visible and auditable.

## Where I want to contribute

I am interested in **AI/ML Engineer**, **Machine Learning Engineer**, **Applied AI Engineer**, and **AI-focused Software Engineer** roles.

The through-line across my work is building production AI/ML systems end to end: models and evaluation, agent workflows, backend services, deployment, observability, reliability, and responsible automation. If your team is solving ambitious problems in those areas, I would be glad to connect.

<p align="center">
  <strong>Build it. Measure it. Make it trustworthy.</strong>
</p>
