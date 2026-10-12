### Yeluru Nitish

Full-stack + GenAI engineer. I ship LLM systems that run in production, and the tooling that keeps them honest. Currently building PatchBay. Chennai, India.

Experience:
- Founding Engineer at a GenAI startup (stealth, NDA). 2023 – Present. Building production LLM and agent systems end-to-end: React and Next.js frontends, FastAPI/Python backends, RAG and eval pipelines.
- AI Evaluation & RL at Alignerr. May 2026 – August 2026.

Education:
- Baba Institute of Technology & Sciences, B.Tech Computer Science. 2021 – 2025.

Open Source Contributions & Merged Pull Requests:

> **Total Merged Pull Requests: 5** across frontier AI tooling, browser agents, and developer infrastructure.

- <img src="https://github.com/unslothai.png" width="20" height="20" align="center"> [unslothai/unsloth#11634](https://github.com/unslothai/unsloth/pull/11634) : On Windows, binding `127.0.0.1:8888` succeeds even while another process owns `0.0.0.0:8888`; `_is_port_free` only ran its connect probe for wildcard hosts, so Studio silently stole localhost traffic from the other app. Extended the connect probe to loopback hosts so the port correctly falls back to 8889. (Oct 11, 2026)
- <img src="https://github.com/reflex-dev.png" width="20" height="20" align="center"> [reflex-dev/reflex#7275](https://github.com/reflex-dev/reflex/pull/7275) : On a bare `reflex` install, `reflex db init` dumped a raw traceback when the `db` extra was missing. The db commands now point at the extra with a clean error instead. (Sep 30, 2026)
- <img src="https://github.com/magnitudedev.png" width="20" height="20" align="center"> [magnitudedev/magnitude#125](https://github.com/magnitudedev/magnitude/pull/125) : The API-key gate compared request paths case-sensitively while the router matched case-insensitively - `GET /INFERENCE/v1/models` from another device, no key, returned 200 from the inference proxy. Normalized the path before the gate. (Sep 24, 2026)
- <img src="https://github.com/magnitudedev.png" width="20" height="20" align="center"> [magnitudedev/magnitude#120](https://github.com/magnitudedev/magnitude/pull/120) : Some macOS systems briefly report available memory above physical capacity, which Magnitude treated as fatal and blocked ad-hoc model loading. Clamps reported available memory to physical capacity while keeping a zero reading invalid. (Sep 23, 2026)
- <img src="https://github.com/go-gitea.png" width="20" height="20" align="center"> [go-gitea/gitea#39155](https://github.com/go-gitea/gitea/pull/39155) : The web editor commit form showed a bare "cannot commit to branch" with no reason. `PrepareCommitFormOptions` now builds `DenyCommitToBranchReason` on the backend and the template renders it. (Aug 28, 2026)

Open under review: <img src="https://github.com/paradedb.png" width="20" height="20" align="center"> [paradedb/paradedb#6447](https://github.com/paradedb/paradedb/pull/6447), <img src="https://github.com/insforge.png" width="20" height="20" align="center"> [insforge/insforge#2115](https://github.com/insforge/insforge/pull/2115).

What I'm Building:

Agent Infrastructure:
- [PatchBay](https://github.com/PatchBay-HQ/patchbay-demo-payments) : A GitHub App that catches breaking third-party API changes before production does. The demo repo runs the full loop end-to-end on Stripe's 2026-06-30 change: detects `source:` usage inside `charges.create(...)`, reproduces the break with a 15-test Jest suite against an in-memory Stripe fake (deterministic, no network or real key), patches `source` -> `payment_method`, re-verifies green, and opens the PR with the evidence. Offline prototype; production version in progress.
- [cookbook-canary](https://github.com/Nitish-1303/cookbook-canary) : Proves every example in a repo still runs - each one alone on its own hardware-isolated Solari microVM, with a cloud browser checking what actually rendered and Linux desktops for the examples that need pixels. CI-gated, live report dashboard.
- [flake-hunter](https://github.com/Nitish-1303/flake-hunter) : Finds flaky tests, proves the root cause, opens the fix PR. Reruns the suite across a 50-sandbox fan-out so flakiness is measured, not rerun-away. Nebius x NVIDIA Global AI Hackathon entry (Coding & Agentic Engineering track).

Applied AI:
- [Debrief](https://github.com/Nitish-1303/Debrief) : Meetings in, tasks out. Extracts every commitment from a transcript with owner and date, then a second verifier pass checks each task's quote exists verbatim and actually supports it, attaching a 0-100 confidence score; failures are flagged unverified. Live at [debrief-bay.vercel.app](https://debrief-bay.vercel.app).
- [Lumina](https://github.com/Nitish-1303/lumina-OS) : iMessage-native life OS - morning briefings, goal accountability, decision support over chat. Concept build: landing page plus an in-browser simulator running the real Gemini agent loop (React, TypeScript, Vite).
- [Migma x Spotify](https://github.com/Nitish-1303/Migma) : Music-campaign automator concept for Migma's plugin platform - turns any listening surface (playlist, track, roster) into an email campaign on their generate-and-poll pipeline. Runs against the real Spotify API with one honest mock; live storyboard at [migma-wireframe.vercel.app](https://migma-wireframe.vercel.app/).

Crypto / Payments:
- [CipherBill](https://github.com/Nitish-1303/CipherBill) : Privacy-first invoicing and settlement on Starknet mainnet - STRK20 shielded balances and private transfers with a selective-disclosure path for accounting. Wallet adapter, guarded connection, shield and private-transfer UI implemented; verified pool config, receipts and evidence still pending, and the README says so. Built for the STRK20 Private Sprint.

Technical Focus:
<p align="left">
  <img src="https://skillicons.dev/icons?i=ts,react,nextjs,nodejs,py,fastapi,postgres,docker,aws,vercel&perline=10" alt="TypeScript, React, Next.js, Node.js, Python, FastAPI, PostgreSQL, Docker, AWS, Vercel" />
</p>

- LLM APIs, RAG, agent tooling, eval pipelines

Contact:
- Email: yelurunitish006@gmail.com
- Portfolio: [yeluru-nitish.vercel.app](https://yeluru-nitish.vercel.app/)
- LinkedIn: [yeluru-nitish](https://www.linkedin.com/in/yeluru-nitish/)
- GitHub: [Nitish-1303](https://github.com/Nitish-1303)
