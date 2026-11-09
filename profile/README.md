<div align="center">

# Vigyan Workstation
### Sovereign Offline Physical Engineering Intelligence & STEM Studio

[![Repository](https://img.shields.io/badge/Flagship_Repository-vigyan--pro_v4.1.0-000000?style=flat&logo=github&logoColor=white)](https://github.com/Vigyan-workstation/vigyan-pro)
[![Hugging Face](https://img.shields.io/badge/Hugging_Face-Experimentlab-ffd21e?style=flat&logo=huggingface&logoColor=black)](https://huggingface.co/Experimentlab)
[![Discord](https://img.shields.io/badge/Discord-Experimentlab_Community-5865F2?style=flat&logo=discord&logoColor=white)](https://discord.com/invite/Jck3tD6mhf)
[![License](https://img.shields.io/badge/License-PolyForm_Noncommercial_1.0.0-blue.svg?style=flat)](https://github.com/Vigyan-workstation/vigyan-pro/blob/main/LICENSE)
[![Back Research](https://img.shields.io/badge/Back_Research-Buy_Me_A_Chai-d97706?style=flat)](https://buymeachai.in/shreyansh001boy)
[![CI Matrix](https://img.shields.io/badge/CI_Matrix-Ubuntu_%7C_macOS_%7C_Windows-success?style=flat)](https://github.com/Vigyan-workstation/vigyan-pro/actions)

<p align="center">
  <b>100% offline, privacy-first desktop workstation and domain-specialized foundation models engineered for physical engineers, mathematicians, and autonomous agent swarms.</b>
</p>

</div>

---

## Technical Philosophy

Vigyan pairs domain-specialized Small Language Models (SLMs) with a deterministic Computer Algebra System (SymPy CAS) and local multiphysics engines.

While generative neural networks effectively decompose physical problems into mathematical formulations, they are inherently prone to probabilistic arithmetic errors. Vigyan guarantees absolute mathematical truth by executing all calculus, differential equations, and algebraic proofs through an in-process, sandboxed Computer Algebra System AST kernel.

* **Air-Gap Sovereign Execution**: Operates completely offline with zero telemetry, zero analytics, and zero external cloud API egress.
* **Deterministic Symbolic Verification**: Eliminates hallucinated calculus, ODEs, and scientific constants via formal CAS grounding.
* **Resource-Governed Runtime**: Engineered to run smoothly on standard consumer hardware (less than 4 GB RAM footprint) without discrete GPUs.

---

## Flagship Repository: Vigyan Pro v4.1.0 (Sovereign Engineering Edition)

The flagship workstation is actively developed and maintained in **[Vigyan-workstation/vigyan-pro](https://github.com/Vigyan-workstation/vigyan-pro)**.

### 1-Click Multi-OS Installation

#### Linux (Debian / Ubuntu / Pop!_OS / Mint)
```bash
# Download official release package & install
wget https://github.com/Vigyan-workstation/vigyan-pro/releases/download/v4.1.0/vigyan-pro_4.1.0_amd64.deb
sudo apt install ./vigyan-pro_4.1.0_amd64.deb

# Launch workstation
vigyan-pro
```

#### Linux Portable Archive (Arch, Fedora, openSUSE, RHEL)
```bash
wget https://github.com/Vigyan-workstation/vigyan-pro/releases/download/v4.1.0/vigyan-pro-4.1.0.tar.gz
tar -xzf vigyan-pro-4.1.0.tar.gz
cd vigyan-pro-4.1.0 && ./vigyan-pro
```

#### Windows 10/11 (PowerShell / Command Prompt)
```powershell
# Extract release zip and double-click Vigyan-Pro.bat (powered by Microsoft Edge WebView2)
Expand-Archive -Path vigyan-pro-4.1.0.zip -DestinationPath C:\VigyanPro
cd C:\VigyanPro
.\Vigyan-Pro.bat
```

#### macOS (Apple Silicon & Intel)
```bash
# Extract and launch native Apple Cocoa WKWebView studio
tar -xzf vigyan-pro-4.1.0.tar.gz
cd vigyan-pro-4.1.0
./Vigyan-Pro.command
```

---

### Core Capabilities (v4.1.0)

1. **Deterministic Computer Algebra Engine (SymPy CAS)**:
   In-process SymPy AST kernel with strict sandboxing against arbitrary code injection or namespace pollution.
   ```bash
   vigyan math "diff(sin(x)*exp(x), x)"
   vigyan math "solve(x**2 - 5*x + 6, x)"
   ```

2. **Parametric 3D CAD & Mesh Generation**:
   Integrated `build123d` and `OpenCASCADE` engine generating manufacturing-ready STL solid meshes on-device, rendered in an interactive Three.js turntable viewport.
   ```bash
   vigyan cad "box(10, 20, 30) - cylinder(r=3, h=30)"
   ```

3. **SciPy RK45 Multiphysics Simulation**:
   Adaptive ODE numerical solver returning full 100-point ballistic drag and oscillator trajectories with interactive 60 FPS browser sliders.
   ```bash
   vigyan sim "d2x/dt2 + 0.1*dx/dt + 9.8*sin(x) = 0"
   ```

4. **RDKit Cheminformatics & Dimensional Algebra**:
   Molecular descriptor evaluation (MW, LogP, TPSA, HBD, HBA), vector SVG bond rendering, and rigorous dimensional verification via Pint & Astropy:
   ```bash
   vigyan chem "CC(=O)Oc1ccccc1C(=O)O"
   vigyan unit "100 km/h to m/s"
   ```

5. **Typst Vector PDF Compiler (<50ms)**:
   Embedded Rust compiler generating publication-ready vector academic papers with embedded SymPy verification badges, replacing heavy 2 GB TeXLive dependencies.

6. **First-Class GGUF Model Management & Local Supervisor**:
   Discovers local models, calculates host RAM headroom, manages embedded `llama-server` on loopback with automatic 10-minute idle memory reclamation.
   ```bash
   vigyan model status
   vigyan model list --remote
   vigyan model pull vigyan-3b-quad-master-iq3_m.gguf
   ```

7. **Autonomous Learning Ledger**:
   Dynamic in-context rule learning backed by a lightweight, reversible git ledger:
   ```bash
   vigyan learn "Always derive equations in SI units before evaluating numbers"
   vigyan ledger
   vigyan undo
   ```

8. **Multi-OS Native Desktop Shells**:
   Native desktop application powered by WebKitGTK (Linux), Microsoft Edge WebView2 (Windows), and Apple Cocoa WKWebView (macOS) with modern reactive Svelte 5 UI components.

---

## Hugging Face Model Ecosystem

Our foundation models, quantized edge runtimes, and pre-training corpora are published under the **[Experimentlab](https://huggingface.co/Experimentlab)** organization:

| Tier | Category | Key Models & Repositories | Target Deployment |
| :--- | :--- | :--- | :--- |
| **Tier 1** | **Edge GGUF Runtimes** | [`Experimentlab/Vigyan-Models-GGUF`](https://huggingface.co/Experimentlab/Vigyan-Models-GGUF) | Laptops, edge CPUs (&lt;4 GB RAM) |
| **Tier 2** | **Sparse Mixture of Experts** | [`Experimentlab/Vigyan-1.5B-4x-MoE`](https://huggingface.co/Experimentlab/Vigyan-1.5B-4x-MoE) | High-throughput local reasoning |
| **Tier 3** | **Foundation STEM SLMs** | [`Experimentlab/Vigyan-AI-32B`](https://huggingface.co/Experimentlab/Vigyan-AI-32B)<br>[`Experimentlab/Vigyan-7B-STEM-Instruct-v1`](https://huggingface.co/Experimentlab/Vigyan-7B-STEM-Instruct-v1)<br>[`Experimentlab/Shreyansh-STEM-AI-2B-v3`](https://huggingface.co/Experimentlab/Shreyansh-STEM-AI-2B-v3) | Deep multi-step scientific deduction |
| **Tier 4** | **Domain Checkpoints** | [`Experimentlab/olmo2-7b-silicon-rtl-eda`](https://huggingface.co/Experimentlab/olmo2-7b-silicon-rtl-eda) (Verilog)<br>[`Experimentlab/olmo2-7b-phd-pure-math`](https://huggingface.co/Experimentlab/olmo2-7b-phd-pure-math) (Calculus) | Specialized doctoral benchmarks |
| **Data** | **Pretraining & Papers** | [`Experimentlab/vigyan-ai-research-papers`](https://huggingface.co/datasets/Experimentlab/vigyan-ai-research-papers) | Research evaluation |

---

## AI Coding Agent Contribution Standard

Vigyan Pro provides dedicated architectural directives for autonomous AI coding agents:

* **[AGENTS.md](https://github.com/Vigyan-workstation/vigyan-pro/blob/main/AGENTS.md)**: Universal specification declaring 6 sovereign invariants (Zero Local Compute, Host RAM Governor, Zero Emojis, SymPy AST Sandboxing, Air-Gap Egress Lock, Learning Ledger Integrity).
* **[CLAUDE.md](https://github.com/Vigyan-workstation/vigyan-pro/blob/main/CLAUDE.md)**: Configuration and CLI command map for Claude Code.
* **[.cursorrules](https://github.com/Vigyan-workstation/vigyan-pro/blob/main/.cursorrules)**: In-editor rules for Cursor IDE.
* **[.github/copilot-instructions.md](https://github.com/Vigyan-workstation/vigyan-pro/blob/main/.github/copilot-instructions.md)**: Guidelines for GitHub Copilot Workspace.
* **Automated Guardrail Enforcement**: Every pull request is verified by `scripts/verify_agent_guardrails.py` in GitHub Actions CI across all platforms.

---

## Community & Discussion

Real-time collaboration, research discussions, and workstation support take place on our official Discord server:

* **Discord Server**: **[Experimentlab Community](https://discord.com/invite/Jck3tD6mhf)** (65+ Members)
* **Key Channels**:
  * `#announcements`: Official releases, model uploads, and architectural papers.
  * `#workstation`: Setup assistance, bug reports, and hardware optimization.
  * `#research`: Foundation models, pre-training corpora, MoE routing, and symbolic CAS.
  * `#model-evals`: Empirical benchmarking, GSM8K, MATH, and Verilog synthesis evaluations.

---

## Legal, Intellectual Property & Non-Commercial Licensing

All source code, software binaries, and documentation released across the Vigyan Workstation organization are governed by the **PolyForm Noncommercial License 1.0.0**:

* **Academic, Educational & Personal Research Use**: Free to use, inspect, modify, and run offline for non-commercial purposes.
* **AI Model Distillation Restriction (Section 8)**: You may not use the software, source code, documentation, or model outputs to train, align, distill, or evaluate competing artificial intelligence or foundation models without prior written permission.
* **Trademark Protection (Section 9)**: No trademark, service mark, or brand rights in "ExperimentLab AI" or "Vigyan Pro" are granted.
* **Contributor Certificate of Origin (DCO v1.1)**: All contributions must include a valid `Signed-off-by:` trailer certifying original authorship or proper licensing.
* **Commercial Enterprise Licensing**: For commercial licensing, enterprise deployment, or OEM hardware distribution, contact **support@experimentlab.in**.

---

<div align="center">
  <sub>Developed by <a href="https://experimentlab.in">ExperimentLab AI</a>. Built for physical engineers who value sovereignty and mathematical precision.</sub>
</div>
