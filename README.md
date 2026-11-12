<img src="./assets/banner.svg" alt="Zeno Vangue" width="100%">

<p align="center">
  <a href="mailto:contact@zenovangue.com"><img src="https://img.shields.io/badge/EMAIL-contact%40zenovangue.com-8b5cf6?style=for-the-badge&labelColor=000000" alt="Email"></a>
  <img src="https://img.shields.io/badge/DISCORD-zenovangue-8b5cf6?style=for-the-badge&logo=discord&logoColor=white&labelColor=000000" alt="Discord">
  <img src="https://img.shields.io/badge/HOURS-CET%20%2F%20CEST-8b5cf6?style=for-the-badge&labelColor=000000" alt="Working hours">
</p>

## About

I am an independent engineer and algorithmic trader. I build trading infrastructure end to end: research tooling, execution engines, backtesting platforms, and the interfaces that sit on top of them.

My approach is systems-first. I prefer explicit architecture, measurable targets, strict validation, and code that is easy to reason about under load. I use AI assistants such as Claude as part of the engineering workflow, with structured specifications and review loops rather than ad hoc prompting.

> Low-latency execution logic, grounded in statistical rigor and hardware-aware design.

### Focus areas

| Area | What I work on |
| :--- | :--- |
| **Systems** | Rust execution engines, shared-memory IPC, zero-copy data paths, kernel-bypass I/O |
| **Quant research** | Regime detection (HMM, HSMM, Kalman), walk-forward validation, CPCV, Monte Carlo |
| **Trading platforms** | MT5 (MQL5), cTrader (cAlgo), NinjaTrader, TradingView (Pine Script), NautilusTrader |
| **Web and desktop** | Landing pages, dashboards, Tauri desktop applications |
| **AI-assisted engineering** | Phased master prompts and review loops for building complete software with LLMs |

---

## Tech Stack

### Languages

<img src="https://skillicons.dev/icons?i=rust,go,py,cs,cpp,ts,js&theme=dark" alt="Languages">

### Web and desktop

<img src="https://skillicons.dev/icons?i=html,css,react,svelte,threejs,tauri&theme=dark" alt="Web and desktop">

### Tools and environment

<img src="https://skillicons.dev/icons?i=linux,git,github,vscode,docker,pytorch&theme=dark" alt="Tools and environment">

### AI tooling

<p>
  <img src="https://img.shields.io/badge/Claude-000000?style=for-the-badge&logo=claude&logoColor=D97757" alt="Claude">
  <img src="https://img.shields.io/badge/Anthropic-000000?style=for-the-badge&logo=anthropic&logoColor=white" alt="Anthropic">
  <img src="https://img.shields.io/badge/Prompt_Engineering-000000?style=for-the-badge&logo=openai&logoColor=a78bfa" alt="Prompt Engineering">
</p>

### Libraries, frameworks and data

| Category | Tools |
| :--- | :--- |
| **Rust** | `Burn` · `wgpu` · `FlatBuffers` · `memmap2` · `Tauri 2` |
| **Python** | `Polars` · `Numba` · `LightGBM` · `Stable-Baselines3` · `PySide6` · `vn.py` |
| **Formats and runtime** | `Parquet` · `ONNX` |
| **Data sources** | `Dukascopy` tick data · `cTrader Open API` · `Kaggle` GPU notebooks |

---

## Technical Skills

### Rust and low-level systems

- Lock-free structures and shared-memory IPC ring buffers
- Zero-copy serialization (FlatBuffers) and memory-mapped data pipelines
- Cache-aware data layout (L1/L2/L3), `mlock`, CPU pinning, process isolation
- From-scratch statistical models in Rust: Gaussian HMM, Kalman filter, ATR, fixed-fractional risk sizing
- Multi-crate Cargo workspaces with clear module boundaries
- Interoperability between Rust, Python, C# AOT and Go runtimes
- GPU compute with `wgpu` shaders for parallel optimization workloads

### Quantitative research and machine learning

- Market regime detection with HMM, HSMM, GMM and Kalman filtering
- Tick-level reinforcement learning (PPO) with ONNX export for Rust inference
- LightGBM signal models on 500-tick event bars (3-class SKIP / BUY / SELL)
- Feature engineering at scale on Dukascopy tick data stored as Parquet
- Validation discipline: walk-forward optimization, CPCV, Monte Carlo, overfitting detection
- Position sizing: fixed-fractional risk, Kelly criterion, ATR-based stops

### Trading platform development

- MQL5 expert advisors, including multi-timeframe confluence systems
- cAlgo C# cBots for cTrader, including MQL5-to-cAlgo conversions
- NinjaTrader strategies in C#
- TradingView strategies in Pine Script
- Shared risk logic across MT5, NinjaTrader and cTrader
- Backtesting and research platforms (Go, Python, Parquet) with proxy-aware data downloaders

### Web and desktop development

- Cinematic landing pages: scroll-driven animation, 3D, looping video heroes
- React and TypeScript component development
- Desktop applications with Tauri 2, Rust and Svelte
- PySide6 trading workstations
- Semantic HTML, modern CSS, responsive and accessible layouts
- Data-heavy dashboards for trading and research

### AI-assisted engineering and prompt engineering

- Phased specifications with acceptance criteria per phase
- Constraint-driven prompts: explicit stack, file layout, performance targets and failure modes
- Generator scripts that output complete project trees from a single file
- Root-cause debugging prompts for ML and quant pipelines
- Review loops: iterating specifications against real output until results are deterministic
- Daily use of Claude for design review, code generation and refactoring, always followed by manual verification

---

## Engineering Principles

1. **Measure before claiming.** Performance figures are labelled as targets until benchmarked.
2. **Validate out of sample.** A backtest is not evidence until it survives walk-forward and CPCV.
3. **Isolate failure.** Process boundaries and explicit interfaces over shared mutable state.
4. **Keep the hot path simple.** No allocation, no locks, no surprises where latency matters.
5. **Document decisions.** Architecture notes and acceptance criteria live next to the code.

---

## Projects

| Project | Stack | Description |
| :--- | :--- | :--- |
| **Aethelgard NANO-GRID** | Rust | Low-latency trading framework: 8-crate workspace, Dukascopy ingestion, shared-memory IPC, `alpha_rsi` reference strategy |
| **Aegis Engine** | Go, Python, Numba, Polars | Backtesting platform with Dukascopy downloader and proxy rotation |
| **XAU Glass** | Tauri 2, Rust, Svelte | XAUUSD research and paper-trading desktop application |
| **Regime-Switching Bot** | Python, HMM | Regime detection routing to trend-following or mean-reversion logic |
| **Tick RL Pipeline** | PPO, Polars, ONNX | Tick-by-tick reinforcement learning on Dukascopy data, exported for Rust inference |
| **Multi-Platform EAs** | MQL5, cAlgo, NinjaTrader | Strategies with consistent risk management across platforms |

### Flagship: Aethelgard NANO-GRID

A pure-Rust execution framework designed to avoid kernel scheduling overhead on the hot path and to keep data movement explicit.

- **Data ingestion:** async Dukascopy byte extraction with optimized binary storage, designed to stream hundreds of millions of ticks mapped to CPU cache blocks.
- **Process isolation:** multi-core sandboxing with lock-free shared-memory IPC ring buffers, integrating Rust, Python and C# AOT strategies.
- **Design targets (not measured benchmarks):** sub-50 ns IPC feedback loop, 300M ticks per second ingestion.

---

## Working Hours

European time (CET / CEST). Async-friendly and documentation-first. Email or Discord, usually within one business day.

**Open to:** trading-system builds, Rust engineering, quant infrastructure, landing pages and web applications, prompt engineering.

---

## GitHub Stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=zenovangue&show_icons=true&bg_color=000000&title_color=a78bfa&text_color=e5e5e5&icon_color=8b5cf6&border_color=2a2a2e" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zenovangue&layout=compact&bg_color=000000&title_color=a78bfa&text_color=e5e5e5&border_color=2a2a2e" alt="Top languages">
</p>

---

## Contact

| | |
| :--- | :--- |
| **Email** | [contact@zenovangue.com](mailto:contact@zenovangue.com) |
| **Discord** | `zenovangue` |
| **GitHub** | [@zenovangue](https://github.com/zenovangue) |
| **Hours** | CET / CEST |
