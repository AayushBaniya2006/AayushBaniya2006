# Aayush Baniya

CS + Math @ UT Austin (University Honors). Software Engineer at [DeepInvent](https://deepinvent.ai) — building agents that reproduce ML papers from an arXiv ID. Founder of [Open Applier](https://www.openapplier.com).

[aayushswebsite.vercel.app](https://aayushswebsite.vercel.app/) · [X](https://x.com/aayushcb) · [LinkedIn](https://www.linkedin.com/in/aayush-baniya-a30551223) · thisisaayushbaniya@gmail.com

---

### Selected work

**[DeepInvent](https://deepinvent.ai)** · Python · Multi-cloud GPU · Agent orchestration
Software Engineer, May 2026 – present. I build the agent core of a system that reproduces ML papers from an arXiv ID — 19 LLM-callable primitives, with the paper offloaded as a REPL variable the model never sees in-context, and verdicts gated on measured on-disk evidence rather than the model's own grade. I also built the multi-cloud GPU layer: a unified sandbox over local, Docker, GCP, and Azure/AKS with a scheduler that pins each job to one GPU, shrinks batch size on CUDA OOM, and fails over GCP → Azure on capacity stockout.

**[Open Applier](https://www.openapplier.com)** · Rust + Next.js · Postgres · Redis · Stripe · Chrome extension
Live SaaS for AI job applications — 500+ signups, private beta, $5/mo Pro. Rust core with tenant-scoped Postgres RLS, idempotent Stripe billing, LLM tailoring pipeline with per-feature cost rails (kill switch, per-call ceilings, daily caps), Vertex AI context caching, LaTeX rendering via Tectonic, browser-side form submission across Workday / Greenhouse / Lever / Ashby. Building with Abheek Pradhan — I own the Rust core, LLM pipeline, ATS integrations, LaTeX renderer, and frontend.

**Agent Survivor** · Python · Postgres · Railway
A public competition where autonomous AI founders each get a small real bankroll and 21 days to build the strongest lawful business they can — no human steering after kickoff. I built the control plane: budget-isolated contestants, a public ledger, an evidence/receipt system, and autonomous confessional triggers.

**[aImsg](https://aimsg.dev)** · TypeScript · Stripe
GitHub from iMessage — review PRs, query code, ship edits from your phone. Multi-provider LLM (Claude / GPT / Gemini) with BYOK and automatic failover. Stripe-billed tiers, live at aimsg.dev.

**[BlinkFund](https://blinkfund.vercel.app)** · TypeScript · Solana
Crowdfunding on Solana Blinks — shareable donation cards that build and fee-split transactions right inside a tweet.

**[Watchtower CLI](https://github.com/Watchtower-Labs/watchtower-cli)** · TypeScript · React · Ink
Terminal observability for Google ADK agents. Constant-time trace rendering for concurrent LLM streams via NDJSON replay and live tailing. Published on npm and PyPI.

**MyFutureSelf** · Swift, SwiftUI, StoreKit
iOS engineering intern, Jul – Oct 2025. Shipped a 3-tier StoreKit paywall with server-side receipt validation and feature-gated access, plus 20+ gesture-driven SwiftUI onboarding flows. App reached 5K+ users and 4.7★ across 500+ App Store reviews.

**[OnionUSDp](https://github.com/AayushBaniya2006/OnionUSDp)** · Solana, Token-2022
Confidential payroll on Solana's Token-2022 confidential transfer extension. Bulk processing, USDC-backed pUSD stablecoin, revocable corporate transfer window. 1st place at OnionDAO ($3K).

**[TST Mechanistic Interpretability](https://github.com/AayushBaniya2006/TST-Mechanistic-Interpretability)** · PyTorch
Activation patching on a 3-layer / 8-head Time Series Transformer. Bootstrap resampling (10K iters) + Benjamini–Hochberg FDR + Cohen's d. Finding: most heads flagged "important" by naive patching don't survive proper statistical controls — stable on simple tasks (p = 0.88–0.89), collapses on complex ones (p = 0.48). Through BlueDot AISF, Jan – Feb 2026.

**[ldos_manip_tracing](https://github.com/AayushBaniya2006/ldos_manip_tracing)** · ROS 2, C++, LTTng, CloudLab
Tracing-driven performance analysis of ROS 2 manipulation under DDS flood. Identified DDS middleware as the primary low-rate DoS surface — 100% MoveIt execution failure at 4000 msg/s on a 32-core EPYC node, while CPU load alone caused no degradation. UT Learning-Directed OS Lab, ongoing since Dec 2024.

---

### Hackathon wins

- **OnionDAO** — $3K, 1st place (OnionUSDp)
- **Nepali Leaders of America** — $1.5K, 1st place
- **Antler × Codex** — $2K in DeepInvent credits (ReproLab)
- **LaunchD** — $500 + residency interview (Agent Graph, with Armaan Amatya & Abheek Pradhan)
- **Akash Network** — $500

---

### Experience

- **Software Engineer**, DeepInvent — May 2026 – present. Agent core for autonomous ML-paper reproduction (19 LLM-callable primitives, evidence-gated verdicts); multi-cloud GPU layer over local / Docker / GCP / Azure-AKS with an OOM-aware, GCP → Azure failover scheduler.
- **Security Analyst Intern**, UT Austin RSOC — Jun 2025 – present. Windows/Linux internals, Active Directory, enumeration, web exploitation labs.
- **iOS Engineering Intern**, MyFutureSelf — Jul – Oct 2025. 3-tier StoreKit paywall + 20+ SwiftUI onboarding flows; app reached 5K+ users at 4.7★.
- **Undergraduate Researcher**, UT Austin Learning-Directed OS Lab — Dec 2024 – present. ROS 2 tracing on CloudLab (32-core EPYC); DDS as the dominant LDoS surface.
- **Independent Researcher**, BlueDot Impact AISF — Jan – Feb 2026. Statistical pipeline (bootstrap + FDR + Cohen's d) for activation patching on a Time Series Transformer.

---

### Tech skills

**Languages** — Rust · Python · TypeScript · JavaScript · Swift · Java · C++ · Go · Solidity · SQL · Dart

**Frameworks** — React · Next.js · Node.js · SwiftUI · Flutter · Tailwind · PyTorch · LangChain · Anchor

**Infra & tools** — PostgreSQL (RLS, PgBouncer) · Redis · Docker · Kubernetes · AWS · GCP · Azure/AKS · Railway · Stripe · StoreKit 2 · Tectonic · ROS 2 · LTTng · FlameGraph · CloudLab · PostHog · Sentry · k6

**AI / ML** — NumPy · Pandas · scikit-learn · SciPy · Hugging Face · OpenAI / Anthropic / Gemini SDKs · Vertex AI (context caching)

**Blockchain** — Solana (Token-2022, Blinks, Anchor) · Ethereum · Web3.js

---

Also: contributed reproduction entries to OpenAI's [parameter-golf](https://github.com/openai/parameter-golf) (the "smallest-LM-in-16MB" challenge — best val_bpb 1.06).

Interested in: AI infrastructure, agent systems, applied interpretability, and dev tools for things that aren't text generation.
