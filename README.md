<img src="./assets/banner.svg" alt="Zeno Vangue" width="100%">

<p align="center">
  <a href="mailto:contact@zenovangue.com"><img src="https://img.shields.io/badge/EMAIL-contact%40zenovangue.com-8b5cf6?style=flat-square&labelColor=000000" alt="Email"></a>
  <img src="https://img.shields.io/badge/DISCORD-zenovangue-8b5cf6?style=flat-square&logo=discord&logoColor=white&labelColor=000000" alt="Discord">
  <img src="https://img.shields.io/badge/HOURS-CET%20%2F%20CEST-8b5cf6?style=flat-square&labelColor=000000" alt="Working hours">
  <a href="https://github.com/zenovangue?tab=repositories"><img src="https://img.shields.io/badge/REPOS-8-8b5cf6?style=flat-square&labelColor=000000" alt="Repositories"></a>
</p>

## About

Independent engineer and algorithmic trader. I build trading infrastructure end to end: research tooling, execution engines, backtesting platforms, and the interfaces on top of them.

> Low-latency execution logic, grounded in statistical rigor and hardware-aware design.

**Focus areas**

| Area | What I work on |
| :--- | :--- |
| **Systems** | Rust execution engines, shared-memory IPC, zero-copy data paths, kernel-bypass I/O |
| **Quant research** | Regime detection (HMM / HSMM / Kalman), walk-forward validation, CPCV, Monte Carlo |
| **Platforms** | MT5 (MQL5), cTrader (cAlgo), NinjaTrader, TradingView (Pine Script), NautilusTrader |
| **Web** | Landing pages, dashboards, desktop apps with Tauri |
| **AI-assisted engineering** | Phased master prompts for building complete software with LLMs |

---

## Tech Stack

**Languages**

<img src="https://skillicons.dev/icons?i=rust,go,py,cs,cpp,ts,js&theme=dark" alt="Languages">

**Web and desktop**

<img src="https://skillicons.dev/icons?i=html,css,react,svelte,threejs,tauri&theme=dark" alt="Web and desktop">

**Tools and environment**

<img src="https://skillicons.dev/icons?i=linux,git,github,vscode,docker,pytorch&theme=dark" alt="Tools">

**Libraries and data**

`Burn` · `wgpu` · `FlatBuffers` · `memmap2` · `Polars` · `Numba` · `Parquet` · `LightGBM` · `Stable-Baselines3` · `ONNX` · `PySide6`

**Data sources**

`Dukascopy` tick data · `cTrader Open API` · `Kaggle` GPU notebooks

---

## Technical Skills

### Rust and low-level systems
- Lock-free structures and shared-memory ring buffers
- Zero-copy serialization and memory-mapped data pipelines
- Cache-aware layout, `mlock`, CPU pinning, process isolation
- From-scratch models in Rust: Gaussian HMM, Kalman filter, ATR, fixed-fractional risk sizing
- Multi-crate Cargo workspaces; Rust, Python, C# AOT and Go interop

### Quantitative research
- Market regime detection with HMM, HSMM, GMM and Kalman filtering
- Tick-level reinforcement learning (PPO) with ONNX export for Rust inference
- LightGBM signal models on 500-tick event bars, 3-class SKIP / BUY / SELL
- Validation: walk-forward optimization, CPCV, Monte Carlo, overfitting detection
- Position sizing: fixed-fractional risk, Kelly, ATR-based stops

### Trading platforms
- MQL5 expert advisors, including multi-timeframe confluence systems
- cAlgo C# cBots, including MQL5 to cAlgo conversions
- NinjaTrader strategies, TradingView Pine Script
- Shared risk logic across MT5, NinjaTrader and cTrader

### Web and desktop
- Cinematic landing pages: scroll-driven animation, 3D, looping video heroes
- React and TypeScript components; Tauri 2 + Svelte desktop apps
- PySide6 trading workstations
- Semantic HTML, modern CSS, responsive layouts

### Prompt engineering
- Phased specifications with acceptance criteria per phase
- Constraint-driven prompts: explicit stack, file layout, performance targets, failure modes
- Generator scripts that output complete project trees
- Root-cause debugging prompts for ML and quant pipelines

---

## Projects

| Project | Stack | Description |
| :--- | :--- | :--- |
| **Aethelgard NANO-GRID** | Rust | HFT framework: 8-crate workspace, Dukascopy ingestion, shared-memory IPC, `alpha_rsi` reference strategy |
| **Aegis Engine** | Go, Python, Numba, Polars | Backtesting platform with Dukascopy downloader and proxy rotation |
| **XAU Glass** | Tauri 2, Rust, Svelte | XAUUSD research and paper-trading desktop app |
| **Regime-Switching Bot** | Python, HMM | Regime detection routing to trend-following or mean-reversion logic |
| **Tick RL Pipeline** | PPO, Polars, ONNX | Tick-by-tick RL on Dukascopy data, exported for Rust |
| **Multi-Platform EAs** | MQL5, cAlgo, NinjaTrader | Strategies with consistent risk management across platforms |

**NANO-GRID design targets** (targets, not measured benchmarks): sub-50 ns IPC feedback loop, 300M ticks/s ingestion.

---

## Working Hours

European time (CET / CEST). Async-friendly, documentation-first. Email or Discord, usually within one business day.

Open to: trading-system builds, Rust engineering, quant infrastructure, landing pages and web apps, prompt engineering.

---

## GitHub Stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=zenovangue&show_icons=true&hide_border=false&bg_color=000000&title_color=a78bfa&text_color=e5e5e5&icon_color=8b5cf6&border_color=2a2a2e" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zenovangue&layout=compact&bg_color=000000&title_color=a78bfa&text_color=e5e5e5&border_color=2a2a2e" alt="Top languages">
</p>

---

## Contact

| | |
| :--- | :--- |
| **Email** | [contact@zenovangue.com](mailto:contact@zenovangue.com) |
| **Discord** | `zenovangue` |
| **GitHub** | [@zenovangue](https://github.com/zenovangue) |
