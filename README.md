<p align="center">
  <img src="/assets/klokworkai-logo-large.png" height="200"/>
</p>

# klökwork AI

Independent platform engineering initiative building AI-native orchestration systems, inspectable developer workflows, and infrastructure automation for cloud and Kubernetes environments.

The focus is not autonomous engineering — it's making AI-assisted workflows observable, collaborative, and operationally grounded before implementation decisions are accepted.

---

## Projects

### [koll♠b](https://github.com/klokworkai/kollab) — ACE · Adversarial Collab Engine

An AI-native orchestration system that runs two independent coding agents — Claude Code (producer) and Codex (critic) — through a structured proposal, critique, revision, and convergence workflow on a shared engineering objective. Every turn, verdict, and reasoning trace is streamed live to a browser UI. The session is fully interruptible: halt at any point, inject a directive into one or both agents, and resume.

<p align="center">
  <img src="/assets/ace-loop.png" width="760" alt="ACE convergence loop — kollab orchestration"/>
</p>

Observability is structural, not opt-in. Turn IDs are stable for the session lifetime. Verdict parsing is mechanical — ACE reads a `<verdict>` trailer on every turn and acts on it. Interrupted turns are preserved as artifacts. Every event is typed, logged to JSONL, and replayable from disk.

**[→ kollab repo](https://github.com/klokworkai/kollab)** · `demoable`

---

### [kre8](https://github.com/klokworkai/kre8) — Thinking Infra Engine

Intent-driven infrastructure planning system. Translates natural-language objectives into policy-validated architecture decisions and inspectable design artifacts before any HCL or IaC is generated. The design artifact is the deliverable — not the Terraform.

**[→ kre8 repo](https://github.com/klokworkai/kre8)** · `design stage`

---

### [kyoo](https://github.com/klokworkai/kyoo) — from Intent to Go

AI-native Kubernetes operator synthesis. Natural-language intent in, production-ready Go controller out — with the operator design surfaced as an inspectable artifact before code generation begins.

**[→ kyoo repo](https://github.com/klokworkai/kyoo)** · `concept stage`

---

## What ties these together

Each project is built around the same premise: AI-assisted engineering workflows should surface their reasoning as an explicit, inspectable artifact before output is accepted. Not as an opt-in log — as the contract.

- **koll♠b** makes inter-model reasoning observable in real time
- **kre8** makes infrastructure intent inspectable before IaC is written
- **kyoo** makes operator design inspectable before Go is generated

---

## Built by

**John Manoah Jeyakumar** — platform and infrastructure engineer with 18+ years across cloud platforms, Kubernetes, and distributed systems. 7× AWS certified, 4× GCP certified. Founding engineer, Klokwork AI.

[LinkedIn](https://www.linkedin.com/in/john-jeyakumar) · [Klokwork AI on LinkedIn](https://www.linkedin.com/company/klokwork-ai) · [X / @klokworkai](https://x.com/klokworkai) · [john@klokwork.ai](mailto:john@klokwork.ai)

---

*Select components will be open-sourced. kollab is the first.*
