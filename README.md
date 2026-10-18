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
instead of asserting it. MIT licensed, 131 tests across 9 suites, CI on every push.
Published to npm as [`opencode-harness-kit`](https://www.npmjs.com/package/opencode-harness-kit).

**[assemblyai-voice-agent](https://github.com/pham-canh/assemblyai-voice-agent)**
Voice agent for clinic booking — real-time AssemblyAI STT into Gemini NLU, with
booking gated behind a spoken YES. Latency is reported **per stage in ms**; there
is no hosted demo URL, so run it locally to reproduce the numbers.
*Entry for the AssemblyAI Voice Agent Hackathon, lablab.ai — completed.*

**[pocketful-factory](https://github.com/pham-canh/pocketful-factory)**
Three coding-agent seats in one room build a wallet service, with an independent
evaluator that **re-derives every figure from the evidence and fails if a document
disagrees**. All 121 agent messages are in `room.json` — every tool call, every
verdict, including the last one that fixed a wrong-revision error. The wallet
service the factory produced lives in the `stage-4/` folder of this repo, so you
can hit it over HTTP.
▶ [9s capture](https://github.com/pham-canh/pocketful-factory/blob/main/docs/demo.mp4) — an overdraft refused with the balance unchanged, then the same idempotency key fired twice answering `201` and then `200`.

**[voicecare-scheduler](https://github.com/pham-canh/voicecare-scheduler)**
Voice booking for elderly clinic patients — speak to book, nothing is booked
without a spoken confirmation. NLU on NVIDIA Nemotron via Nebius Token Factory,
with the active provider reported in the UI. 28 tests, a one-command demo
recorder, and a latency claim that matches what the app actually prints.
*Entry for the Nebius x NVIDIA Global AI Hackathon on Devpost — in progress.*
▶ [24s capture](https://github.com/pham-canh/voicecare-scheduler/blob/main/docs/demo.mp4) — the patient speaks, the agent reads back the specialty and time, and the booking only lands after the spoken YES.

**[dark-factory](https://github.com/pham-canh/dark-factory)**
A mini software factory built for the BAND Dark Factory track: spec to code to an
independent evaluator, with **5/5 holdout scenarios** passed. The holdout set is
what stops a factory from grading its own homework.
▶ [5s capture](https://github.com/pham-canh/dark-factory/blob/main/docs/demo.mp4) — one click of *Run factory*, the evaluator answers `5/5 passed (rate 1.0)`. The app needs no API keys, so it runs from a clean checkout.

**[failed-strategies](https://github.com/pham-canh/failed-strategies)**
Backtested trading strategies that lost money, kept with post-mortems. Published
on purpose — knowing why an approach failed is more useful than hiding it.

## Research

Separate from the work above: **[eurorwa](https://github.com/pham-canh/eurorwa)** is a
**research project**, not a product. It studies how public data for tokenized
money-market funds can be collected and then **independently verified** — a daily
snapshot is hashed (keccak-256), signed with a dedicated key, and the signature
published on-chain, so anyone can re-hash the data and check it against the
attestation. MIT licensed, no paywall, no API key, no hosted service.

Listing it apart is the point: the agent work above is things I built to ship, this
is a question I am still working on.

## What I care about

Claim it, then make it checkable. A fallback that silently downgrades the system
is worse than a loud failure, and a README number that the app contradicts is a
bug I want to hear about.

---

Open to contract work on agent systems, LLM integration, and automation.

- LinkedIn — <https://www.linkedin.com/in/canh-pham-bot-dev>
- GitHub — <https://github.com/pham-canh>
- Upwork — <https://www.upwork.com/>

Or open an issue on any repo above.
