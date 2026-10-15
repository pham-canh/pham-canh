# Phạm Cảnh

**AI agent systems that prove their own work.** I build agents where every claim is
re-derivable from the repo — not screenshots.

I'm a software engineer working on **AI agents, automation, and the verification
around them**. Most agent demos assert that something worked. The pattern I keep
coming back to is making the assertion checkable: an evaluator seat that re-derives
every claim from the artefacts, and a CI gate that fails the build when a claim
and the repo disagree.

- 🔭 **Verifiable agent pipelines** — claim re-derivation, independent evaluation, measurable baselines
- 🛠 **Python-first**, with TypeScript/JS where the interface needs it
- 🧪 **Tested and gated** — tests, CI, and honest fallbacks that report which provider actually answered
- 🌏 Based in Ho Chi Minh City, Vietnam · open to remote

## Tech stack

```
Python  ·  TypeScript / JavaScript  ·  Bash
Node  ·  Docker  ·  GitHub Actions
PostgreSQL  ·  Redis  ·  AWS  ·  OpenTelemetry
LLM providers: NVIDIA Nemotron (Nebius) · Gemini · OpenAI
STT/TTS: AssemblyAI · Edge TTS
```

## Selected work

**[opencode-harness-kit](https://github.com/pham-canh/space-harness)**
Model-agnostic harness kit for coding agents — capability profiles, context
pruning, and **measured baselines** so you can show a change made the model faster
instead of asserting it. MIT licensed, 9 test suites.

**[pocketful-factory](https://github.com/pham-canh/pocketful-factory)**
Three coding-agent seats in one room build a wallet service, with an independent
evaluator that **re-derives every figure from the evidence and fails if a document
disagrees**. All 121 agent messages are in `room.json` — every tool call, every
verdict, including the last one that fixed a wrong-revision error.

**[voicecare-scheduler](https://github.com/pham-canh/voicecare-scheduler)**
Voice booking for elderly clinic patients — speak to book, nothing is booked
without a spoken confirmation. NLU on NVIDIA Nemotron via Nebius Token Factory,
with the active provider reported in the UI. 28 tests, a one-command demo
recorder, and a latency claim that matches what the app actually prints.

**[failed-strategies](https://github.com/pham-canh/failed-strategies)**
Backtested trading strategies that lost money, kept with post-mortems. Published
on purpose — knowing why an approach failed is more useful than hiding it.

## What I care about

Claim it, then make it checkable. A fallback that silently downgrades the system
is worse than a loud failure, and a README number that the app contradicts is a
bug I want to hear about.

---

Reach me on [Upwork](https://www.upwork.com/) — open to contract work on agent
systems, LLM integration, and automation.
