<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,100:1f6feb&height=200&section=header&text=Zeno%20Vangue&fontColor=ffffff&fontSize=52&fontAlignY=38&desc=Systems%20%7C%20Quant%20Infrastructure%20%7C%20Web%20%7C%20Prompt%20Engineering&descAlignY=60&descSize=16" alt="Zeno Vangue banner" width="100%">
</p>

<h2 align="center">Principal Systems Architect & Quantitative Infrastructure Engineer</h2>

<p align="center">
  <em>"Sovereign systems. Low-latency execution logic. Forging nanosecond infrastructure at the absolute intersection of 19th-century statistical rigor and predictive hardware computing."</em>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Rust-Stable_Core-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust Core">
  <img src="https://img.shields.io/badge/Kernel-Bypass-0d1117?style=for-the-badge&logo=linux&logoColor=white" alt="Kernel Bypass">
  <img src="https://img.shields.io/badge/Process-Isolation-1f6feb?style=for-the-badge&logo=gnometerminal&logoColor=white" alt="Process Isolation">
  <img src="https://img.shields.io/badge/Prompt-Engineering-8957e5?style=for-the-badge&logo=openai&logoColor=white" alt="Prompt Engineering">
</p>

---

## 👤 About Me

I am an independent engineer and algorithmic trader based in Morocco. I design and build trading infrastructure end to end: quantitative research, low-latency execution engines, backtesting platforms, and the web interfaces that sit on top of them.

My work combines three disciplines:

- **Systems engineering:** Rust-first, memory-aware, latency-obsessed.
- **Quantitative research:** regime detection, state-space models, and rigorous validation.
- **Product and web:** fast, cinematic, production-grade interfaces.
- **AI-assisted engineering:** structured prompt design for building complex software with LLMs.

---

## 🛠️ Core Infrastructure Stack

| Architecture Layer | Technologies & Frameworks |
| :--- | :--- |
| **⚡ Low-Latency & Memory** | `Rust` (Stable Core) • `Kernel-Bypass (SPDK/DMA)` • `Zero-Copy FlatBuffers` • `memmap2` • `mlock` |
| **🧠 Deep Learning & Statistics** | Pure Rust `Burn` Framework • Expectation-Maximization `GMM` • Dynamic Duration `HSMM` • `HMM` • `Kalman Filter` |
| **🚀 Hardware Optimization** | Distributed `wgpu` Compute Shaders • Parallel `Walk-Forward Optimization (WFO)` • `CPCV` |
| **📈 Trading Platforms** | `MetaTrader 5 (MQL5)` • `NinjaTrader` • `cTrader (cAlgo C#)` • `TradingView (Pine Script)` |

---

## 🦀 Rust & Systems Skills

- Lock-free data structures and shared-memory IPC ring buffers
- Zero-copy serialization (FlatBuffers) and memory-mapped data pipelines
- Cache-aware data layout (L1/L2/L3), `mlock`, CPU pinning and process isolation
- From-scratch statistical models in Rust (Gaussian HMM, Kalman, ATR, risk sizing)
- Multi-language runtime integration: `Rust` • `Python` • `C# AOT` • `Go`
- Workspace architecture: multi-crate Cargo projects with clean module boundaries

<p>
  <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img src="https://img.shields.io/badge/Tauri-24C8DB?style=flat-square&logo=tauri&logoColor=white">
</p>

---

## 🌐 Web Development Skills

- Cinematic landing pages: scroll-driven animation, 3D, looping video heroes
- Component-based UIs with `React` and `TypeScript`
- Desktop apps with `Tauri 2` + `Svelte`
- Performance-first front end: semantic HTML, modern CSS, responsive and accessible layouts
- Trading dashboards and data-heavy interfaces

<p>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img src="https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB">
  <img src="https://img.shields.io/badge/Svelte-FF3E00?style=flat-square&logo=svelte&logoColor=white">
  <img src="https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white">
</p>

---

## 🧠 Prompt Engineering

I write production-grade "master prompts" that let AI coding assistants build complete, correct software on the first pass.

- **Phased specifications:** architecture, then modules, then validation, with clear acceptance criteria per phase
- **Constraint-driven prompts:** explicit stack, file layout, performance targets and failure modes
- **Single-file and multi-file delivery:** generator scripts that produce full project trees
- **Debug prompts:** root-cause investigation prompts for ML and quant pipelines
- **Review loops:** iterating prompts against real output until the result is deterministic

---

## 💻 Flagship Node: `Aethelgard NANO-GRID`

A pure-Rust, high-throughput execution framework designed to bypass traditional Linux kernel scheduling constraints and communicate directly with hardware.

- **Data Ingestion Matrix:** async Dukascopy byte extraction combined with optimized binary storage, streaming hundreds of millions of ticks mapped to CPU cache blocks.
- **Process Isolation Sandbox:** multi-core process sandboxing with lock-free shared-memory IPC ring buffers, integrating `Rust`, `Python` and `C# AOT` strategies.

## 🔬 Other Projects

- **Aegis Engine:** Go + Python/Numba/Polars/Parquet backtesting platform with a Dukascopy downloader
- **Regime-Switching Systems:** HMM/HSMM regime detection routing to trend-following or mean-reversion logic
- **XAU Glass:** Tauri 2 + Rust + Svelte research and paper-trading desktop app for XAUUSD
- **Multi-Platform EAs:** MQL5, cAlgo and NinjaTrader strategies with consistent risk management

---

## 📊 System Telemetry

```rust
// Current Operational Status: ONLINE
pub struct SystemMetrics {
    pub latency: Nanoseconds,
    pub throughput: TicksPerSecond,
    pub isolation_layer: Sandbox,
    pub engine_status: Execution,
}

pub const METRICS: SystemMetrics = SystemMetrics {
    latency: Nanoseconds(50),
    throughput: TicksPerSecond(300_000_000),
    isolation_layer: Sandbox::KernelBypass,
    engine_status: Execution::Sovereign,
};
```

---

## 📫 Contact

- GitHub: [@zenovangue](https://github.com/zenovangue)
- Email: your-email@example.com
- Location: Morocco 🇲🇦

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=zenovangue&style=flat-square&color=1f6feb&label=PROFILE+VIEWS" alt="Profile views">
</p>
