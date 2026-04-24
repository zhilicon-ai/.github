<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-dark.png" width="320">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-light.png" width="320">
  <img alt="Zhilicon" src="https://raw.githubusercontent.com/zhilicon-ai/.github/main/profile/assets/zhilicon-logo-light.png" width="320">
</picture>

# Zhilicon — Organization Profile & Community Health

### Org-level GitHub landing page, community-health files, and cross-repository policy for the Zhilicon five-chip silicon portfolio.

[![Org Profile](https://img.shields.io/badge/org_profile-live-00C853)](https://github.com/zhilicon-ai)
[![Portfolio](https://img.shields.io/badge/Zhilicon-v0.2.0-0d1117)](https://github.com/zhilicon-ai)
[![Repositories](https://img.shields.io/badge/repositories-15-0d1117)](https://github.com/orgs/zhilicon-ai/repositories)
[![License](https://img.shields.io/badge/License-Proprietary-red)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/zhilicon-ai/.github?color=0d1117&label=last%20commit)](https://github.com/zhilicon-ai/.github/commits/main)

</div>

---

<p align="center">
  <a href="https://github.com/zhilicon-ai"><strong>Organization Page</strong></a>&nbsp;·&nbsp;
  <a href="profile/README.md"><strong>Profile README</strong></a>&nbsp;·&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk"><strong>SDK</strong></a><sup>🔒</sup>&nbsp;·&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-developer-docs"><strong>Developer Docs</strong></a>&nbsp;·&nbsp;
  <a href="https://github.com/zhilicon-ai/zhilicon-sdk-examples/releases/tag/v0.2.0"><strong>v0.2.0 Release</strong></a>
</p>

---

## What this repository is

This is the **special `.github` repository** for the [`zhilicon-ai`](https://github.com/zhilicon-ai) GitHub organization. GitHub treats this repository as a source of defaults for every other repository in the org: if a community-health file (CODE_OF_CONDUCT, CONTRIBUTING, SECURITY, etc.) is missing in a given repository, GitHub falls back to the one in this repo. This is how Apple, NVIDIA, AMD, Samsung, Intel, Qualcomm and every tier-1 GitHub org maintains consistent governance across a multi-repo portfolio.

**Two roles in one repo:**

| File | Renders where | Audience |
|---|---|---|
| [`profile/README.md`](profile/README.md) | [`github.com/zhilicon-ai`](https://github.com/zhilicon-ai) (org landing page) | Public visitors — prospective customers, LPs, candidates |
| [`README.md`](README.md) *(this file)* | [`github.com/zhilicon-ai/.github`](https://github.com/zhilicon-ai/.github) (this repo) | Maintainers updating org governance |

---

## Org-level governance surface

The Zhilicon organization maintains a unified community-health baseline across all 15 repositories. The files in this repository are the defaults — individual repositories override only when they have a repo-specific policy.

```
.github/
├── profile/
│   ├── README.md              ← org-landing page (rendered at github.com/zhilicon-ai)
│   └── assets/
│       ├── zhilicon-logo-light.png
│       └── zhilicon-logo-dark.png
├── README.md                  ← this file (the repo landing page)
└── [roadmap]
    ├── CODE_OF_CONDUCT.md     ← org-wide default
    ├── CONTRIBUTING.md        ← org-wide default
    ├── SECURITY.md            ← org-wide default (reporting policy)
    ├── SUPPORT.md             ← org-wide default (getting help)
    ├── FUNDING.yml            ← org-wide (sponsor buttons)
    └── workflows/
        └── <reusable workflows>
```

> **Scope.** This repository holds **only org-level community-health defaults**. Repository-specific code, tests, CI workflows, and repo-specific governance live in the individual repositories. See [`profile/README.md`](profile/README.md) for the full 15-repository map.

---

## The Zhilicon portfolio — at a glance

Zhilicon ships **five category-defining silicon products** plus a unified cross-chip SDK. Every claim below links to a reproducible artefact.

| Chip | Category | Tape-out |
|:---|:---|:---|
| **Discovery-1** | Healthcare-native AI — DICOM ASIC, privacy enclave, FDA 510(k) pathway | Q3 2026 |
| **Horizon-1** | Rad-hard space AI — 300 krad TID, TMR-protected 16.4 TOPS, DO-254 DAL-B | Q1 2027 |
| **Nexus-1** | Sub-THz 6G — D-band hybrid-bond GaN/CMOS, on-die AI-learned beamforming | Q4 2026 Rev A |
| **Sentinel-1** | Crypto & ZKP — FIPS 140-3 L4 + silicon ZKP engines + silicon PQC | Q2 2026 |
| **Prometheus** | Datacenter AI — 8-chiplet X-Cube SoIC-X, dual-foundry (Intel 18A + Samsung SF2) | Q3 2026 |

**SDK v0.2.0** — 5 chip-specific Python packages, **428 tests passing**, **29 Architecture Decision Records**. See the full narrative on the [organization landing page](https://github.com/zhilicon-ai).

---

## Repository map — 15 repositories

### Developer surface (public)

| Repository | Description |
|:---|:---|
| [`zhilicon-sdk-examples`](https://github.com/zhilicon-ai/zhilicon-sdk-examples) | Runnable demos — LEO cross-chip, sovereign inference on K8s, chat UI, CUDA migration |
| [`zhilicon-developer-docs`](https://github.com/zhilicon-ai/zhilicon-developer-docs) | Public documentation site + 29 ADRs |
| [`zhilicon-benchmarks`](https://github.com/zhilicon-ai/zhilicon-benchmarks) | Performance benchmark suite (activates at first silicon) |

### Software stack (private)

| Repository | Description |
|:---|:---|
| [`zhilicon-sdk`](https://github.com/zhilicon-ai/zhilicon-sdk) 🔒 | Python SDK — five chip packages + serving + sovereign attestation |
| [`zhilicon-compiler`](https://github.com/zhilicon-ai/zhilicon-compiler) 🔒 | ZCC (Z Compute Compiler) — graph IR + MLIR dialect |
| [`zhilicon-runtime`](https://github.com/zhilicon-ai/zhilicon-runtime) 🔒 | ZRT runtime + ZCCL collectives + Kubernetes operator |
| [`zhilicon-boot-fw`](https://github.com/zhilicon-ai/zhilicon-boot-fw) 🔒 | Boot firmware + secure-boot chain + SoC tools |

### Silicon (private)

| Repository | Description |
|:---|:---|
| [`zhilicon-architecture`](https://github.com/zhilicon-ai/zhilicon-architecture) 🔒 | Per-chip architecture + system block diagrams |
| [`zhilicon-microarchitecture`](https://github.com/zhilicon-ai/zhilicon-microarchitecture) 🔒 | Per-chip microarchitecture workbooks + remediation |
| [`zhilicon-rtl-top`](https://github.com/zhilicon-ai/zhilicon-rtl-top) 🔒 | Top-level RTL sources for all five chips |
| [`zhilicon-uvm`](https://github.com/zhilicon-ai/zhilicon-uvm) 🔒 | UVM testbenches + cocotb harnesses |
| [`zhilicon-verification-plan`](https://github.com/zhilicon-ai/zhilicon-verification-plan) 🔒 | Verification closure + formal-proof tracking (5,442 properties) |

### Governance (private)

| Repository | Description |
|:---|:---|
| [`zhilicon-requirements`](https://github.com/zhilicon-ai/zhilicon-requirements) 🔒 | Per-chip specifications + upgrade plans + ZPAS schemas |
| [`zhilicon-release-management`](https://github.com/zhilicon-ai/zhilicon-release-management) 🔒 | KPI dashboards + deliverables + spec-tools CI |
| [`zhilicon-docs-internal`](https://github.com/zhilicon-ai/zhilicon-docs-internal) 🔒 | Strategy, portfolio KPIs, board materials (LP + Board only) |
| [`zhilicon-ai/.github`](https://github.com/zhilicon-ai/.github) | *(this repo)* Org-level profile + community-health defaults |

> 🔒 = private repository. External contributors should start with the public developer surface.

---

## Contributing to this repository

The community-health files in this repository govern the behaviour of **every repository in the Zhilicon organization**. Changes require review from the maintainers listed below and a reasoned justification in the PR description.

### Change-control policy

| Change type | Reviewers required |
|---|---|
| `profile/README.md` (org landing page) | `@zhilicon-ai/sdk` + `@zhilicon-ai/docs` |
| `profile/assets/*` (logo/brand assets) | `@zhilicon-ai/docs` + explicit brand sign-off |
| Org-level `CODE_OF_CONDUCT.md` / `CONTRIBUTING.md` / `SECURITY.md` | `@zhilicon-ai/sdk` + `@zhilicon-ai/docs` + `@zhilicon-ai/security` |
| `README.md` (this file) | `@zhilicon-ai/docs` |

### Development workflow

```bash
# Clone, branch, edit, push, PR
git clone https://github.com/zhilicon-ai/.github.git
cd .github
git checkout -b docs/improve-org-readme
# ... edit files ...
git add -A
git commit -s -m "docs(profile): <what changed>"   # DCO sign-off required
git push origin docs/improve-org-readme
gh pr create
```

All commits in this repository must be **DCO-signed** (`git commit -s`). GPG signing is recommended. The `main` branch is protected — all changes land via pull request.

---

## Org-wide badges — canonical list

These badges appear in every repo's README header. They are GitHub-API-driven and always reflect live state:

| Badge | URL template (replace `REPO` with the target repository name) |
|---|---|
| **CI** | `github.com/zhilicon-ai/REPO/actions/workflows/ci.yml/badge.svg` — latest main-branch CI run |
| **Release** | `img.shields.io/github/v/release/zhilicon-ai/REPO` — latest published release |
| **Last Commit** | `img.shields.io/github/last-commit/zhilicon-ai/REPO` — commit freshness indicator |
| **Portfolio** | `img.shields.io/badge/Zhilicon-vSEMVER-0d1117` — portfolio-wide version anchor |

Each repo supplements this core row with repo-specific badges (Python versions, linters, classification, export-control, chip coverage, etc.). See any repo's README for the concrete pattern.

---

## Security

Report security vulnerabilities privately by emailing **security@zhilicon.ai**. Do not open public issues for security-sensitive matters — the public issue tracker is not a triage surface for vulnerabilities.

Each Zhilicon repository carries its own `SECURITY.md` with repository-specific details. Start with the public [`zhilicon-sdk-examples/SECURITY.md`](https://github.com/zhilicon-ai/zhilicon-sdk-examples/blob/main/SECURITY.md) or [`zhilicon-developer-docs/SECURITY.md`](https://github.com/zhilicon-ai/zhilicon-developer-docs/blob/main/SECURITY.md) for the externally-visible policy.

For export-compliance questions on private silicon-design repositories (RTL, UVM, verification, architecture, microarchitecture, requirements), contact `export-compliance@zhilicon.ai`.

---

## License

Content in this repository is **Proprietary** — © Zhilicon. The organization landing page, logo assets, and community-health defaults are published on GitHub as part of the public-facing brand surface; they remain Zhilicon's property and are not licensed for reuse without written permission.

Individual Zhilicon repositories are licensed per their own `LICENSE` file.

---

<div align="center">

<a href="https://github.com/zhilicon-ai">github.com/zhilicon-ai</a>&nbsp;·&nbsp;
<a href="https://github.com/zhilicon-ai/zhilicon-sdk">SDK</a><sup>🔒</sup>&nbsp;·&nbsp;
<a href="https://github.com/zhilicon-ai/zhilicon-sdk-examples">Examples</a>&nbsp;·&nbsp;
<a href="https://github.com/zhilicon-ai/zhilicon-developer-docs">Developer Docs</a>&nbsp;·&nbsp;
<a href="https://github.com/zhilicon-ai/zhilicon-sdk-examples/releases">Releases</a>

</div>
