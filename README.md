# Zhenzhuo (Altair) Li

**Financial ML · Quantitative Research · Reliable AI Systems**

I am a Data Science undergraduate at HKUST(GZ), working at the intersection of quantitative modeling, reliable AI, and agent infrastructure. GitHub is where I publish reproducible research artifacts, maintain systems projects, and contribute durable fixes upstream.

For publications, education, research experience, and my academic CV, see **[altairpaca.github.io](https://altairpaca.github.io/)**.

## Current focus

- **Financial ML / quantitative research** — chronological information boundaries, non-stationarity, walk-forward and out-of-time evaluation, signal robustness, and model behavior under changing market regimes.
- **Reliable AI systems** — session/state isolation, provider and cache semantics, failure classification, tool/runtime boundaries, and workflows whose behavior can be audited rather than inferred from a happy-path demo.
- **Open-source engineering** — evidence-first debugging, regression-oriented fixes, release correctness, cross-platform validation, and maintainable contributor surfaces.

## What I maintain

| Project | Role | What it demonstrates |
| --- | --- | --- |
| **[DSHelm](https://github.com/Altairpaca/dshelm)** | creator / maintainer | Explainable multi-model routing for DeepSeek Harness: policy resolution, compatibility boundaries, Resolution Trace, migration tooling, and evidence-gated community release work. |
| **[AlphaSeeker-TradeMaster](https://github.com/Altairpaca/AlphaSeeker-TradeMaster)** | research artifact maintainer | Financial time-series forecasting code with chronological validation and an explicit audit of offline-vs-causal information boundaries. |
| **[dsh-computer-use-windows](https://github.com/Altairpaca/dsh-computer-use-windows)** | creator / maintainer | Window-scoped Windows computer-use bridge with OCR-targeted actions, verification loops, explicit failure evidence, and hosted CI separated from real-desktop validation. |

## Selected upstream impact

| Area | Contribution | Upstream outcome |
| --- | --- | --- |
| **Session isolation** | [oh-my-openagent #6829](https://github.com/code-yeongyu/oh-my-openagent/pull/6829): diagnosed cross-session ULW continuation state leaking between independent sessions sharing one working directory; proposed explicit session scoping and fail-closed status reads. | Maintainer called the diagnosis "correct and load-bearing"; the final upstream fix adopted the session-scope module boundary and credited me through co-authorship. |
| **SDK failure semantics** | [senpi #1223](https://github.com/code-yeongyu/senpi/pull/1223): centralized terminal-result failure classification across streaming, managed failover, resident settlement, and successful-turn bookkeeping. | The shared failure-classification design was adopted and explicitly credited in the merged upstream implementation. |
| **Provider/cache semantics** | [senpi #1237](https://github.com/code-yeongyu/senpi/pull/1237): models prompt-cache lifetime as `fixed`, `automatic`, `disabled`, or `unknown`, avoiding fabricated TTL/savings claims for provider-managed DeepSeek caching. | Active upstream review. |
| **Release correctness** | [senpi #1224](https://github.com/code-yeongyu/senpi/pull/1224): preserves the Linux x64 PTY prebuild through build → artifact staging → npm packaging and makes required-target publication fail closed. | Active upstream review. |

My default contribution loop is:

`reproduce → identify the invariant → locate the ownership boundary → add regression evidence → implement the smallest durable fix → state residual limits`

## Research ↔ engineering bridge

My research work is centered on **Financial ML / quantitative modeling** and **reliable AI**. I have worked on large-scale financial time-series research infrastructure, real-market quantitative modeling, and reliable multi-agent financial forecasting. Public repositories are intentionally separated from proprietary market data, employer IP, credentials, and private research assets.

Research details: **[Academic site](https://altairpaca.github.io/)** · **[Google Scholar](https://scholar.google.com/citations?user=md5Z-D8AAAAJ)** · **[LinkedIn](https://www.linkedin.com/in/zhenzhuo-li-2a2bb0307/)**

## Current OSS priorities

- make DSHelm installable and independently verifiable from a clean environment;
- collect cross-platform installation evidence and a bounded planner → workers → reviewer first-run path;
- finish upstream review on Senpi provider/cache and PTY packaging work;
- keep public Financial ML artifacts explicit about leakage, causality, and evaluation contracts;
- publish new local projects only when they have a clear independent user, reproducibility, and maintenance boundary.

<sub>GitHub is my engineering / open-source surface. My academic site is the canonical source for CV-level biographical and research information.</sub>
