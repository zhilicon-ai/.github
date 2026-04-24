<p align="center">
  <br>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-dark.png" width="480">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-light.png" width="480">
    <img alt="Zhilicon" src="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-light.png" width="480">
  </picture>
  <br><br>
  <em>Sovereign silicon for the AI era — five chips, one SDK, one engineering discipline.</em>
  <br><br>
</p>

<!-- Hero badges -->
<p align="center">
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk/releases/tag/v0.2.0"><img src="https://img.shields.io/badge/Portfolio-v0.2.0-0d1117?style=for-the-badge&labelColor=0d1117" alt="Portfolio v0.2.0"></a>&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk"><img src="https://img.shields.io/badge/SDK-Open_Source-3da639?style=for-the-badge&labelColor=0d1117" alt="Open Source SDK"></a>&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk/actions/workflows/ci.yml"><img src="https://img.shields.io/badge/Tests-428_passing-00C853?style=for-the-badge&labelColor=0d1117" alt="428 tests passing"></a>
</p>

<!-- Tech stack badges -->
<p align="center">
  <img src="https://img.shields.io/badge/SystemVerilog-2017-4B0082?style=flat-square&labelColor=1a1a2e" alt="SystemVerilog 2017">&nbsp;
  <img src="https://img.shields.io/badge/C-11-00599C?style=flat-square&logo=c&logoColor=white&labelColor=1a1a2e" alt="C11">&nbsp;
  <img src="https://img.shields.io/badge/C++-17-00599C?style=flat-square&logo=cplusplus&logoColor=white&labelColor=1a1a2e" alt="C++17">&nbsp;
  <img src="https://img.shields.io/badge/Python-3.10_|_3.11_|_3.12-3776AB?style=flat-square&logo=python&logoColor=white&labelColor=1a1a2e" alt="Python">&nbsp;
  <img src="https://img.shields.io/badge/MLIR-dialect-1a73e8?style=flat-square&labelColor=1a1a2e" alt="MLIR dialect">&nbsp;
  <img src="https://img.shields.io/badge/UVM-1.2-6E4C9E?style=flat-square&labelColor=1a1a2e" alt="UVM 1.2">
</p>

<br>

<p align="center">
  <strong>We design five category-defining silicon products from the transistor up.</strong><br>
  Datacenter AI · Rad-hard space · Sub-THz 6G · Crypto & ZKP · Healthcare-native.<br>
  Architecture, RTL, verification, compiler, runtime, SDK — one team, one portfolio, one mission.
</p>

<p align="center">
  <a href="https://zhilicon.ai">Website</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-developer-docs">Developer Docs</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk-examples">SDK Examples</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk/releases/tag/v0.2.0">v0.2.0 Release</a>
</p>

---

## The Portfolio — five chips

Zhilicon's five silicon products are purpose-built for verticals where incumbent AI silicon cannot credibly serve regulated buyers. Each has its own category; the SDK spans them all.

| Chip | Category | Target |
|:---|:---|:---|
| **Discovery-1** | Healthcare-native AI — DICOM ASIC, privacy enclave, FDA 510(k) pathway | Q3 2026 tape-out |
| **Horizon-1** | Rad-hard space AI — 300 krad TID, TMR-protected 16.4 TOPS, DO-254 DAL-B | Q1 2027 tape-out |
| **Nexus-1** | Sub-THz 6G — D-band hybrid-bond GaN/CMOS, on-die AI-learned beamforming | Q4 2026 Rev A |
| **Sentinel-1** | Crypto & ZKP — FIPS 140-3 L4 + silicon ZKP engines + silicon PQC | Q2 2026 tape-out |
| **Prometheus** | Datacenter AI — 8-chiplet X-Cube SoIC-X, dual-foundry (Intel 18A + Samsung SF2) | Q3 2026 tape-out |

Every chip is category-creating, not a spec-sheet comparator.

---

## The Stack

Zhilicon owns every layer — from silicon architecture to the Python SDK you `pip install`. Every layer ships from this organization.

```
                        ┌───────────────────────────────────────────────────┐
                        │                                                   │
  Developer Surface     │   SDK Examples  ·  Benchmarks  ·  Developer Docs  │
                        │   (public — start here)                           │
                        │                                                   │
  ══════════════════════╪═══════════════════════════════════════════════════
                        │                                                   │
  Software Stack        │   Python SDK  ·  Compiler  ·  Runtime  ·  Boot FW │
                        │   5 chip packages · ONNX · HuggingFace · Chat API │
                        │                                                   │
  ══════════════════════╪═══════════════════════════════════════════════════
                        │                                                   │
  Silicon               │   Architecture  ·  Microarchitecture  ·  RTL      │
                        │   UVM Verification  ·  Verification Plan          │
                        │                                                   │
                        └───────────────────────────────────────────────────┘
                                            │
                     ┌─────────┬─────────┬──┴───────┬──────────┬──────────┐
                     │Discovery│ Horizon │  Nexus   │ Sentinel │Prometheus│
                     │   -1    │   -1    │    -1    │    -1    │          │
                     └─────────┴─────────┴──────────┴──────────┴──────────┘
```

---

## Start in 60 seconds — cross-chip integration demo

No hardware needed. The full SDK runs on a pure-numpy emulation backend.

```bash
git clone https://github.com/zhilicon-ai/zhilicon-sdk-examples.git
cd zhilicon-sdk-examples
pip install git+https://github.com/zhilicon-ai/zhilicon-sdk.git
python demos/leo-satellite-inference/demo.py
```

Expected output in **under one second**:

```
========================================================================
ZHILICON LEO SATELLITE DEPLOYMENT EVALUATION
========================================================================

[1/5] ✓ SOVEREIGN ZONE        ae-defense-leo (classified)
[2/5] ✓ CHIPLET FABRIC        8 chiplets, max-abs-diff 0.00e+00 vs single-chip
[3/5] ✓ RAD-HARD SEU CAMPAIGN FIT/Mbit 560 (< 1000 unhardened reference)
[4/5] ✓ 6G DOWNLINK (140 GHz) +13.9 dB SNR, 9.32 Gbps @ 500 km
[5/5] ✓ CRYPTO ATTESTATION    HMAC-DRBG key + TVLA PASS + signed receipt

OVERALL: ALL FIVE CHECKS PASSED
```

One script, four chips composed, deterministic output, 428 passing tests back it. "One API, five capabilities" — runnable today, pre-silicon.

---

## What's in v0.2.0

Released **2026-04-18**. First production drop of the five-chip mitigation sweep. [Full release notes](https://github.com/zhilicon-ai/zhilicon-sdk/releases/tag/v0.2.0).

| Package | Chip | Closes audit gap |
|:---|:---|:---|
| `zhilicon.crypto` | Sentinel-1 | NIST SP 800-90A HMAC-DRBG + TVLA side-channel + CAVP generator |
| `zhilicon.medical` | Discovery-1 | HIPAA Safe Harbor 18-identifier scrubber + HMAC-chained audit log |
| `zhilicon.chiplet` | Prometheus | 8-chiplet fabric + tensor-parallel LLaMA (bit-identical to single-chip) |
| `zhilicon.rad_hard` | Horizon-1 | SEU injection (SBU/MCU/dist/BER) + TMR voter + robustness harness |
| `zhilicon.rf` | Nexus-1 | Friis link budget + MIMO channel + DFT/SVD/AI beamforming + OFDM |

**428 tests passing** across a Python 3.10 / 3.11 / 3.12 CI matrix. **29 ADRs** documenting every silicon and SDK decision from first principles.

---

## Repository map — 15 repositories

### Developer surface (public)

| Repository | Description |
|:---|:---|
| [`zhilicon-sdk`](https://github.com/zhilicon-ai/zhilicon-sdk) | Python SDK v0.2.0 — five chip packages + serving + sovereign attestation |
| [`zhilicon-sdk-examples`](https://github.com/zhilicon-ai/zhilicon-sdk-examples) | Runnable demos — LEO cross-chip, sovereign inference on K8s, chat UI, CUDA migration |
| [`zhilicon-developer-docs`](https://github.com/zhilicon-ai/zhilicon-developer-docs) | Public documentation site + 29 ADRs |
| [`zhilicon-benchmarks`](https://github.com/zhilicon-ai/zhilicon-benchmarks) | Performance benchmark evidence (activates at first silicon) |

### Software stack

| Repository | Description |
|:---|:---|
| [`zhilicon-compiler`](https://github.com/zhilicon-ai/zhilicon-compiler) | ZCC (Z Compute Compiler) — graph IR + MLIR dialect + codegen |
| [`zhilicon-runtime`](https://github.com/zhilicon-ai/zhilicon-runtime) | ZRT on-device runtime + ZCCL collectives + Kubernetes operator |
| [`zhilicon-boot-fw`](https://github.com/zhilicon-ai/zhilicon-boot-fw) | Boot firmware + secure-boot chain + SoC-level tools |

### Silicon

| Repository | Description |
|:---|:---|
| [`zhilicon-architecture`](https://github.com/zhilicon-ai/zhilicon-architecture) | Per-chip architecture deep-dives + system block diagrams |
| [`zhilicon-microarchitecture`](https://github.com/zhilicon-ai/zhilicon-microarchitecture) | Per-chip microarchitecture workbooks + remediation |
| [`zhilicon-rtl-top`](https://github.com/zhilicon-ai/zhilicon-rtl-top) | Top-level RTL sources for all five chips |
| [`zhilicon-uvm`](https://github.com/zhilicon-ai/zhilicon-uvm) | UVM testbenches + cocotb harnesses |
| [`zhilicon-verification-plan`](https://github.com/zhilicon-ai/zhilicon-verification-plan) | Verification closure + formal-proof tracking (5,442-property plan) |

### Governance

| Repository | Description |
|:---|:---|
| [`zhilicon-requirements`](https://github.com/zhilicon-ai/zhilicon-requirements) | Per-chip specifications + upgrade plans + ZPAS schemas |
| [`zhilicon-release-management`](https://github.com/zhilicon-ai/zhilicon-release-management) | KPI dashboards + deliverables + spec-tools CI |
| [`zhilicon-docs-internal`](https://github.com/zhilicon-ai/zhilicon-docs-internal) | Strategy, portfolio KPIs, board materials (Confidential — LP + Board only) |

---

## Engineering discipline

- **29 Architecture Decision Records** — every silicon and SDK decision documented with context, alternatives considered, and consequences.
- **428 SDK tests passing** on every push across Python 3.10 / 3.11 / 3.12 matrix.
- **Test-count regression guard** in CI — silent test deletion is caught before merge.
- **Dual-foundry production** — Intel 18A + Samsung SF2 for Prometheus with an 8-week switch playbook.
- **5,442-property formal verification plan** across the portfolio.
- **Sovereign attestation at silicon level** — per-zone data residency enforced in hardware (v2, post-silicon) and in software today (v1, ADR-0024).

---

## Get involved

- **Contribute** — See each public repo's `CONTRIBUTING.md`. DCO sign-off required.
- **Issues** — Use GitHub Issues on the relevant repository.
- **Security** — Report vulnerabilities privately per each repo's [`SECURITY.md`](https://github.com/zhilicon-ai/zhilicon-sdk/blob/main/SECURITY.md).
- **Community** — [Zhilicon on GitHub](https://github.com/zhilicon-ai) · [zhilicon.ai](https://zhilicon.ai).

---

<p align="center">
  <a href="https://zhilicon.ai">zhilicon.ai</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-developer-docs">Docs</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk/releases">Releases</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://zhilicon.ai/careers">Careers</a>
</p>
