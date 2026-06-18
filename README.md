<p align="center">
  <img src="/assets/klokworkai-wordmark-clock.png" height="200"/>
</p>

# klökwork AI

Independent platform engineering initiative building AI-native orchestration systems, inspectable developer workflows, and infrastructure automation for ICs and cloud platforms.

The focus is not autonomous engineering — it's making AI-assisted workflows observable, collaborative, and operationally grounded before implementation decisions are accepted.

---

## Projects

### [koll♠b](https://github.com/klokworkai/kollab) — ACE · Adversarial Collab Engine · OSS

An AI-native orchestration system that runs two agents through a structured proposal → critique → revision → convergence workflow on a shared engineering objective. Every turn, verdict, and reasoning trace is streamed live to a browser UI. The session is fully interruptible: halt at any point, inject a directive into one or both agents, and resume.

Built for ICs who already use multiple AI models to cross-validate their work — bouncing between Claude, Codex, GPT, or Gemini to catch what one model misses. koll♠b replaces that manual tab-switching with a structured loop: one model proposes, another adversarially reviews, and ACE enforces the back-and-forth until the proposal holds up or the disagreement is explicit. Less trial and error. No lost context. Full audit trail.

<p align="center">
  <img src="/assets/ace-loop.png" width="760" alt="ACE convergence loop — kollab orchestration"/>
</p>

Currently ships with Claude Code as producer and Codex as critic. The current two-agent model will become extensible with a pluggable provider registry — Anthropic, OpenAI, DeepSeek, Groq, Gemini — with configurable roles (architect, reviewer, coder, tester, security, custom roles) and user-defined multi-stage workflows. The validation loop stays the same; what changes is what runs inside it.

Observability is structural, not opt-in. Turn IDs are stable for the session lifetime. Verdict parsing is mechanical — ACE reads a `<verdict>` trailer on every turn and acts on it. Interrupted turns are preserved as artifacts. Every event is typed, logged to JSONL, and replayable from disk. The result isn't just AI output — it's a validated proposal with an auditable provenance trail. [Roadmapped for API workflow as well]

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

**John Manoah Jeyakumar** - IC in Platform and Infrastructure Engineering with 18+ years across various Software Engineering roles. 10+ years in cloud platforms, Kubernetes, and distributed systems. Masters in Cloud Computing, 7× AWS certified, 4× GCP certified and others.

[Personal LinkedIn](https://www.linkedin.com/in/john-jeyakumar) · [X / @klokworkai](https://x.com/klokworkai) · [john@klokwork.ai](mailto:john@klokwork.ai)

---

*Select projects will be open-sourced. kollab is the first.*
