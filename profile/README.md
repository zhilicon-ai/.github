<p align="center">
  <br>
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-dark.png" width="480">
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-light.png" width="480">
    <img alt="Zhilicon" src="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-light.png" width="480">
  </picture>
  <br><br>
  <em>Purpose-built silicon for AI inference</em>
  <br><br>
</p>

<!-- Hero badges -->
<p align="center">
  <a href="https://developers.zhilicon.ai"><img src="https://img.shields.io/badge/ZHI--1_B0-Production_Silicon-0d1117?style=for-the-badge&labelColor=0d1117" alt="ZHI-1 B0"></a>&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk-examples/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-Apache_2.0-3da639?style=for-the-badge&labelColor=0d1117" alt="Apache 2.0"></a>&nbsp;
  <a href="https://discord.gg/zhilicon"><img src="https://img.shields.io/badge/Discord-Community-5865F2?style=for-the-badge&logo=discord&logoColor=white&labelColor=0d1117" alt="Discord"></a>
</p>

<!-- Tech stack badges -->
<p align="center">
  <img src="https://img.shields.io/badge/SystemVerilog-2017-4B0082?style=flat-square&labelColor=1a1a2e" alt="SystemVerilog 2017">&nbsp;
  <img src="https://img.shields.io/badge/C-11-00599C?style=flat-square&logo=c&logoColor=white&labelColor=1a1a2e" alt="C11">&nbsp;
  <img src="https://img.shields.io/badge/C++-17-00599C?style=flat-square&logo=cplusplus&logoColor=white&labelColor=1a1a2e" alt="C++17">&nbsp;
  <img src="https://img.shields.io/badge/Python-3.10_|_3.11_|_3.12-3776AB?style=flat-square&logo=python&logoColor=white&labelColor=1a1a2e" alt="Python">&nbsp;
  <img src="https://img.shields.io/badge/ONNX-Supported-005CED?style=flat-square&logo=onnx&logoColor=white&labelColor=1a1a2e" alt="ONNX">&nbsp;
  <img src="https://img.shields.io/badge/UVM-1.2-6E4C9E?style=flat-square&labelColor=1a1a2e" alt="UVM 1.2">
</p>

<!-- Performance highlight badges -->
<p align="center">
  <img src="https://img.shields.io/badge/ResNet--50_FP16-12,400_img%2Fs-00C853?style=flat-square&labelColor=1a1a2e" alt="ResNet-50 FP16">&nbsp;
  <img src="https://img.shields.io/badge/LLaMA--3--8B-3,200_tok%2Fs-00C853?style=flat-square&labelColor=1a1a2e" alt="LLaMA-3-8B">&nbsp;
  <img src="https://img.shields.io/badge/Speculative_Decode-7,400_tok%2Fs-00C853?style=flat-square&labelColor=1a1a2e" alt="Speculative Decode">&nbsp;
  <img src="https://img.shields.io/badge/BGE--large-28K_seq%2Fs-00C853?style=flat-square&labelColor=1a1a2e" alt="BGE-large">
</p>

<br>

<p align="center">
  <strong>We design AI inference chips from the transistor up.</strong><br>
  Architecture, RTL, verification, compiler, runtime, SDK — one team, one chip, one mission.
</p>

<p align="center">
  <a href="https://developers.zhilicon.ai">Developer Portal</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://developers.zhilicon.ai/docs">Documentation</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://discord.gg/zhilicon">Discord</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://developers.zhilicon.ai/access">Hardware Access</a>
</p>

---

## The Stack

Zhilicon owns every layer — from the silicon architecture to the Python SDK you pip-install. This is the full engineering surface, and every layer ships from this organization.

```
                        ┌─────────────────────────────────────────────────┐
                        │                                                 │
  Developer Surface     │   SDK Examples  ·  Benchmarks  ·  Developer Docs│
                        │   (public — start here)                         │
                        │                                                 │
  ══════════════════════╪═════════════════════════════════════════════════ │
                        │                                                 │
  Software Stack        │   Python SDK  ·  Compiler  ·  Runtime  ·  FW    │
                        │   ONNX → .zhimodel → execute → results          │
                        │                                                 │
  ══════════════════════╪═════════════════════════════════════════════════ │
                        │                                                 │
  Silicon               │   Architecture  ·  Microarchitecture  ·  RTL    │
                        │   Verification  ·  Implementation               │
                        │                                                 │
                        └─────────────────────────────────────────────────┘
                                            │
                                     ┌──────┴──────┐
                                     │   ZHI-1 B0  │
                                     │  AI Silicon  │
                                     └─────────────┘
```

---

## Start in 60 Seconds

No hardware needed. The full SDK runs on a free software simulator.

```bash
pip install zhilicon-sdk[simulator] --index-url https://pypi.zhilicon.ai/simple/
export ZHILICON_DEVICE=simulator
python -c "
import zhilicon as zhi
device = zhi.open_device()
model  = zhi.load_model('resnet50.zhimodel')
result = model.run(zhi.Tensor.random([1, 3, 224, 224]))
print(result.topk(1))
"
```

```
[zhilicon] Device: simulator  Backend: ZHI-1 functional model
[zhilicon] Top-1: tabby cat (confidence: 0.94)
```

When you're ready for real numbers, [apply for a ZHI-1 B0 evaluation board](https://developers.zhilicon.ai/access).

---

## Open Source

These repositories are public. Contributions welcome.

| Repository | Description | |
|:-----------|:------------|:--|
| **[zhilicon-sdk-examples](https://github.com/zhilicon-ai/zhilicon-sdk-examples)** | Production-ready examples: vision, NLP, recommendation, multi-device | [![CI](https://github.com/zhilicon-ai/zhilicon-sdk-examples/actions/workflows/ci.yml/badge.svg)](https://github.com/zhilicon-ai/zhilicon-sdk-examples/actions) [![License](https://img.shields.io/badge/Apache%202.0-blue.svg)](https://github.com/zhilicon-ai/zhilicon-sdk-examples/blob/main/LICENSE) |
| **[zhilicon-benchmarks](https://github.com/zhilicon-ai/zhilicon-benchmarks)** | Reproducible performance benchmarks with full methodology | [![CI](https://github.com/zhilicon-ai/zhilicon-benchmarks/actions/workflows/ci.yml/badge.svg)](https://github.com/zhilicon-ai/zhilicon-benchmarks/actions) [![License](https://img.shields.io/badge/Apache%202.0-blue.svg)](https://github.com/zhilicon-ai/zhilicon-benchmarks/blob/main/LICENSE) |
| **[zhilicon-developer-docs](https://github.com/zhilicon-ai/zhilicon-developer-docs)** | SDK reference, compiler guide, runtime guide, hardware overview | [![CI](https://github.com/zhilicon-ai/zhilicon-developer-docs/actions/workflows/ci.yml/badge.svg)](https://github.com/zhilicon-ai/zhilicon-developer-docs/actions) |

---

## ZHI-1 B0 Performance

Selected results from published benchmarks. Full methodology and reproduction steps in [zhilicon-benchmarks](https://github.com/zhilicon-ai/zhilicon-benchmarks).

| Workload | Model | Precision | Throughput | Metric |
|:---------|:------|:---------:|:----------:|:-------|
| Image Classification | ResNet-50 | FP16 | **12,400** | images/sec |
| Image Classification | ResNet-50 | INT8 | **18,900** | images/sec |
| Object Detection | YOLOv8-L | FP16 | **1,850** | images/sec |
| LLM Decode | LLaMA-3-8B | FP16 | **3,200** | tokens/sec |
| Speculative Decode | LLaMA-3-8B + draft | FP16 | **7,400** | tokens/sec |
| Sentence Embeddings | BGE-large | FP16 | **28,000** | sequences/sec |
| Retrieval | Two-tower | FP16 | **420K** | queries/sec |
| Pipeline Parallel | LLaMA-3-70B (4-chip) | FP16 | **890** | tokens/sec |

<sup>All numbers measured on ZHI-1 B0 silicon at production clock, batch-optimal settings, 5+ runs, median reported. Simulator results will differ. See <a href="https://github.com/zhilicon-ai/zhilicon-benchmarks/blob/main/docs/METHODOLOGY.md">methodology</a>.</sup>

---

## Repository Map

### Developer Surface (Public)

| Repository | Purpose |
|:-----------|:--------|
| [zhilicon-sdk-examples](https://github.com/zhilicon-ai/zhilicon-sdk-examples) | End-to-end examples: classification, detection, LLM decode, multi-device |
| [zhilicon-benchmarks](https://github.com/zhilicon-ai/zhilicon-benchmarks) | Performance benchmark suite with reproducible methodology |
| [zhilicon-developer-docs](https://github.com/zhilicon-ai/zhilicon-developer-docs) | Full SDK, compiler, runtime, and hardware documentation |

### Software Stack (Internal)

| Repository | Purpose |
|:-----------|:--------|
| zhilicon-sdk | Python SDK — device management, model loading, tensor operations, profiling |
| zhilicon-compiler | Graph compiler — ONNX ingestion, quantization, optimization passes |
| zhilicon-runtime | Execution engine — memory management, command scheduling, host-device protocol |
| zhilicon-boot-fw | Boot firmware — device init, power sequencing, diagnostics, secure boot |

### Silicon (Internal)

| Repository | Purpose |
|:-----------|:--------|
| zhilicon-architecture | Architecture specification, ISA definition, architecture decision records |
| zhilicon-microarchitecture | Microarchitecture design — pipeline, memory hierarchy, accelerator blocks |
| zhilicon-rtl-top | Top-level RTL integration — synthesis, lint, CDC, place-and-route handoff |
| zhilicon-uvm | UVM verification environment — agents, scoreboards, coverage, assertions |
| zhilicon-verification-plan | Verification strategy — test plans, coverage models, regression management |

### Governance (Internal)

| Repository | Purpose |
|:-----------|:--------|
| zhilicon-requirements | System and functional requirements with traceability |
| zhilicon-docs-internal | Internal engineering documentation — architecture specs, design reviews |
| zhilicon-release-management | Milestone governance — M0-M10 gates, release checklists, sign-off |

---

## Hardware Access

| Path | What You Get | How |
|:-----|:-------------|:----|
| **Simulator** | Full SDK, functional accuracy, all examples | `pip install zhilicon-sdk[simulator]` — free, immediate |
| **ZHI-1 B0 Board** | Production silicon, real throughput and power numbers | [Apply at developers.zhilicon.ai/access](https://developers.zhilicon.ai/access) |

---

## Get Involved

We build in the open where we can, and welcome contributions to our public repositories.

- **Contribute** — See [CONTRIBUTING.md](https://github.com/zhilicon-ai/zhilicon-sdk-examples/blob/main/CONTRIBUTING.md) for guidelines, DCO process, and review SLA
- **Report issues** — Use GitHub Issues on the relevant repository
- **Security** — Report vulnerabilities privately to **security@zhilicon.ai** ([policy](https://github.com/zhilicon-ai/zhilicon-sdk-examples/blob/main/SECURITY.md))
- **Discuss** — [Developer Forum](https://developers.zhilicon.ai/forum) · [Discord](https://discord.gg/zhilicon) · [Stack Overflow `zhilicon` tag](https://stackoverflow.com/questions/tagged/zhilicon)

---

<p align="center">
  <a href="https://zhilicon.ai">zhilicon.ai</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://developers.zhilicon.ai">Developers</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://developers.zhilicon.ai/docs">Docs</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://discord.gg/zhilicon">Discord</a>&nbsp;&nbsp;·&nbsp;&nbsp;
  <a href="https://zhilicon.ai/careers">Careers</a>
</p>
