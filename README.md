# Aayush Baniya

CS + Math @ UT Austin. Software Engineer at [DeepInvent](https://deepinvent.ai) — building agents that reproduce ML papers from an arXiv ID.

[aayushswebsite.vercel.app](https://aayushswebsite.vercel.app/) · [X](https://x.com/aayushcb) · [LinkedIn](https://www.linkedin.com/in/aayush-baniya-a30551223) · thisisaayushbaniya@gmail.com

---

### Selected work

**[DeepInvent](https://deepinvent.ai)** · Python · Multi-cloud GPU · Agent orchestration
Software Engineer, May 2026 – present. I build the agent core: give it an arXiv ID and it reproduces the paper end to end. 19 model-callable primitives, the paper held as a REPL variable the model never sees in its context, and a result only passes when the measured on-disk evidence backs it — the model's own grade doesn't count. I also built the multi-cloud GPU layer: one sandbox over local, Docker, GCP, and Azure/AKS, with a scheduler that pins each job to a single GPU, drops the batch size on CUDA OOM, and fails a job over from GCP to Azure when GCP runs out of capacity.

**[Open Applier](https://aayushswebsite.vercel.app/archive/openapplier)** · Rust + Next.js · Postgres · Redis · Stripe · Chrome extension · *retired*
Job applications you still approved, minus the typing. Rust/Axum core with tenant-scoped Postgres RLS, idempotent Stripe billing, and an LLM tailoring pipeline with real cost rails (kill switch, per-call ceilings, daily caps); LaTeX rendered through Tectonic; a Chrome extension filled and submitted on the employer's own site. Reached 500+ users, 5,000+ applications, and 95% submission success across 8+ ATS (Workday, Greenhouse, Lever, Ashby) before I wound it down. Built with Abheek Pradhan — I owned the Rust core, LLM pipeline, ATS integrations, LaTeX renderer, and frontend.

**[aImsg](https://aayushswebsite.vercel.app/archive/aimsg)** · TypeScript · Next.js · *retired*
A messaging layer for coding agents — you texted a GitHub repo over iMessage and it answered: questions about the code, PR reviews, edits shipped from your phone, multi-provider with failover. Built in 2025, before Apple sanctioned any third-party AI agent inside iMessage (that arrived March 2026). It never scaled: iMessage has no official API, so the only routes are fragile Mac relays or reverse-engineering the protocol — and Apple shuts those down.

**MyFutureSelf** · Swift · SwiftUI · StoreKit
iOS engineering intern, Jul – Oct 2025. One of two engineers taking the app from zero to 5,000+ users and 500+ App Store reviews at 4.7★. Owned the SwiftUI launch flows and Firebase sync, and built three StoreKit 2 subscription tiers with server-side receipt validation.

**[OnionUSDp](https://github.com/AayushBaniya2006/OnionUSDp)** · Solana · Token-2022
Confidential payroll on Solana's Token-2022 confidential-transfer extension. Bulk processing, USDC-backed pUSD stablecoin, revocable corporate transfer window. 1st place at OnionDAO ($3K).

**[TST Mechanistic Interpretability](https://github.com/AayushBaniya2006/TST-Mechanistic-Interpretability)** · PyTorch
Activation patching on a 96-class Time Series Transformer. 10,000-resample bootstrap CIs + Benjamini–Hochberg FDR + Cohen's d. Finding: most heads flagged "important" by naive patching don't survive proper statistical controls — rankings hold on simple tasks (Kendall tau 0.88) and fall apart on complex ones (0.48). Through BlueDot AISF, Jan – Feb 2026. [Write-up](https://thisisaayushbaniya.substack.com/p/most-important-attention-heads-in).

**[ldos_manip_tracing](https://github.com/AayushBaniya2006/ldos_manip_tracing)** · ROS 2 · C++ · LTTng · CloudLab
Tracing-driven analysis of a ROS 2 manipulation stack under DDS flood. DDS middleware is the primary low-rate DoS surface: 4,000 msg/s drove MoveIt on a simulated 7-DOF Panda to 100% execution failure, while replaying the same load under cgroups v2 on 32-core CloudLab nodes ruled CPU out. UT Learning-Directed OS Lab, Dec 2024 – May 2026.

---

### Hackathon wins

- **OnionDAO** — 1st place, $3K (OnionUSDp)
- **Nepali Leaders of America** — 1st place, $1.5K (VoiceCanvas)
- **Antler × Codex** — 2nd place, $2K in DeepInvent credits (ReproLab)
- **LaunchD** — 2nd place, $500 + residency interview (Agent Graph, with Armaan Amatya & Abheek Pradhan)
- **Akash Network** — 3rd place, $500 (Change-Aware Auditor)

---

### Experience

- **Software Engineer**, DeepInvent — May 2026 – present. Agent core for reproducing ML papers from an arXiv ID (19 model-callable primitives, evidence-gated results); multi-cloud GPU layer over local / Docker / GCP / Azure-AKS with an OOM-aware, GCP → Azure failover scheduler.
- **iOS Engineering Intern**, MyFutureSelf — Jul – Oct 2025. Three StoreKit 2 subscription tiers with server-side receipt validation and 20+ SwiftUI onboarding flows; app reached 5K+ users at 4.7★.
- **Undergraduate Researcher**, UT Austin Learning-Directed OS Lab — Dec 2024 – May 2026. ROS 2 tracing on 32-core CloudLab nodes; found DDS saturation, not CPU, to be the dominant low-rate DoS surface.
- **Independent Researcher**, BlueDot Impact AISF — Jan – Feb 2026. Bootstrap CIs + Benjamini–Hochberg FDR + Cohen's d to separate real attention-head effects from statistical noise on a Time Series Transformer. [Write-up](https://thisisaayushbaniya.substack.com/p/most-important-attention-heads-in).

---

### Tech skills

**Languages** — Rust · Python · TypeScript · JavaScript · Swift · Java · C · SQL · Bash

**Frameworks** — React · Next.js · Node.js · FastAPI · Axum · SwiftUI · gRPC · LangChain · PyTorch

**Infra & data** — PostgreSQL · pgvector · Redis · MongoDB · Docker · Kubernetes · AWS · GCP · Azure/AKS · Railway · Stripe · Tectonic · ROS 2 · LTTng · CloudLab

**Testing & tools** — pytest · Jest · Playwright · OpenTelemetry · Linux · Git

**Blockchain** — Solana (Token-2022, Blinks, Anchor)

---

Also: contributed reproduction entries to OpenAI's [parameter-golf](https://github.com/openai/parameter-golf) (the "smallest-LM-in-16MB" challenge — best val_bpb 1.06).

Interested in AI infrastructure, agent systems, applied interpretability, and dev tools for things that aren't text generation.
