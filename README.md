<p align="center">
  <picture>
    <source media="(max-width: 600px)" srcset="./assets/banner-mobile.svg">
    <img src="./assets/banner-desktop.svg" alt="Mohammed Samaruddin Ahmed — evidence-first AI systems" width="100%">
  </picture>
</p>

<p align="center">
  <a href="https://github.com/MrSamarAhmed">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3500&pause=900&color=38BDF8&center=true&vCenter=true&width=650&lines=Systems+that+show+their+work.;Evidence-first+AI+%C2%B7+Python+%C2%B7+FastAPI;Verification+before+resolution.;Learning+Go+%C2%B7+cloud-native+curious;GSoC+2027+%C2%B7+LFX+Mentorship+aspirant" alt="Systems that show their work — evidence-first AI, verification before resolution, learning Go, GSoC 2027 and LFX Mentorship aspirant">
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=MrSamarAhmed&style=flat-square&color=1D4ED8&label=profile+views" alt="Profile views">
  <img src="https://img.shields.io/badge/focus-evidence--first_AI-38BDF8?style=flat-square&labelColor=04070F" alt="Focus: evidence-first AI">
  <img src="https://img.shields.io/badge/open_to-GSoC_2027_%C2%B7_LFX_2027-6366F1?style=flat-square&labelColor=04070F" alt="Open to GSoC 2027 and LFX Mentorship 2027">
</p>

## Systems that show their work

I'm Mohammed Samaruddin Ahmed, a Mechanical Engineering undergrad who builds AI systems that have to prove themselves: research agents with inspectable sources, debugging workflows that stop for human approval, and reliability tooling whose success is decided by a verifier rather than a confident sentence.

Most of my projects share one shape: **a probabilistic model can propose, but deterministic code decides what counts as done.**

- **Evidence over assertion.** Citations are checked against retrieved sources; fixes are recorded against real test runs.
- **Verification before resolution.** A recovery or a fix is not finished until a separate verifier confirms it.
- **Honest failure.** Missing credentials, unproven fixes, and unavailable providers are reported, not papered over.

**Currently**

- 🌱 Learning **Go** from the ground up — fundamentals first, no proficiency claims yet.
- ☁️ Reading cloud-native codebases (starting with **Meshery**) to prepare for open-source contribution.
- 🎯 Working toward **GSoC 2027**, with LFX Mentorship 2027 as a parallel track.

<img src="./assets/divider.svg" width="100%" alt="">

## Selected work

### 01 · ORBIT Machine Guardian

*Autonomous reliability for rotating machinery, in simulation. Built for the AMD Developer Hackathon ACT III.*

A closed-loop agent for a simulated 6205-bearing motor rig: it reads vibration and temperature windows, detects faults, ranks competing hypotheses, plans a precondition-checked intervention, and verifies recovery before closing an incident. Only a deterministic verifier can mark an incident resolved; when recovery cannot be proven, the incident escalates instead.

> **Simulation boundary:** every machine scenario is simulated. ORBIT does not connect to or control real industrial equipment, and the project does not claim AMD GPU or ROCm execution.

**Stack** — Python · FastAPI · Streamlit · PyTorch · NumPy · SciPy · AMD Token Factory

**[View the repository →](https://github.com/MrSamarAhmed/ORBIT-MACHINE-GUARDIAN)**

### 02 · ORBIT Search

*A research workflow that leaves the queries, sources, and citations visible behind the answer.*

It plans several sub-queries, searches the live web through SerpApi, deduplicates the results, and asks Gemini to write an answer from the collected evidence only. When synthesis is rate-limited or unavailable, it returns the sources and a warning instead of inventing an answer; answer URLs that were not in the evidence are flagged. The API exposes each stage's output, and the browser workspace ships with no build step.

**Stack** — Python · FastAPI · SerpApi · Google Gemini · httpx · Vanilla JS · Docker

**[View the repository →](https://github.com/MrSamarAhmed/ORBIT-SEARCH)**

### 03 · MaintAI

*From failure to verified fix, with a human approval gate. Built for the IBM Bob 2.0 Hackathon.*

It drives IBM Bob 2.0 through an investigation protocol: provenance-bearing evidence, competing hypotheses, an adversarial review, and an exact patch proposal. A human decision is bound to the run and file digests; the patch is applied only after approval, and verification is a real `unittest` run executed by the trusted workflow. If Bob is unavailable, the run fails closed.

> **Scope note:** a local demonstration control plane for a deterministic concurrent-inventory bug, not a production security boundary. The README lists its open limitations.

**Stack** — Python · FastAPI · IBM Bob 2.0 · Next.js · React · TypeScript · Tailwind CSS

**[View the repository →](https://github.com/MrSamarAhmed/MaintAI)**

### 04 · Tablekeeper

*Stage 1 of the WeAreDevelopers × BAND Dark Factory — a service built by an agent factory.*

A FastAPI + SQLite table-reservation service produced by a three-agent Architect → Builder → Reviewer pipeline with rejection, revision, and approval cycles. The repository preserves the factory's BAND transcript, build attempts, review records, and the Stage 1 artifact, alongside its Docker setup and contract tests.

> **Scope note:** a Stage 1 hackathon submission. The README documents an unresolved specification conflict and open limitations.

**Stack** — Python · FastAPI · SQLite · Docker · BAND · GitHub Actions

**[View the repository →](https://github.com/MrSamarAhmed/dark-factory-tablekeeper)**

<img src="./assets/divider.svg" width="100%" alt="">

## More work

- **[Second-Opinion](https://github.com/MrSamarAhmed/Second-Opinion)** — Audits Qloo music recommendations for supporting metadata, with re-derivable receipts and a bounded follow-up lookup. Standard-library Python.
- **[ShipProof](https://github.com/MrSamarAhmed/shipproof)** — A browser-only ledger that audits completion claims against linked JUnit evidence, even when every test in the report passes. TypeScript · Vite · Vitest.
- **[StandIn](https://github.com/MrSamarAhmed/standin)** — Local-first, reversible pseudonymization for using AI on confidential documents, running entirely in the browser. React · TypeScript · Transformers.js · ONNX.

<img src="./assets/divider.svg" width="100%" alt="">

## Toolkit

<p align="center">
  <a href="https://github.com/MrSamarAhmed?tab=repositories">
    <img src="https://skillicons.dev/icons?i=python,ts,js,fastapi,docker,sqlite,react,nextjs&perline=8" alt="Python, TypeScript, JavaScript, FastAPI, Docker, SQLite, React, Next.js"><br>
    <img src="https://skillicons.dev/icons?i=tailwind,vite,pytorch,numpy,pytest,git,githubactions&perline=8" alt="Tailwind CSS, Vite, PyTorch, NumPy, pytest, Git, GitHub Actions">
  </a>
</p>

**Languages** — Python · TypeScript · SQL · JavaScript<br>
**Backend & services** — FastAPI · Uvicorn · Streamlit · SQLite · Docker · httpx<br>
**AI & agents** — Google Gemini · SerpApi · IBM Bob 2.0 · BAND · Qloo · AMD Token Factory · Transformers.js<br>
**Data & ML** — PyTorch · NumPy · SciPy · ONNX<br>
**Frontend** — React · Next.js · Tailwind CSS · Vite<br>
**Testing & delivery** — pytest · Vitest · unittest · GitHub Actions · pnpm

<sub>Only tools that appear in the repositories above are listed; this is not a proficiency ranking. Go is deliberately absent — it is in progress, not yet evidenced.</sub>

<img src="./assets/divider.svg" width="100%" alt="">

## GitHub analytics

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=MrSamarAhmed&theme=transparent" alt="GitHub stats" height="165">
  <img src="https://streak-stats.demolab.com?user=MrSamarAhmed&hide_border=true&background=04070F&ring=38BDF8&fire=60A5FA&currStreakLabel=38BDF8&sideLabels=94A3B8&dates=5B6B84&currStreakNum=F8FAFC&sideNums=F8FAFC" alt="Contribution streak" height="165">
</p>

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=MrSamarAhmed&theme=transparent" alt="Top languages by repository">
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=MrSamarAhmed&bg_color=04070F&color=94A3B8&line=38BDF8&point=60A5FA&area=true&hide_border=true&title_color=7DD3FC" alt="Contribution activity graph" width="100%">
</p>

<img src="./assets/divider.svg" width="100%" alt="">

<sub>Every project links to its public repository. Claims are limited to what each repository's README and source code support. ORBIT Machine Guardian operates on simulated machine scenarios only.</sub>