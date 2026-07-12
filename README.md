# Jonathan Beale

### Research systems for biology, markets, agent reliability, and quantum sensing

I build systems that make their own evidence inspectable. A result should lead to a dataset, configuration, benchmark, decision record, structure file, circuit, validation report, or preserved failure.

## Project index

| No. | System | Question | Repository |
| ---: | --- | --- | --- |
| 01 | Hybrid QML–KG | Can biomedical graph evidence rank plausible drug–disease links? | [open repository](https://github.com/iconbaypark2900/hybrid-qml-kg-poc) |
| 02 | SIGMA | Can a market signal survive baselines, costs, and promotion gates? | [open repository](https://github.com/Quantum-Global-Group/sigma) |
| 03 | Liaison | How should independent AI executors be governed and reviewed? | [open repository](https://github.com/iconbaypark2900/liaison-agentSystem) |
| 04 | Quantum Sensing Earth | Can gravity-derived water-mass data support a reproducible sensing workflow? | [open repository](https://github.com/iconbaypark2900/quantum-sensing-earth) |

---

## 01 / Hybrid QML–KG

**Biomedical link prediction on Hetionet**

```text
Hetionet
→ RotatE embeddings
→ compound–disease features
→ classical models + QSVC
→ stacking ensemble
→ PR-AUC evaluation
→ ranked candidates
```

| Inspect | Evidence |
| --- | --- |
| Problem | Predict missing Compound-treats-Disease links under severe class imbalance |
| Current reproducible best | Ensemble PR-AUC **0.7805** at seed 42 |
| Multi-seed result | **0.7398 ± 0.038** across five seeds |
| Classical baseline | HistGBDT **0.7393 ± 0.037** |
| Quantum result | Optimized QSVC remains near chance at approximately **0.50** |
| Structural artifact | CYP19A1 / aromatase PDB used for Anastrozole investigation |
| Verdict | The ensemble clears the project threshold; quantum advantage is **not** established |

[Repository](https://github.com/iconbaypark2900/hybrid-qml-kg-poc) · [Results table](https://github.com/iconbaypark2900/hybrid-qml-kg-poc/blob/main/results/multiseed/TABLE3.md) · [Architecture](https://github.com/iconbaypark2900/hybrid-qml-kg-poc/blob/main/docs/ARCHITECTURE.md)

---

## 02 / SIGMA

**Paper-first market research and execution governance**

```text
market window
→ features
→ model score
→ baseline comparison
→ cost-aware gate
→ BUY / HOLD / SELL record
→ paper execution
→ promotion or rejection
```

| Inspect | Evidence |
| --- | --- |
| Decision surface | Timestamped signal, confidence, expected return, and model version |
| Research controls | Purged cross-validation, triple-barrier labels, and cost-aware net-edge gates |
| Execution controls | Paper executor, audit records, retries, singleton worker lock, and risk limits |
| Promotion policy | Human-gated evaluation before champion or live promotion |
| Current phase | Internal-alpha infrastructure; paper validation remains the priority |
| Verdict | Trading infrastructure exists; persistent predictive alpha is **not yet proven** |

[Canonical SIGMA repository](https://github.com/Quantum-Global-Group/sigma)  
*The working repository is access-controlled; the link is retained as the canonical project location.*

---

## 03 / Liaison

**Local-first human-in-the-loop agent control plane**

Liaison does not wrap coding agents into one opaque assistant. Claude Code, Codex, OpenCode, Hermes, and research workers remain independent executors. Liaison passes durable context and governs what moves forward.

```bash
liaison init task-001 "One focused goal"
liaison snapshot --show
liaison attach hermes --text "Implementation report"
liaison approve-artifact <outbox-file>
liaison validate --profile python
liaison close-task --summary "Task complete"
```

| Durable artifact | Purpose |
| --- | --- |
| Task brief | Defines one bounded objective |
| Context snapshot | Preserves the state given to an executor |
| Outbox report | Records raw agent output |
| Approval / rejection | Keeps the human decision explicit |
| Validation summary | Connects checks to the produced artifact |
| Closeout record | Preserves result, limitation, and handoff |

[Repository](https://github.com/iconbaypark2900/liaison-agentSystem) · [Integrated operator model](https://github.com/iconbaypark2900/liaison-agentSystem/blob/main/docs/integrated-operator-model.md) · [Architecture](https://github.com/iconbaypark2900/liaison-agentSystem/blob/main/docs/architecture.md)

---

## 04 / Quantum Sensing Earth

**GRACE / GRACE-FO hydrology validation with sensing simulation**

```text
gravity-derived raster
→ provenance-preserving preprocessing
→ sensor simulation
→ detector comparison
→ spatial validation
→ basin and drought comparison
→ review artifacts
```

| Inspect | Evidence |
| --- | --- |
| Inputs | GRACE / GRACE-FO-style gravity grids, CRS, resolution, masks, and manifests |
| Validation | Detector comparison, calibration splits, spatial folds, confidence intervals |
| External context | USDM, GLDAS / TWS, basin summaries, and optional groundwater observations |
| Outputs | HTML report, JSON / CSV results, overlays, metrics, and artifact manifest |
| Scientific limit | Drought proxies are not direct groundwater truth |
| Verdict | Reproducible validation workflow; **not** a proven quantum groundwater detector |

[Repository](https://github.com/iconbaypark2900/quantum-sensing-earth) · [Scientific claims](https://github.com/iconbaypark2900/quantum-sensing-earth/blob/main/docs/SCIENTIFIC_CLAIMS.md) · [Data sources](https://github.com/iconbaypark2900/quantum-sensing-earth/blob/main/docs/DATA_SOURCES.md)

---

## Engineering principles

1. **Artifacts over claims** — expose files, metrics, commands, and outputs.
2. **Baselines before novelty** — classical methods remain visible beside quantum or agentic methods.
3. **Provenance at every boundary** — identify data, model, backend, fallback, and run.
4. **Promotion is a decision** — a successful execution is not automatically a successful experiment.
5. **Failures remain part of the record** — weak results and blocked gates are useful evidence.

## Operating environment

| Workstation | Role |
| --- | --- |
| NVIDIA DGX Spark | Embeddings, graph ML, quantum simulation, large backtests, and local model serving |
| GMKtec EVO-X2 | APIs, dashboards, orchestration, documentation, and lightweight experiments |
| Liaison | Shared task packets, evidence, validation, approval, and closeout across both systems |

## Core tools

**Languages:** Python, TypeScript, Java, SQL  
**ML / data:** PyTorch, scikit-learn, TensorFlow, NetworkX, PyKEEN  
**Quantum:** Qiskit, PennyLane, CUDA-Q  
**Systems:** FastAPI, Next.js, Docker, PostgreSQL, pgvector, Neo4j, Qdrant  
**Operations:** GitHub Actions, local model endpoints, DGX Spark, EVO-X2

---

I am interested in research engineering where reproducibility, honest evaluation, and system reliability matter as much as the model.
