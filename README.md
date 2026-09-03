# Altair Li

**Reliable AI systems · Agent infrastructure · Financial ML research engineering**

I am a Data Science undergraduate at HKUST(GZ). On GitHub, I mainly work on systems where correctness depends on explicit state, provider semantics, reproducible evidence, and failure behavior—not just whether a happy-path demo runs.

For publications, research experience, education, and my academic CV, see **[altairpaca.github.io](https://altairpaca.github.io/)**.

## What I maintain

| Project | Role | What it demonstrates |
| --- | --- | --- |
| **[DSHelm](https://github.com/Altairpaca/dshelm)** | creator / maintainer | Explainable multi-model routing for DeepSeek Harness: policy resolution, compatibility boundaries, Resolution Trace, migration tooling, and evidence-gated community release work. |
| **[AlphaSeeker-TradeMaster](https://github.com/Altairpaca/AlphaSeeker-TradeMaster)** | research artifact maintainer | Financial time-series forecasting code with explicit chronological validation and documented information-set / leakage boundaries. |
| **[dsh-computer-use-windows](https://github.com/Altairpaca/dsh-computer-use-windows)** | creator / maintainer | Window-scoped Windows computer-use bridge with OCR-targeted actions, verification loops, failure evidence, and hosted CI separated from real-desktop validation. |

## Selected upstream work

| Area | Contribution | Upstream outcome |
| --- | --- | --- |
| **Session isolation** | [oh-my-openagent #6829](https://github.com/code-yeongyu/oh-my-openagent/pull/6829): diagnosed cross-session ULW continuation state leaking between independent sessions sharing one working directory; proposed explicit session scoping and fail-closed status reads. | Core diagnosis and module boundary were incorporated upstream; credited through co-authorship in the resulting implementation. |
| **SDK failure semantics** | [senpi #1223](https://github.com/code-yeongyu/senpi/pull/1223): centralized terminal-result failure classification across streaming, managed failover, resident settlement, and successful-turn bookkeeping. | Classification design was adopted and explicitly credited in the upstream implementation. |
| **Provider/cache semantics** | [senpi #1237](https://github.com/code-yeongyu/senpi/pull/1237): models prompt-cache lifetime as `fixed`, `automatic`, `disabled`, or `unknown`, avoiding fabricated TTL/savings claims for provider-managed DeepSeek caching. | Active upstream review. |
| **Release correctness** | [senpi #1224](https://github.com/code-yeongyu/senpi/pull/1224): preserves the Linux x64 PTY prebuild through build → artifact staging → npm packaging and makes required-target publication fail closed. | Active upstream review. |

The pattern I try to preserve in upstream work is:

`reproduce → identify the invariant → locate the ownership boundary → add regression evidence → implement the smallest durable fix → state residual limits`

## Research engineering

My research work is centered on **Financial ML / quantitative modeling** and **reliable AI**. The public repositories here are deliberately separated from proprietary market data and employer IP. For quantitative work, I care especially about chronological information boundaries, non-stationarity, walk-forward / out-of-time validation, and whether an apparent signal survives alternative baselines.

Research and publication details: **[Academic site](https://altairpaca.github.io/)** · **[Google Scholar](https://scholar.google.com/citations?user=md5Z-D8AAAAJ)**

## Current OSS priorities

- make DSHelm installable and independently verifiable from a clean environment;
- collect cross-platform installation evidence and a bounded planner → workers → reviewer first-run path;
- finish upstream review on Senpi provider/cache and PTY packaging work;
- keep public Financial ML artifacts explicit about leakage, causality, and evaluation contracts.

<sub>GitHub is my engineering / open-source surface. My academic site is the canonical source for CV-level biographical and research information.</sub>
