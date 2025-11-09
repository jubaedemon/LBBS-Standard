# LLM Billing & Benchmarking Standard (LBBS) — v0.1 (Draft for Public Comment)

**Goal:** Establish a vendor‑neutral primary metric for LLM billing and benchmarking so buyers, researchers, vendors, and regulators can compare models fairly.

**Core metric:** **$·s/task** — the dollar cost multiplied by wall‑clock seconds to complete a defined task at an agreed quality threshold.

- **Secondary metrics:** $/task, s/task, success@Q
- **Compliance levels:** LBBS‑C1 (Baseline), LBBS‑C2 (Enhanced), LBBS‑C3 (Verified)
- **Governance (proposed):** Pilot under MLCommons/MLPerf → formalize via IEEE/ISO/NIST

---

## 📄 Standard Draft (PDF)

- **LBBS v0.1 — 2‑page standard draft (PDF):** [`docs/LBBS_v0_1_Standard_Draft.pdf`](docs/LBBS_v0_1_Standard_Draft.pdf)

## 🔎 What This Repo Is For

- Central hub for **public comments**, **issues**, **errata**, and **pilot submissions** around LBBS.
- Transparent discussion of definitions, measurement protocol, reporting, and compliance.

## 🧭 How to Participate

1. **Read the draft** (PDF linked above).  
2. **Open an issue** using the appropriate template:
   - “Proposal feedback” for comments on definitions or metrics.
   - “Data submission” for pilot results (include required metadata).
   - “Bug/errata” for problems in the spec or examples.
3. **(Optional) Submit a PR** to propose concrete text changes to the draft.

## 🧪 Running a Pilot (Quick Start)

- Select one public benchmark task (e.g., reasoning QA).  
- Run ≥30 trials per (model, task) over ≥24 h via **public API** and a declared plan tier.  
- Record **$/task**, **s/task**, **$·s/task**, **success@Q**, plus **metadata**: provider, model ID, tier, region, dates, any caching/preview toggles.  
- Publish median and [p10, p90] for the three metrics and success@Q CI.  
- Submit via the **Data submission** issue template with a small CSV (see the template in the issue).

## 🧩 Compliance Levels (Short)

- **LBBS‑C1:** Report $·s/task, $/task, s/task, success@Q, metadata.  
- **LBBS‑C2:** Add energy/task or GPU‑hour equivalents.  
- **LBBS‑C3:** Independent lab audit (e.g., MLCommons).

## 📬 Contact & Coordination

- We encourage coordination with **MLCommons/MLPerf** working groups for benchmarking alignment.  
- For standards track discussion: IEEE/ISO/NIST channels.

## 📣 License & Citation

- Text in this repo © authors, licensed **CC BY 4.0** (see `LICENSE`).  
- Please cite with the CFF metadata in `CITATION.cff`.

## ⚠️ Disclaimer

This is a community draft intended for discussion; it is not yet an adopted standard.
