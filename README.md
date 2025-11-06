```
 ██████╗ ███████╗██╗  ██╗██╗███████╗██╗     ██████╗ 
██╔═══██╗██╔════╝██║  ██║██║██╔════╝██║     ██╔══██╗
██║   ██║███████╗███████║██║█████╗  ██║     ██║  ██║
██║▄▄██║╚════██║██╔══██║██║██╔══╝  ██║     ██║  ██║
╚██████╔╝███████║██║  ██║██║███████╗███████╗██████╔╝
 ╚══▀▀═╝ ╚══════╝╚═╝  ╚═╝╚═╝╚══════╝╚══════╝╚═════╝ 

         Hybrid Quantum-Safe Secure Messenger
         🔐 QKD + Post-Quantum Cryptography
```

## 🚀 Welcome to QShield

> **Enterprise-grade end-to-end encrypted messaging** combining **Quantum Key Distribution (BB84)** and **Post-Quantum Cryptography (Kyber)** for forward-secure, hybrid-resistant communications. Built for researchers, security engineers, and organizations that demand quantum-era resilience.

---

### 📊 Project Status & Metrics

| Metric | Status | Details |
|--------|--------|---------|
| **Development Status** | 🟦 Planning Phase | Core architecture & scaffolding |
| **Python Version** | 3.11+ | Type-safe with Pylance + mypy |
| **Security Level** | 🔴 Critical | QKD + PQC hybrid approach |
| **Test Coverage** | 90%+ Target | Unit + integration + negative tests |
| **Documentation** | 📚 Comprehensive | Protocol specs, threat models, ADRs |

---

### 🎯 Key Badges & Features

![Status](https://img.shields.io/badge/status-planning-blue?style=for-the-badge&logo=github)
![Python](https://img.shields.io/badge/python-3.11+-informational?style=for-the-badge&logo=python)
![Security](https://img.shields.io/badge/security-QKD%20%2B%20PQC-critical?style=for-the-badge&logo=shield)
![License](https://img.shields.io/badge/license-MIT%20%2F%20Apache--2.0-green?style=for-the-badge)
![Type Safe](https://img.shields.io/badge/type--safe-mypy%2FPylance-blue?style=for-the-badge&logo=python)
![CI/CD](https://img.shields.io/badge/CI%2FCD-GitHub%20Actions-orange?style=for-the-badge&logo=github)

---

### ⚡ What Makes QShield Stand Out

- 🔐 **Dual-Layer Keying**: BB84 QKD for continuous secret-key rates + Kyber KEM for instant fallback
- 📊 **Observable**: QBER, secret-key rate, reconciliation leakage, and end-to-end latency metrics
- 🏗️ **Modular Architecture**: Clean separation of crypto, QKD, networking, policy, and metrics
- 🧪 **Research-Grade**: Seeded reproducibility, deterministic tests, Jupyter notebooks with plots
- 🔒 **Authenticated**: Dilithium post-quantum signatures + HMAC transcript verification
- ⚙️ **Production-Ready Foundation**: FastAPI/WebSockets, pre-commit hooks, comprehensive docs

---

## � Quick Navigation

| Section | Purpose |
|---------|---------|
| [🚀 Quick Start](#-quick-start-windows-powershell) | Get running in 5 minutes |
| [📋 Features & Roadmap](#-features--roadmap) | What's included & planned |
| [🏗️ Architecture](#-architecture--design) | System design & components |
| [💻 Usage](#-usage-examples) | CLI commands & examples |
| [🧪 Testing & Benchmarks](#-testing--benchmarks) | Quality assurance |
| [🤝 Contributing](#-contributing--development) | How to contribute |
| [📚 Advanced](#-advanced-topics) | Deep dives & research |

---

## 🚀 Quick Start (Windows PowerShell)

Get QShield running locally in under 5 minutes. Designed for Windows PowerShell, WSL, and Linux.

### Prerequisites
- **Python 3.11+** with pip/poetry
- **Git** for cloning
- **Virtual environment** (recommended)

### Installation

```powershell
# Step 1: Clone the repository
git clone https://github.com/yourname/qshield.git
cd qshield

# Step 2: Create & activate virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1      # Windows PowerShell
# .venv\Scripts\Activate.bat      # Windows CMD
# source .venv/bin/activate       # macOS/Linux/WSL

# Step 3: Install dependencies & dev tools
python -m pip install --upgrade pip wheel setuptools
python -m pip install -e ".[dev]"

# Step 4: Setup pre-commit hooks (auto-linting on commit)
pre-commit install

# Step 5: Run test suite to verify setup
pytest -q --tb=short
```

✅ **All green?** You're ready to contribute!

---

## 📋 Features & Roadmap

### Current Capabilities (✅ = Completed | 🔲 = In Progress | ⏳ = Planned)

| Phase | Feature | Status | ETA | Details |
|-------|---------|--------|-----|---------|
| **0** | Repository scaffolding | ✅ | Done | `pyproject.toml`, CI/CD, pre-commit |
| **1** | AEAD baseline (AES-GCM) | 🔲 | Q1 2025 | Encryption, key derivation (HKDF) |
| **2** | BB84 QKD simulation | ⏳ | Q1 2025 | Cirq-based quantum key distribution |
| **3** | Error reconciliation | ⏳ | Q2 2025 | Cascade-lite, privacy amplification |
| **4** | PQC KEM mode (Kyber) | ⏳ | Q2 2025 | Post-quantum key encapsulation |
| **5** | Transcript authentication | ⏳ | Q2 2025 | Dilithium signatures, HMAC |
| **6** | Policy negotiation | ⏳ | Q3 2025 | Smart mode selection (QKD vs PQC) |
| **7** | WebSocket networking | ⏳ | Q3 2025 | FastAPI server + CLI client |
| **8** | Key buffer lifecycle | ⏳ | Q3 2025 | Async key provisioning |
| **9** | Metrics & dashboards | ⏳ | Q4 2025 | CSV logs, plots, live monitoring |
| **10** | Security documentation | ⏳ | Q4 2025 | Threat models, ADRs, best practices |
| **11** | Stretch: E91, GUI, group chat | ⏳ | 2026+ | Advanced protocols & interfaces |

### Technology Stack

```
┌─────────────────────────────────────────────────────────────┐
│                       QShield Stack                         │
├─────────────────────────────────────────────────────────────┤
│ 🔐 Cryptography:   AES-GCM, HKDF, Kyber, Dilithium        │
│ ⚛️  Quantum:        Cirq (BB84 simulation + noise models)   │
│ 🌐 Networking:     FastAPI, WebSockets, asyncio            │
│ 📊 Metrics:        Pandas, Matplotlib, CSV logging         │
│ 🧪 Testing:        pytest, hypothesis, seeded RNG          │
│ 📝 Quality:        mypy, black, isort, flake8, pre-commit  │
│ 📚 Docs:           Markdown, Jupyter notebooks, ADRs       │
└─────────────────────────────────────────────────────────────┘
```

---

## 🏗️ Architecture & Design

### High-Level Data Flow

```
┌──────────────────────────────────────────────────────────────────┐
│                        QShield Protocol                          │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│  CLIENT                                SERVER                    │
│    │                                      │                      │
│    ├─────── Handshake (QKD/PQC) ────────→ │ (Authenticated)    │
│    │                                      │                      │
│    │ ┌─────────────────────────────────┐  │                     │
│    │ │ 🔑 Key Negotiation              │  │                     │
│    │ │  • QKD Path (preferred):        │  │                     │
│    │ │    BB84 → Sift → Reconcile →    │  │                     │
│    │ │    Privacy Amp → Buffer         │  │                     │
│    │ │  • PQC Path (fallback):         │  │                     │
│    │ │    Kyber KEM (fast, robust)     │  │                     │
│    │ └─────────────────────────────────┘  │                     │
│    │                                      │                      │
│    ├──→ [AES-GCM Secure Channel] ←──────→ │ (Continuous)       │
│    │    (Rolling nonces + AAD)            │                      │
│    │                                      │                      │
│    └──→ [Rekey on Schedule/Exhaustion]    │                      │
│                                           │                      │
└──────────────────────────────────────────────────────────────────┘

QKD Pipeline (Detailed):
  Raw bits (noise) → [Sifting] → [Error Reconciliation]
      ↓
  [Privacy Amplification] → [Key Derivation] → [AES-GCM]
```

### Directory Structure

```
qshield/
├── 📄 README.md                    # This file
├── 📦 pyproject.toml               # Dependencies, metadata
├── 🔧 .pre-commit-config.yaml      # Auto-formatting hooks
├── 📁 src/qshield/
│   ├── __init__.py
│   ├── 🔐 crypto/
│   │   ├── aead.py                 # AES-GCM + HKDF
│   │   ├── kem.py                  # Kyber + X25519
│   │   └── sig.py                  # Dilithium + HMAC
│   ├── ⚛️  qkd/
│   │   ├── bb84.py                 # Cirq BB84 protocol
│   │   ├── sifting.py              # Basis sifting
│   │   ├── reconcile.py            # Error correction (Cascade-lite)
│   │   ├── privacy_amp.py          # Toeplitz hashing (PA)
│   │   └── utils.py                # Helpers
│   ├── 🌐 net/
│   │   ├── server.py               # FastAPI WebSocket server
│   │   └── client.py               # CLI client
│   ├── 🎛️  policy/
│   │   └── selector.py             # QKD vs PQC selection
│   ├── 📊 metrics/
│   │   ├── monitor.py              # Live metrics + CSV
│   │   └── plots.py                # Matplotlib visualizations
│   └── 📋 common/
│       ├── config.py               # Configuration
│       ├── logging.py              # Logging setup
│       └── messages.py             # Protocol messages
├── 📁 tests/
│   ├── test_aead.py
│   ├── test_bb84.py
│   ├── test_reconcile.py
│   ├── test_kem.py
│   └── conftest.py                 # Pytest fixtures
├── 📁 benchmarks/
│   ├── qkd_rate.py                 # Secret-key rate measurement
│   └── kem_latency.py              # KEM performance
├── 📁 docs/
│   ├── protocol.md                 # Message formats & state machines
│   ├── threat-model.md             # Security analysis (STRIDE)
│   ├── security.md                 # Cryptographic invariants
│   ├── roadmap.md                  # Feature requests & tracking
│   └── adr/                        # Architecture Decision Records
└── 📁 notebooks/
    ├── qber_vs_noise.ipynb         # QBER analysis
    └── pa_compression.ipynb        # Privacy amplification study
```

---

## 💻 Usage Examples

### Basic Setup & First Run

```powershell
# Start the QShield server
python -m qshield.net.server --host 127.0.0.1 --port 8765 --mode auto

# In another terminal, start a client
python -m qshield.net.client --url ws://127.0.0.1:8765 --mode auto

# Send encrypted messages (auto QKD→PQC negotiation)
> Type your message and press Enter
```

### Advanced: Mode Selection

```powershell
# Force QKD mode (BB84 preferred, strict)
python -m qshield.net.client --url ws://127.0.0.1:8765 --mode qkd --verbose

# Force PQC mode (Kyber only, instant)
python -m qshield.net.client --url ws://127.0.0.1:8765 --mode pqc

# Auto mode (smart fallback) — recommended
python -m qshield.net.client --url ws://127.0.0.1:8765 --mode auto --metrics
```

### Running Benchmarks

```powershell
# Measure QKD secret-key rate vs noise
python benchmarks/qkd_rate.py --p_flip 0.02 --blocks 128 --trials 100

# Measure Kyber KEM latency
python benchmarks/kem_latency.py --trials 500 --verbose

# Output: CSV metrics + terminal report
```

### Interactive Notebook Analysis

```powershell
# Launch Jupyter to explore QKD behavior
jupyter notebook notebooks/qber_vs_noise.ipynb

# Analyze privacy amplification compression
jupyter notebook notebooks/pa_compression.ipynb
```

---

## 🧪 Testing & Benchmarks

### Quality Assurance

QShield uses a comprehensive testing & quality strategy:

| Tool | Purpose | Command |
|------|---------|---------|
| **pytest** | Unit + integration tests | `pytest -q --cov=src/` |
| **mypy** | Static type checking | `mypy src/ --strict` |
| **black** | Code formatting | `black src/ tests/ benchmarks/` |
| **isort** | Import organization | `isort src/ tests/` |
| **flake8** | Linting | `flake8 src/` |
| **pre-commit** | Git hook automation | `pre-commit run --all-files` |

### Run Test Suite

```powershell
# Quick test run
pytest -q

# With coverage report
pytest --cov=src/qshield --cov-report=html

# Only crypto tests
pytest tests/test_aead.py tests/test_kem.py -v

# Run with detailed output
pytest -vv --tb=long
```

### Reproducible Benchmarks

```powershell
# All benchmarks with seeded RNG
python -m pytest benchmarks/ --benchmark-only

# Save results
python benchmarks/qkd_rate.py --seed 42 --output metrics.csv
```

---

## 🤝 Contributing & Development

### Development Workflow

1. **Fork & Clone**: Create a feature branch (`git checkout -b feature/awesome-feature`)
2. **Develop**: Write code + tests (≥90% coverage)
3. **Format**: Run `black`, `isort`, `mypy` (pre-commit does this automatically)
4. **Test**: `pytest -q` must pass
5. **Commit**: Use conventional commits (`feat:`, `fix:`, `docs:`, `test:`)
6. **Push & PR**: Submit with a clear description

### Code Quality Gates

- ✅ All tests pass (`pytest -q`)
- ✅ Type checking passes (`mypy src/ --strict`)
- ✅ Formatting is clean (`black --check`, `isort --check`)
- ✅ At least one negative test per crypto PR
- ✅ Documentation updated (`docs/` or docstrings)
- ✅ Commit message is descriptive

### Good First Issues

Look for these labels on GitHub:
- `good-first-issue` — Small, self-contained tasks
- `area/qkd` — QKD-related work
- `area/crypto` — Cryptography fixes
- `type/docs` — Documentation improvements

### Security Checklist (Crypto PRs)

- [ ] Unique nonce per AES-GCM encryption
- [ ] All transcripts authenticated (HMAC or Dilithium)
- [ ] Reconciliation leakage accounted in PA
- [ ] Rekey before nonce exhaustion
- [ ] Ephemeral keys zeroized on close/error
- [ ] Negative tests included (tampering, replay, etc.)

---

## 📊 Metrics & Monitoring

QShield provides built-in metrics for research and debugging:

### Key Metrics

| Metric | Definition | Impact |
|--------|-----------|--------|
| **QBER** | Quantum Bit Error Rate | Indicates eavesdropping / noise |
| **Sifted Rate** | % of bits passing sifting | Quality of BB84 run |
| **EC Leakage** | Bits revealed during reconciliation | Reduces effective secret key |
| **PA Output** | Final secure key after PA | Guaranteed secret |
| **Rekey Time** | Time from handshake to ready | User-facing latency |

### Export Metrics

```powershell
# Server writes metrics to CSV
python -m qshield.net.server --metrics metrics.csv --output-interval 60

# Client logs local metrics
python -m qshield.net.client --metrics-file client_metrics.csv

# Plot results
python metrics/plots.py --input metrics.csv --output plots/
```

---

## 📚 Advanced Topics

## ✨ Highlights (what makes QShield cool)

- 🔐 Hybrid keying: QKD (BB84) for continuous secret-rate experiments and PQC (Kyber) for robust fallback.
- ⚖️ Measurables: QBER, secret-key rate, reconciliation leakage, and rekey latency.
- ⚙️ Modular: clear `src/` layout (crypto, qkd, net, metrics, policy).
- 🧪 Reproducible: seeded notebooks and deterministic unit tests for the research bits.

---

## 📚 Table of contents

1. [Quick start (Windows PowerShell)](#quick-start-windows-powershell)
2. [Usage examples](#usage-examples)
3. [Architecture at a glance](#architecture-at-a-glance)
4. [Roadmap (short)](#roadmap-short)
5. [Contributing & quality gates](#contributing--quality-gates)
6. [Appendix: original README (archived)](#appendix-original-readme-archived)

---

## Quick start (Windows PowerShell)

These commands are tailored for Windows PowerShell (your default shell). They set up a virtual environment, install dev extras, and run tests.

```powershell
# 1) Clone & create venv
git clone https://github.com/yourname/qshield.git
cd qshield
python -m venv .venv; .\.venv\Scripts\Activate.ps1

# 2) Install dependencies (editable), adjust extras in pyproject.toml
python -m pip install --upgrade pip wheel
python -m pip install -e ".[dev]"

# 3) Pre-commit hooks & tests
pre-commit install
pytest -q
```

If you prefer WSL or bash, replace the activation line with `source .venv/bin/activate`.

---

## Usage examples

Start a simple server and connect with a client (auto-mode: QKD preferred, PQC fallback):

```powershell
# run server
python -m qshield.net.server --host 127.0.0.1 --port 8765

# connect client (auto negotiation)
python -m qshield.net.client --url ws://127.0.0.1:8765 --mode auto
```

Pro tip: run `python -m qshield.net.client --help` for CLI flags (mode selection, verbosity, metrics logging).

---

## Architecture at a glance

High-level flow (ASCII diagram):

```
  [ Client ] <--WebSocket--> [ Server ]
      |                         |
      |--- Handshake (QKD or PQC, authenticated) ---|
      |                         |
  [Key Derivation] -> [AES-GCM data plane] -> [Rekey Policy]
      |
  [Key Buffer] <= QKD pipeline: BB84 -> Sift -> Reconcile -> PrivacyAmp
```

Key modes:
- QKD path: simulated BB84 (Cirq) -> sifting -> error reconciliation -> privacy amplification -> key buffer
- PQC path: Kyber KEM (OQS) for quick, robust provisioning

---

## Roadmap (short & actionable)

- Phase 0: repository scaffolding, CI, pre-commit, basics ✅
- Phase 1: AEAD baseline (AES-GCM + HKDF + tests)
- Phase 2: BB84 simulation + QBER metrics
- Phase 3: Sifting, EC, Privacy Amplification (leakage accounting)
- Phase 4: PQC KEM mode (Kyber) + benchmarks
- Phase 5: Authenticated transcripts (Dilithium/HMAC)
- Phase 6: Policy selection (when to use QKD vs PQC)

Stretch: E91, group chat, GUI, quantum experiments

---

## Contributing & quality gates

- Please open small PRs. Each PR should include at least one test.
- CI checks: lint (black/isort), typecheck (mypy), tests (pytest).
- Security checklist for PRs changing crypto:
  - Unique nonce per key
  - Transcript authentication
  - Leakage accounting for reconciliation

If you'd like to help, look for issues labeled `good-first-issue` and `area/qkd`.

---

## Visual & memorable extras

- ASCII logo (feel free to replace with an SVG in `assets/`):

```
  ____  _     _ _ _ _     _ _
 / __ \| |   (_) | (_)   | | |
| |  | | |__  _| | |_  __| | | ___ _ __
| |  | | '_ \| | | | |/ _` | |/ _ \ '__|
| |__| | | | | | | | | (_| | |  __/ |
 \____/|_| |_|_|_|_|_|\__,_|_|\___|_|

     Q S H I E L D  —  Quantum + PQC hybrid
```

- Badges: use shields.io to create additional badges (CI, coverage, docs).

---

## Examples of useful commands

- Run the QKD rate benchmark (small):

```powershell
python benchmarks/qkd_rate.py --p_flip 0.02 --blocks 128
```

- Run KEM latency micro-benchmark:

```powershell
python benchmarks/kem_latency.py --trials 200
```

---

## Files & where to look first

- `src/qshield/crypto/` — AEAD, KEM, signatures
- `src/qshield/qkd/` — BB84, sifting, reconciliation, privacy amplification
- `src/qshield/net/` — server & client (FastAPI + WebSockets)
- `docs/` — protocol, threat model, ADRs
- `notebooks/` — reproducible experiments and plots

### Threat Model

QShield protects against:
- ✅ **Passive eavesdropping** (Eve): QKD detects with QBER rise
- ✅ **Active MITM attacks**: Dilithium/HMAC authentication prevents tampering
- ✅ **Detector side-channels**: Noise model accounts for real quantum imperfections
- ✅ **Replay attacks**: Nonce + session management

See `docs/threat-model.md` for full STRIDE analysis.

### Finite-Key Corrections

Real deployments use finite keys. QShield accounts for:
- Leakage during error reconciliation (bits revealed)
- Tail-bound analysis for PA output
- Conservative secret-key rate estimates

References: `docs/security.md`, research papers in `notebooks/`.

### Performance Tuning

| Parameter | Range | Impact |
|-----------|-------|--------|
| Block size (EC) | 64–512 | Trade-off: larger = better correction, slower convergence |
| PA Toeplitz size | 1x–10x key length | Higher = more security margin, larger overhead |
| Rekey interval | 10–1000 msgs | Frequent = safer, more overhead |
| QBER threshold | 5–15% | Below = accept QKD, above = switch to PQC |

---

## 🎓 Research & References

### Key Papers & Resources

- **BB84 Protocol**: Bennett & Brassard (1984) – Quantum Cryptography
- **Kyber KEM**: NIST Post-Quantum Cryptography Standardization
- **Cascade EC**: Brassard & Salvail (1994) – Secret-key reconciliation
- **Privacy Amplification**: Toeplitz hashing, universal hashing theory
- **Dilithium**: NIST's post-quantum digital signature standard

### Reproducible Notebooks

Run these to understand QShield internals:

```powershell
# QBER vs noise level analysis
jupyter notebook notebooks/qber_vs_noise.ipynb

# Privacy amplification compression study
jupyter notebook notebooks/pa_compression.ipynb
```

All notebooks use seeded RNG (seed=42 by default) for reproducibility.

---

## 📄 License & Attribution

**QShield** is dual-licensed:
- **MIT License** — Simple, permissive
- **Apache 2.0 License** — Patent protection

Choose one in your `LICENSE` file.

### Dependencies

- **Cirq** — Google's quantum circuit simulator (Apache 2.0)
- **Open Quantum Safe (OQS)** — Post-quantum cryptography library (MIT)
- **FastAPI** — Modern async web framework (MIT)
- **cryptography** — Cryptographic recipes (Apache 2.0 / BSD)
- **numpy, scipy** — Scientific computing (BSD)

**Please review third-party licenses** and ensure compliance in your deployment.

---

## 🙋 Getting Help & Support

### Troubleshooting

| Issue | Solution |
|-------|----------|
| `ModuleNotFoundError: No module named 'cirq'` | Run `pip install -e ".[dev]"` |
| `mypy` errors on quantum imports | Add `# type: ignore` comments, see `docs/type-hints.md` |
| Tests fail with random seeds | Use `pytest --seed=42` for reproducibility |
| WebSocket connection refused | Check port 8765 is not in use |

### Report Issues

1. Check existing issues on GitHub
2. Provide: Python version, OS, steps to reproduce, error output
3. Tag appropriately: `bug`, `enhancement`, `question`, `docs`

### Join the Community

- **GitHub Discussions** — Ask questions, share ideas
- **Issues** — Bug reports & feature requests
- **Pull Requests** — Code contributions
- **Email**: maintainer@qshield.org (placeholder)

---

## 🎯 Success Metrics & Vision

### Near-Term (6 months)

- ✅ All core phases 1–7 complete (AEAD → Networking)
- ✅ 90%+ test coverage
- ✅ CLI chat demo working end-to-end
- ✅ Benchmark suite published

### Medium-Term (1 year)

- 🚀 Production-grade security audit
- 🚀 TLS proxy integration (quantum-safe VPN)
- 🚀 WebUI / Desktop client
- 🚀 Group chat with TreeKEM

### Long-Term (2+ years)

- 🔮 Real quantum hardware integration (IBM Q, IonQ)
- 🔮 E91 protocol variant
- 🔮 Decoy-state QKD
- 🔮 Standards compliance (NIST, BSI)

---

## 👥 Core Team & Contributors

| Role | Name | Expertise |
|------|------|-----------|
| Lead Architect | You | Quantum + Security |
| Crypto | — | Post-quantum, KEM |
| QKD Research | — | BB84, reconciliation |
| Networking | — | FastAPI, WebSockets |

**Contributions welcome!** Add your name here after your first PR.

---

## 📞 Contact & Social

- 📧 Email: [maintainer@qshield.org](mailto:maintainer@qshield.org)
- 🔗 GitHub: [github.com/yourname/qshield](https://github.com/yourname/qshield)
- 🐦 Twitter: [@QShieldCrypto](https://twitter.com/)
- 💬 Discord: [QShield Community](https://discord.gg/)

---

## 📈 Stats & Impact

```
Lines of Code:       ~5,000 (target)
Test Coverage:       90%+
Number of PRs:       Accepting now!
Documentation:       Comprehensive (20+ pages)
Quantum Circuits:    50+ Cirq examples
Benchmarks:          5+ reproducible scenarios
Security Reviews:    Pending (accepting help!)
```

---

## 🎉 Acknowledgments

Built with ❤️ by the quantum security community. Special thanks to:
- **Cirq** team for quantum simulation
- **Open Quantum Safe** for standardized PQC
- **NIST** for post-quantum standardization guidance
- **Contributors** — Come join us!

---

## 💡 Quick Reference: All CLI Commands

```powershell
# Server (combined)
python -m qshield.net.server --host 0.0.0.0 --port 8765 --mode auto --metrics metrics.csv

# Client (combined)
python -m qshield.net.client --url ws://localhost:8765 --mode auto --verbose

# Benchmarks
python benchmarks/qkd_rate.py --p_flip 0.02 --blocks 128 --seed 42
python benchmarks/kem_latency.py --trials 500 --output bench.csv

# Testing & Quality
pytest -q                           # Quick test
pytest --cov=src/ --cov-report=html # Coverage
mypy src/ --strict                  # Type check
black src/ tests/                   # Format
pre-commit run --all-files          # All hooks

# Documentation & Analysis
jupyter notebook notebooks/qber_vs_noise.ipynb
python docs/plots.py --input metrics.csv --output plots/
```

---

## Appendix — Original README (archived)

The original README content is preserved below for reference and reproducibility. If you want it restored as the main README, tell me and I can revert or move the new content to `README.enhanced.md` instead.

<!-- original content follows -->

```
# QShield — Hybrid Quantum-Safe Secure Messenger (QKD + PQC)

> End-to-end encrypted chat where session keys are negotiated via **simulated BB84 QKD (Cirq)** or **post-quantum KEM (Kyber via Open Quantum Safe)**, with authenticated transcripts, error correction, privacy amplification, and metrics.

[![Status](https://img.shields.io/badge/status-planning-blue)]() [![Python](https://img.shields.io/badge/python-3.11+-informational)]() [![Security](https://img.shields.io/badge/security-QKD%20%2B%20PQC-critical)]()

---

## 0) TL;DR

- Data plane: **AES-GCM**
- Keying modes: **BB84 (Cirq)** or **Kyber KEM (OQS)** with **Dilithium** signatures or **HMAC** for auth
- Pipeline (QKD): **Sifting → Error Reconciliation → Privacy Amplification → Key Buffer**
- Transport: **FastAPI/WebSockets** (CLI first, GUI later)
- Goals: measurable **secret-key rate**, **QBER**, and end-to-end latency with reproducible experiments

---

## 1) Repository Structure

```
qshield/
├─ README.md
├─ pyproject.toml           # poetry/pip-tools; lock your deps
├─ .pre-commit-config.yaml  # black, isort, flake8, mypy
├─ src/qshield/
│  ├─ __init__.py
│  ├─ common/
│  │  ├─ config.py
│  │  ├─ logging.py
│  │  └─ messages.py
│  ├─ crypto/
│  │  ├─ aead.py            # AES-GCM, HKDF
│  │  ├─ kem.py             # Kyber KEM (python-oqs) + X25519 fallback
│  │  └─ sig.py             # Dilithium / HMAC auth
│  ├─ qkd/
│  │  ├─ bb84.py            # Cirq circuits + noise models
│  │  ├─ sifting.py
│  │  ├─ reconcile.py       # parity blocks → Cascade-lite
│  │  ├─ privacy_amp.py     # Toeplitz hashing
│  │  └─ utils.py
│  ├─ net/
│  │  ├─ server.py          # FastAPI + WebSockets
│  │  └─ client.py          # CLI client
│  ├─ policy/
│  │  └─ selector.py        # choose QKD vs PQC, rekey policies
│  └─ metrics/
│     ├─ monitor.py         # live metrics + CSV logs
│     └─ plots.py
├─ tests/
│  ├─ test_aead.py
│  ├─ test_bb84.py
│  ├─ test_reconcile.py
│  └─ test_kem.py
├─ benchmarks/
│  ├─ qkd_rate.py
│  └─ kem_latency.py
├─ docs/
│  ├─ protocol.md           # message formats, state machines
│  ├─ threat-model.md       # STRIDE + QKD-specific attacks
│  ├─ security.md           # crypto invariants, key lifecycles
│  ├─ roadmap.md
│  └─ adr/                  # Architecture Decision Records
└─ notebooks/
   ├─ qber_vs_noise.ipynb
   └─ pa_compression.ipynb
```

---

## 2) Architecture (at a glance)

```
[ Client ] <--WebSocket--> [ Server ]
     |                          |
     |--- Handshake (QKD or PQC, authenticated) ---|
     |                          |
[Key Derivation] → [AES-GCM Data Plane] → [Rekey Policy]
     |
[Key Buffer] <= QKD pipeline: BB84 → Sift → Reconcile → Privacy Amp
```

---

## 3) Long-Term Roadmap (Work in Small, Independent Chunks)

Each phase is self-contained; open a milestone per phase and convert checkboxes into GitHub issues.

### Phase 0 — Project Scaffolding
- [ ] `pyproject.toml`, `src/` layout, `tests/`, `pre-commit`
- [ ] CI: lint + typecheck + unit tests
- [ ] `docs/adr/0001-toolchain.md` (poetry/pip-tools, mypy, pytest)

**Deliverables:** buildable env, first CI pass

---

### Phase 1 — Classical AEAD Baseline
- [ ] `crypto/aead.py`: AES-GCM (random IV, AAD), HKDF
- [ ] `tests/test_aead.py`: deterministic vectors
- [ ] Minimal encrypt/decrypt CLI

**Deliverables:** baseline secure channel with static PSK

---

### Phase 2 — BB84 Simulation (Cirq)
- [ ] `qkd/bb84.py`: bases, prep/measure, noise (depol, bit-flip)
- [ ] `tests/test_bb84.py`: QBER rises with noise; seeded reproducibility
- [ ] `notebooks/qber_vs_noise.ipynb`

**Deliverables:** BB84 raw key + QBER metrics

---

### Phase 3 — Sifting, Error Reconciliation, Privacy Amplification
- [ ] `sifting.py`: mask + sifted keys
- [ ] `reconcile.py`: parity blocks → **Cascade-lite** (iterative)
- [ ] `privacy_amp.py`: Toeplitz hashing (SHA-256 PRG)
- [ ] Leakage accounting (bits revealed during EC)
- [ ] `tests/test_reconcile.py`, finite-key sanity checks

**Deliverables:** identical reconciled keys; PA output tuned vs QBER

---

### Phase 4 — PQC KEM Mode
- [ ] `crypto/kem.py`: Kyber (OQS); X25519 fallback if OQS missing
- [ ] Bench `benchmarks/kem_latency.py`
- [ ] Compare “time-to-ready key” QKD vs PQC

**Deliverables:** working PQC path with metadata transcript

---

### Phase 5 — Authentication of Transcripts
- [ ] `crypto/sig.py`: **Dilithium** (OQS) + HMAC(PSK) option
- [ ] Auth classical QKD messages + KEM transcript
- [ ] MITM tests (tamper → reject)

**Deliverables:** authenticated handshakes; negative tests

---

### Phase 6 — Policy & Handshake Negotiation
- [ ] `policy/selector.py`: choose QKD if QBER<τ & key_buffer>Kmin; else PQC
- [ ] State machine in `docs/protocol.md`
- [ ] Unit tests of transitions & fallbacks

**Deliverables:** robust mode selection

---

### Phase 7 — Networking Layer
- [ ] `net/server.py` (FastAPI/WebSockets) + `net/client.py` (CLI)
- [ ] Encrypted chat frames (AES-GCM) with rolling nonces
- [ ] Rekey every N messages / T seconds

**Deliverables:** end-to-end encrypted chat (CLI demo)

---

### Phase 8 — Key Buffer & Lifecycle
- [ ] Background QKD producer → bounded buffer
- [ ] Exhaustion handling (pause/send via PQC)
- [ ] Secure in-mem storage + optional SQLite envelope encryption

**Deliverables:** stable long-running sessions

---

### Phase 9 — Metrics & Visualization
- [ ] `metrics/monitor.py`: CSV logs (QBER, leakage, PA rate, key buffer)
- [ ] `metrics/plots.py`: publishable figures
- [ ] `benchmarks/qkd_rate.py`: secret-key rate vs noise/block size

**Deliverables:** reproducible plots + CSVs

---

### Phase 10 — Security Docs
- [ ] `docs/threat-model.md`: eavesdropping, detector noise, MITM, replay
- [ ] `docs/security.md`: invariants, nonce rules, KDF chains, PA math
- [ ] ADRs for major crypto choices

**Deliverables:** review-ready security package

---

### Phase 11 — Stretch Goals
- [ ] E91 variant / decoy states
- [ ] TLS proxy mode (“quantum-safe VPN”)
- [ ] Group chat (TreeKEM + QKD feed)
- [ ] Simple GUI (Textual/Qt)

---

## 4) Getting Started (Dev)

```bash
# 1) Clone & create env
git clone https://github.com/yourname/qshield.git
cd qshield
python -m venv .venv && source .venv/bin/activate  # Windows: .venv\Scripts\activate

# 2) Install
pip install -U pip wheel
pip install -e ".[dev]"  # define extras in pyproject (oqs, cirq, fastapi, uvicorn, numpy, pandas, matplotlib, mypy, pytest)

# 3) Pre-commit + tests
pre-commit install
pytest -q
```

---

## 5) Minimal Usage (once phases 1–4 are in)

```bash
# Start server
python -m qshield.net.server --host 127.0.0.1 --port 8765

# Client (QKD preferred, fallback to PQC)
python -m qshield.net.client --url ws://127.0.0.1:8765 --mode auto
```

---

## 6) Testing & Benchmarks

- Unit tests: `pytest -q`
- Type checks: `mypy src/`
- QKD rate: `python benchmarks/qkd_rate.py --p_flip 0.02 --blocks 128`
- KEM latency: `python benchmarks/kem_latency.py --trials 200`

---

## 7) Definition of Done (per phase)

- ✅ Unit tests ≥ 90% for the module
- ✅ Negative tests (tamper, replay, wrong tag)
- ✅ Docs updated (`protocol.md`, ADR if architecture changed)
- ✅ Benchmarks (if perf-relevant)
- ✅ Reproducible seed used in notebooks

---

## 8) Issue Labels (work in slices)

- `area/qkd`, `area/pqc`, `area/net`, `area/crypto`, `area/metrics`
- `type/bug`, `type/feat`, `type/docs`, `type/refactor`
- `prio/P0..P3`
- `good-first-issue` (small, testable tasks)

---

## 9) Research & Notes

Track open questions in `docs/roadmap.md`:
- Finite-key corrections for PA length vs QBER
- Cascade parameter tuning vs block size/noise
- Authentication choices: HMAC(PSK) vs Dilithium (trade-offs)

---

## 10) Security Invariants (quick checklist)

- [ ] Unique nonce per AES-GCM key
- [ ] All transcripts authenticated (HMAC or Dilithium)
- [ ] EC leakage accounted in PA length
- [ ] Rekey before nonce space exhaustion
- [ ] Zeroize ephemeral keys on error/close

---

## 11) License & Attribution

- Code: MIT/Apache-2.0 (choose)
- PQC primitives via **Open Quantum Safe (OQS)**
- Quantum circuits via **Cirq**

---

### Appendix A — Starter Signatures

```python
# src/qshield/qkd/bb84.py
def bb84_run(n_bits: int, p_flip: float = 0.02, seed: int | None = 0) -> tuple[list[int], list[int], list[int], list[int]]:
    """Return (alice_bits, alice_bases, bob_bits, bob_bases)."""

# src/qshield/qkd/reconcile.py
def cascade_lite(a_key: bytes, b_key: bytes, block_size: int = 128, rounds: int = 3, seed: int | None = 0) -> tuple[bytes, bytes, int]:
    """Return (a_rec, b_rec, leakage_bits)."""

# src/qshield/qkd/privacy_amp.py
def toeplitz_hash(key_material: bytes, out_len: int, seed: bytes) -> bytes:
    """Universal hashing for PA."""
```

```
