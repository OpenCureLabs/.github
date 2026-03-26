<p align="center">
  <a href="https://github.com/OpenCureLabs/OpenCureLabs">
    <img src="https://raw.githubusercontent.com/OpenCureLabs/OpenCureLabs/main/logos/OpenCure%20Labs%20Inverted%20Color%20Transparent%20bg.svg" alt="OpenCure Labs" width="400">
  </a>
</p>

<p align="center"><strong>Autonomous AI agents for computational biology — open tools, public artifacts, and reproducible workflows.</strong></p>

---

## What We Do

OpenCure Labs is open infrastructure for computational biology, with a long-term goal of enabling more open and accessible personalized medicine workflows.

The platform runs neoantigen prediction, protein structure modeling, molecular docking, and QSAR pipelines against public datasets (TCGA, ClinVar, ChEMBL, GEO). All outputs — variant calls, docking scores, binding predictions — are published as structured artifacts with provenance metadata and integrity signatures.

The system supports both shared and private usage. In the default mode, a Cloudflare D1 task queue coordinates work across contributors, and results are signed by the contributing system and stored in R2. In solo mode, users run the same pipelines locally on their own data with no external calls.

---

## How It Works

1. **AI-driven workflows** — Specialist agents run genomics, structural biology, and pharmacology pipelines. A coordinator dispatches tasks; agents execute and return structured results.
2. **Public artifacts** — Every result is published to GitHub, PDF reports, and a downloadable dataset at **[opencurelabs.ai](https://opencurelabs.ai)**. Artifacts include Ed25519 signatures and review metadata.
3. **Independent AI critique** — Grok reviews every result through a two-tier critique process with literature cross-referencing. Results carry confidence-oriented review scores, not endorsements.
4. **Open contribution** — All code, configs, and pipeline definitions are open source. Run your own experiments, contribute compute to the shared task queue, or extend existing workflows.

---

## Built On

NVIDIA NeMo AgentIQ · MHCflurry · AlphaFold · AutoDock Vina · Vast.ai · PostgreSQL · Cloudflare R2/D1

---

> *Built in public. Run by agents. Reviewed with independent AI critique.*
