<img src="https://raw.githubusercontent.com/zenovangue/zenovangue/main/assets/banner.gif" alt="Banner" width="100%">

<p align="center">
  <a href="mailto:contact@zenovangue.com"><img src="https://img.shields.io/badge/EMAIL-contact%40zenovangue.com-71717a?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0naHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmcnIHZpZXdCb3g9JzAgMCAyNCAyNCcgZmlsbD0nd2hpdGUnPjxwYXRoIGQ9J00yMCA0SDRhMiAyIDAgMCAwLTIgMnYxMmEyIDIgMCAwIDAgMiAyaDE2YTIgMiAwIDAgMCAyLTJWNmEyIDIgMCAwIDAtMi0yem0wIDQtOCA1LTgtNVY2bDggNSA4LTV2MnonLz48L3N2Zz4%3D&logoColor=white&labelColor=000000" alt="Email"></a>
  <img src="https://img.shields.io/badge/DISCORD-zenovangue-71717a?style=for-the-badge&logo=discord&logoColor=white&labelColor=000000" alt="Discord">
  <img src="https://img.shields.io/badge/HOURS-CET%20%2F%20CEST-71717a?style=for-the-badge&labelColor=000000" alt="Working hours">
</p>

## About

I am an independent engineer and algorithmic trader. I build trading infrastructure end to end: research tooling, execution engines, backtesting platforms, and the interfaces that sit on top of them.

My approach is systems-first. I prefer explicit architecture, measurable targets, strict validation, and code that is easy to reason about under load.

> Low-latency execution logic, grounded in statistical rigor and hardware-aware design.

### Focus areas

| Area | What I work on |
| :--- | :--- |
| **Systems** | Rust execution engines, shared-memory IPC, zero-copy data paths, kernel-bypass I/O |
| **Quant research** | Regime detection (HMM, HSMM, Kalman), walk-forward validation, CPCV, Monte Carlo |
| **Strategy engineering** | Turning visual (price-action) strategies into precise, testable trading algorithms, filters and adaptive indicators |
| **Trading platforms** | MT5 (MQL5), cTrader (cAlgo C#), NinjaTrader, TradingView (Pine Script v6), NautilusTrader |
| **Custom platforms** | Research and execution platforms, FIX protocol connectivity, CLI tools and GUI applications |
| **Full-stack web** | Complete websites and web applications: frontend, backend APIs, databases, with security and encryption |
| **Desktop** | Tauri desktop applications, PySide6 trading workstations |

---

## Tech Stack

### Languages

<img src="https://skillicons.dev/icons?i=rust,go,py,cs,cpp,ts,js&theme=dark" alt="Languages">

### Web and desktop

<img src="https://skillicons.dev/icons?i=html,css,react,svelte,threejs,tauri&theme=dark" alt="Web and desktop">

### Tools and environment

<p>
  <img src="https://skillicons.dev/icons?i=linux,git,github,vscode,docker,pytorch&theme=dark" alt="Tools and environment" height="48"><img src="https://raw.githubusercontent.com/zenovangue/zenovangue/main/assets/claude.svg" alt="Claude" height="48">
</p>

### Backend and databases

<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi,postgres,mysql,mongodb,redis,sqlite,nginx&theme=dark" alt="Backend and databases">

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

### Strategy engineering: from visual idea to algorithm

- Translate a discretionary, visual strategy (chart patterns, structure, price action) into explicit, deterministic rules that a machine can execute
- Define every concept numerically: swing detection, market structure, zones, entries, stop placement, take-profit logic and invalidation conditions
- Build entry, regime and volatility filters that decide when a strategy should trade and when it should stay out
- Design adaptive indicators that adjust to market conditions: volatility-scaled lengths, regime-aware thresholds, Kalman-based smoothing, HMM/HSMM state routing
- Keep the same logic across platforms so that results on TradingView, MT5 and cTrader can be compared like for like
- Validate before deploying: walk-forward testing, CPCV, Monte Carlo and parameter-stability checks to avoid curve fitting
- Document each rule set with acceptance criteria so the algorithm can be audited and extended later

### Trading platform development

- **TradingView, Pine Script v6:** indicators, strategies and libraries, including adaptive indicators, multi-timeframe logic and alert-ready signals
- **MetaTrader 5, MQL5:** expert advisors, custom indicators and multi-timeframe confluence systems
- **cTrader, C# (cAlgo):** cBots and indicators, including MQL5-to-cAlgo conversions
- **NinjaTrader:** strategies in C#
- Shared risk logic and position sizing across MT5, cTrader, NinjaTrader and TradingView
- Backtesting and research platforms (Go, Python, Parquet) with proxy-aware data downloaders

### Custom trading platforms and tooling

- **Research platforms:** data ingestion, backtesting, walk-forward and Monte Carlo analysis, overfitting detection, reproducible experiment pipelines
- **Execution platforms:** order routing and trade management over the **FIX protocol** and broker APIs, with risk limits and kill-switch logic
- **CLI platforms:** fast command-line tools for data download, backtests, optimization runs and deployment
- **GUI platforms:** desktop applications (Tauri, PySide6) and web dashboards for monitoring, research and manual control
- Clean separation between data, strategy, risk and execution layers so each part can be tested and replaced independently

### Full-stack web development

- Complete websites from design to deployment: frontend, backend and database
- Frontend: semantic HTML, modern CSS, TypeScript, React, responsive and accessible layouts
- Backend: REST APIs, authentication, validation, background jobs, WebSocket and real-time data feeds
- Databases: relational schema design (PostgreSQL, MySQL, SQLite), document stores, caching with Redis
- Security and encryption: HTTPS/TLS everywhere, password hashing, secure session and token handling, role-based access control, encrypted storage of secrets and API keys, input validation and protection against common web attacks
- Complete web applications and full websites, delivered end to end from database schema to deployed frontend
- Data-heavy dashboards for trading and research, with live charts and tables
- Cinematic landing pages: scroll-driven animation, 3D, looping video heroes

### Desktop development

- Desktop applications with Tauri 2, Rust and Svelte
- PySide6 trading workstations
- Native-feeling UIs over local data pipelines and trading APIs

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

**Open to:** converting trading strategies into algorithms and indicators (Pine Script v6, MQL5, cAlgo C#), trading-system builds, FIX and execution platforms, Rust engineering, quant infrastructure, secure full-stack websites and web applications.

---

## GitHub Stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=zenovangue&show_icons=true&bg_color=000000&title_color=e5e5e5&text_color=e5e5e5&icon_color=a1a1aa&border_color=27272a" alt="GitHub stats">
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=zenovangue&layout=compact&bg_color=000000&title_color=e5e5e5&text_color=e5e5e5&border_color=27272a" alt="Top languages">
</p>

---

## Contact

| | |
| :--- | :--- |
| **Email** | [contact@zenovangue.com](mailto:contact@zenovangue.com) |
| **Discord** | `zenovangue` |
| **GitHub** | [@zenovangue](https://github.com/zenovangue) |
| **Hours** | CET / CEST |
