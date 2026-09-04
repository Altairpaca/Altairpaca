<p align="center">
  <img src="assets/hero.svg?v=20260904-dark2" alt="Zhenzhuo (Altair) Li — Financial ML, Quantitative Research, Reliable AI and Decision Systems" width="100%">
</p>

<p align="center">
  <a href="https://altairpaca.github.io/"><b>Academic Homepage</b></a> ·
  <a href="https://scholar.google.com/citations?user=md5Z-D8AAAAJ">Google Scholar</a> ·
  <a href="https://www.linkedin.com/in/zhenzhuo-li-2a2bb0307/">LinkedIn</a> ·
  <a href="https://altairpaca.github.io/assets/resume.pdf">CV</a>
</p>

I am a Data Science undergraduate at **HKUST(GZ)** and a quantitative research intern. My primary research and career axis is **Financial ML / AI-related Quant**, with a broader interest in reliable learning from non-stationary sequential data and in AI systems whose **state, evidence, time, and failure boundaries are explicit**.

This GitHub profile is my **engineering and public-research evidence surface**. For publications, research trajectory, education, PhD-facing research direction, and the canonical CV, use my [academic homepage](https://altairpaca.github.io/).

## Research & career direction

| Axis | Questions I care about | Current evidence |
| --- | --- | --- |
| **Financial ML / Quantitative Research** | How do models remain valid under non-stationarity, changing information sets, signal redundancy, and realistic temporal evaluation? | LENS (ACM ICAIF 2025), real-market Level-2 research, AlphaSeeker, quantitative internship |
| **Reliable AI & Decision Systems** | How should high-stakes systems expose temporal provenance, policy boundaries, uncertainty, and decision lineage instead of hiding them behind model output? | Clausula, Reliable Multi-Agent Financial Forecasting FYP |
| **Agent / Research Systems** | How can autonomous research and tool-using systems make state, provider semantics, evidence, and failure behavior auditable? | DSHelm, upstream Senpi / oh-my-openagent work, Windows computer-use bridge |

My 2027 PhD applications are centered on the methodological overlap between **Financial ML, non-stationary sequential learning, robust evaluation, reliable AI, and data/agent systems**. Long term, I expect to work close to quantitative research and Financial AI while keeping the underlying research questions transferable beyond a single market or model family.

## Flagship public work

| Project | Role | Why it matters to my profile |
| --- | --- | --- |
| **[Clausula](https://github.com/Altairpaca/clausula)** | creator / maintainer | Local-first deterministic investment decision system. Versioned ledgers, point-in-time provenance, policies, research evidence, capital/risk boundaries, and decision memory remain canonical outside the LLM. This is the clearest bridge between my Financial ML interests and reliable-system design. |
| **[DSHelm](https://github.com/Altairpaca/dshelm)** | creator / maintainer | Explainable multi-model routing for DeepSeek Harness with evidence-backed policy resolution, compatibility boundaries, Resolution Trace, and reproducible execution fixtures. |
| **[AlphaSeeker-TradeMaster](https://github.com/Altairpaca/AlphaSeeker-TradeMaster)** | research artifact maintainer | Financial time-series forecasting artifact from TradeMaster Cup 2026 with chronological validation and an explicit audit of offline-versus-causal information boundaries. |

<p align="center">
  <img src="assets/portfolio-map.svg?v=20260904-dark2" alt="Map from research questions to public artifacts and engineering evidence" width="100%">
</p>

## Applied systems

| Project | Surface | Engineering signal |
| --- | --- | --- |
| **[LedgerNest](https://github.com/Altairpaca/ledgernest)** · [EN overview](https://github.com/Altairpaca/ledgernest/blob/main/README.en.md) | self-hosted collaborative accounting | explicit accounting semantics, multi-user isolation, audit trails, import/export correctness, mobile-first product delivery |
| **[Keji](https://github.com/Altairpaca/keji)** · [EN overview](https://github.com/Altairpaca/keji/blob/main/README.en.md) | self-hosted client-work CRM | privacy-oriented vertical product engineering, document workflows, permissions, backup/restore, operational auditability |
| **[dsh-computer-use-windows](https://github.com/Altairpaca/dsh-computer-use-windows)** | Windows computer-use bridge | OCR-grounded actions, bounded verification, explicit failure evidence, hosted-CI versus real-desktop validation boundaries |

Small personal and experimental repositories remain public when they have a useful independent boundary, but they are intentionally not part of the main research / career narrative.

## Selected upstream impact

| Area | Contribution | Upstream outcome |
| --- | --- | --- |
| **Session isolation** | [oh-my-openagent #6829](https://github.com/code-yeongyu/oh-my-openagent/pull/6829): diagnosed cross-session ULW continuation state leaking between independent sessions sharing one working directory; proposed explicit session scoping and fail-closed status reads. | Maintainer called the diagnosis “correct and load-bearing”; the final upstream fix adopted the session-scope module boundary and credited me through co-authorship. |
| **SDK failure semantics** | [senpi #1223](https://github.com/code-yeongyu/senpi/pull/1223): centralized terminal-result failure classification across streaming, managed failover, resident settlement, and successful-turn bookkeeping. | The shared failure-classification design was adopted and explicitly credited in the merged upstream implementation. |
| **Provider/cache semantics** | [senpi #1237](https://github.com/code-yeongyu/senpi/pull/1237): models prompt-cache lifetime as `fixed`, `automatic`, `disabled`, or `unknown`, avoiding fabricated TTL/savings claims for provider-managed caching. | Active upstream review. |
| **Release correctness** | [senpi #1224](https://github.com/code-yeongyu/senpi/pull/1224): preserves the Linux x64 PTY prebuild through build → artifact staging → npm packaging and makes required-target publication fail closed. | Active upstream review. |

## How I build

`reproduce → identify the invariant → locate the ownership boundary → make time/state explicit → add regression evidence → implement the smallest durable fix → state residual limits`

Across Financial ML and systems work, I repeatedly care about the same failure mode: **a result can look correct while silently depending on information, state, credentials, execution conditions, or assumptions that will not hold later**. My research and engineering both try to surface those dependencies before they become hidden sources of error.

## Public surface map

| Surface | Canonical role |
| --- | --- |
| **[Academic homepage](https://altairpaca.github.io/)** | PhD / research-job visual CV: research focus, future direction, publications, experience, education, distinctions |
| **GitHub profile** | engineering depth, public research artifacts, project ownership, upstream review outcomes |
| **[Google Scholar](https://scholar.google.com/citations?user=md5Z-D8AAAAJ)** | publication record |
| **[LinkedIn](https://www.linkedin.com/in/zhenzhuo-li-2a2bb0307/)** | professional trajectory and external career identity |

<sub>Public repositories are intentionally separated from proprietary market data, employer IP, credentials, personal financial records, and private research assets.</sub>