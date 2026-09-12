# Zhenzhuo (Altair) Li

### Financial ML · Quantitative Research · Performance & Reliable Systems

[Academic homepage](https://altairpaca.github.io/) · [Google Scholar](https://scholar.google.com/citations?user=md5Z-D8AAAAJ) · [LinkedIn](https://www.linkedin.com/in/zhenzhuo-li-2a2bb0307/) · [CV](https://altairpaca.github.io/assets/resume.pdf)

I am a Data Science undergraduate at **HKUST(GZ)** and a quantitative research intern. I want to connect **market understanding, useful models, and dependable implementation**: understand what a signal measures, establish when its inputs are available, and build systems whose correctness and performance can be independently checked.

This profile is my engineering evidence surface, not a list of every framework I have tried. My academic homepage remains the canonical source for publications, education, research trajectory, and my CV.

## Main direction

| Track | Questions and work | Evidence boundary |
| --- | --- | --- |
| **Quantitative research / Financial ML** | Market microstructure, financial time series, signal construction, and evaluation under the actual decision and execution constraints. | LENS (ACM ICAIF 2025), quantitative internship, and the public AlphaSeeker competition artifact. Employer research and proprietary data are not redistributed. |
| **Quantitative systems / performance engineering** | Market-data ingestion and replay, event ordering, bounded concurrency, C++ / Rust implementation, and HPC workload optimization. | An active development direction. Code, regression tests, workload definitions, and measured results must precede claims about speed, scale, or production readiness. |
| **Reliable research infrastructure** | Deterministic accounting, observable failures, session isolation, and tools that make research easier to verify. | Clausula, selected DSHelm work, and focused upstream contributions. Agent infrastructure supports the first two tracks rather than becoming an end in itself. |

I am interested in research and engineering roles close to quantitative decision-making. Methodological research remains important; the public engineering goal is to turn a concrete problem into a reproducible, useful artifact rather than to accumulate model wrappers or architectural diagrams.

## Selected projects

| Project | Role and useful boundary | Next evidence that matters |
| --- | --- | --- |
| **[Clausula](https://github.com/Altairpaca/clausula)** | Creator / maintainer. Local-first deterministic financial state, accounting, provenance, and explicit capability boundaries. | Real host/data acceptance, import and replay correctness, recovery evidence, and measured bottlenecks. It is not an HFT execution engine. |
| **[DSHelm](https://github.com/Altairpaca/dshelm)** | Creator / maintainer. Explainable routing and compatibility evidence for DeepSeek Harness. | A verified install/runtime journey and observable requested → resolved → effective routing. A source-compatible adapter alone is not runtime support. |
| **[AlphaSeeker-TradeMaster](https://github.com/Altairpaca/AlphaSeeker-TradeMaster)** | Maintainer of the TradeMaster Cup 2026 forecasting artifact, from the team that placed fifth. | Preserve the original competition path and its explicit offline-versus-causal information boundary. Competition results are not live trading results. |

**New systems work is a separate evidence line**, not a rewrite of a competition archive or an expansion of Clausula into market microstructure storage. The first useful deliverables should be narrowly scoped C++ / Rust components or upstream fixes with correctness oracles, reproducible workloads, and before/after measurements.

## Selected upstream work

| Area | Contribution | Attribution and status boundary |
| --- | --- | --- |
| **Session isolation** | [oh-my-openagent #6829](https://github.com/code-yeongyu/oh-my-openagent/pull/6829): diagnosed cross-session ULW continuation state sharing one working directory and proposed explicit session scoping. | The final upstream implementation adopted the session-scope boundary and credited the contribution through co-authorship. |
| **Failure semantics** | [senpi #1223](https://github.com/code-yeongyu/senpi/pull/1223): centralized terminal-result failure classification across streaming and settlement paths. | The shared classification design was adopted and credited upstream. |
| **Provider request boundaries** | [senpi #1558](https://github.com/code-yeongyu/senpi/pull/1558): preserve OpenCode session attribution in builtin compaction without changing provider authority order. | Proposed fix and focused regression coverage; the linked PR is authoritative for current review and CI status. |
| **Diagnostics and concurrency safety** | [oh-my-openagent #8098](https://github.com/code-yeongyu/oh-my-openagent/pull/8098) preserves bounded supervisor diagnostics; [#7880](https://github.com/code-yeongyu/oh-my-openagent/pull/7880) scopes parallel guidance to read-only work or isolated writers. | Proposed contributions, not claims that every branch is merged or every real-host gate has passed. |

Bug reports, diagnosis, implementation, independent verification, and maintainer integration are different contributions. I credit them separately; commenting on another author's merged PR is not authorship of that implementation.

## Supporting work, kept deliberately bounded

[SkillBench](https://github.com/Altairpaca/skillbench), [Agent Harness Index](https://github.com/Altairpaca/agent-harness-index), and [Local Agent Gateway](https://github.com/Altairpaca/local-agent-gateway) cover skill conformance, comparable experiment evidence, and bounded local delegation. They should earn further investment through actual consumers and end-to-end evidence, not additional layers of contracts alone.

[LedgerNest](https://github.com/Altairpaca/ledgernest) and [Keji](https://github.com/Altairpaca/keji) remain applied product work. Other experiments and course repositories are intentionally outside the main quant/systems narrative. A fork is not a maintenance commitment or an upstream contribution by itself.

## How I evaluate engineering work

**Reproduce → identify the invariant → build a reference test → measure the real bottleneck → implement the smallest durable change → compare on the same workload → state residual limits.**

Performance evidence should identify the source revision, compiler and flags, hardware, input distribution, warm-up and repetitions, and correctness checks. Throughput, service time, queueing latency, tail latency, memory, and allocation count are not interchangeable. Hosted CI is useful for correctness and benchmark smoke tests; hardware-specific performance claims require controlled measurements.

I do not equate a green synthetic test with production deployment, a model benchmark with trading returns, or a faster microbenchmark with an end-to-end improvement.

<sub>Public work is separated from proprietary market data, employer IP, credentials, personal financial records, and private research assets. No live brokerage execution is implied by these repositories.</sub>
