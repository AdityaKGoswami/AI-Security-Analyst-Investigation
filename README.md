# AI Security Analyst — Investigating Simulated Cyber Attacks with AI

A defensive cybersecurity investigation platform that simulates multi-stage incidents, normalizes telemetry, detects suspicious behavior, correlates events, maps ATT&CK techniques, extracts IOCs, builds attack relationships, performs evidence-grounded AI analysis, validates AI claims, generates response playbooks and exports analyst-ready reports.

## Features

- Multiple synthetic attack scenarios
- Benign telemetry and noise
- Detection-as-code rules
- Sigma-like rule metadata
- Behavioral anomaly detection
- Event correlation and attack graph
- IOC extraction and optional enrichment hooks
- MITRE ATT&CK mapping and attack-path reconstruction
- Evidence provenance and SHA-256 integrity hash
- Deterministic local AI analyst
- Optional OpenAI / Ollama analysis
- AI claim validation and evidence coverage
- Competing hypothesis analysis
- Detection precision / recall / F1 evaluation
- AI investigation benchmark metrics
- Incident playbooks
- Markdown / JSON / CSV / STIX-style exports
- Streamlit SOC console
- Investigation replay view
- Analyst notes and evidence bookmarks
- GitHub Actions CI

## Run

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python run.py --scenario credential_compromise
streamlit run app.py
```

Linux/macOS activation:

```bash
source .venv/bin/activate
```

## Expanded investigation catalog

The build contains an expanded synthetic investigation and detection corpus across identity, endpoint, network, cloud, web, data, impact and defense-evasion categories. The datasets are synthetic and designed to exercise investigation, detection QA, ATT&CK mapping and evidence validation without executing real attack behavior.

## Product layer

The build includes a product-oriented architecture for SMB/MSSP evolution covering universal telemetry contracts, tenant-aware data handling, entity resolution, UEBA and ML anomaly scoring, dynamic risk, attack-surface and vulnerability intelligence contracts, identity/cloud/SaaS/email/data/supply-chain security contracts, threat-intelligence ingestion, knowledge-graph foundations, a safe security-hunt DSL, AI investigation planning and tool routing, RAG grounding, hypothesis testing, uncertainty and missing-telemetry reasoning, model routing/cost tracking, AI safety controls, human approval gates, SOAR action contracts, MDR/MSP primitives, RBAC, retention, posture scoring, usage metering, audit and privacy controls.

The product layer is provider-neutral. Local execution remains the default, with external infrastructure and model providers introduced behind adapters.

See `docs/product-architecture.md` and `docs/feature-matrix.md`.
