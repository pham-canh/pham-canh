# Phạm Cảnh

**AI agent systems that prove their own work.** I build agents where every claim is
re-derivable from the repo — not screenshots.

I'm a software engineer working on **AI agents, automation, and the verification
around them**. Most agent demos assert that something worked. The pattern I keep
coming back to is making the assertion checkable: an evaluator seat that re-derives
every claim from the artefacts, and a CI gate that fails the build when a claim
and the repo disagree.

- 🔭 **Verifiable agent pipelines** — claim re-derivation, independent evaluation, measurable baselines
- 🛠 **Python-first**, with TypeScript/JavaScript where the interface needs it
- 🧪 **Tested and gated** — tests, CI, and honest fallbacks that report which provider actually answered
- 🌏 Based in Ho Chi Minh City, Vietnam · open to remote

## Selected work

**[opencode-harness-kit](https://github.com/pham-canh/opencode-harness-kit)** —
model-agnostic harness for OpenCode. Capability profiles, context pruning, model
failover, and a `verify` command that checks the installed config against the
profile. MIT, CI on every push, published on npm as
[`opencode-harness-kit`](https://www.npmjs.com/package/opencode-harness-kit).

**[pocketful-factory](https://github.com/pham-canh/pocketful-factory)** —
three coding-agent seats build a wallet service from a written spec, with an
independent evaluator that re-derives every figure and fails when a document
disagrees. 4/4 stages, 36 claims checked by [`verify_claims.py`](https://github.com/pham-canh/pocketful-factory/blob/main/verify_claims.py),
all 121 room messages written by agent seats.

**[voicecare-scheduler](https://github.com/pham-canh/voicecare-scheduler)** —
voice booking for elderly clinic patients: speak, hear the appointment read back,
and nothing is booked without a spoken yes. 28 tests, per-stage latency, and the
UI names the provider that actually answered.
▶ [42s capture](https://youtu.be/z8tE1k7CDfM)

**[eurorwa](https://github.com/pham-canh/eurorwa)** —
research project on independently verifiable snapshots for tokenized money-market
funds: hash the snapshot, sign it, publish the attestation on-chain, and let
anyone re-hash and check the signer with no credentials.

## Competition entries

| Event | Project | What it shows |
|---|---|---|
| BAND Dark Factory — WeAreDevelopers, lablab.ai (2026) | [pocketful-factory](https://github.com/pham-canh/pocketful-factory) | multi-agent factory, independent evaluation, 4/4 stages, offline-built service |
| Nebius × NVIDIA Global AI Hackathon — Devpost (Oct 2026) | [voicecare-scheduler](https://github.com/pham-canh/voicecare-scheduler) | voice agent with a hard consent gate; Nemotron NLU with labelled fallbacks |
| AssemblyAI Voice Agent Hackathon — lablab.ai (2026) | [assemblyai-voice-agent](https://github.com/pham-canh/assemblyai-voice-agent) | realtime STT → NLU booking loop; no booking without a spoken YES |
| Vultr Agent Rush (2026) | [consult-homeopathic](https://github.com/pham-canh/consult-homeopathic) | patient intake with a human doctor in the loop |

Earlier entries kept for history, not pinned:
[dark-factory](https://github.com/pham-canh/dark-factory) (superseded by `pocketful-factory`),
[blast-radius-zero](https://github.com/pham-canh/blast-radius-zero),
[amd-web-retrieval-agent](https://github.com/pham-canh/amd-web-retrieval-agent).

## Research

Separate from the work above, **[eurorwa](https://github.com/pham-canh/eurorwa)** is a
research project, not a product. It studies how public data for tokenized
money-market funds can be collected and then independently verified — a daily
snapshot is hashed (keccak-256), signed with a dedicated key, and the signature
published on-chain, so anyone can re-hash the data and check it against the
attestation. MIT licensed, no paywall, no API key, no hosted service.

**[failed-strategies](https://github.com/pham-canh/failed-strategies)** keeps
backtested strategies that lost money, with post-mortems. Published on purpose:
knowing why an approach failed is more useful than hiding it.

Listing the research apart is the point: the agent work above is what I built to
ship; these are questions I am still working on.

## Tech stack

```
Python  ·  TypeScript / JavaScript  ·  Bash
Node  ·  Docker  ·  GitHub Actions
PostgreSQL  ·  Redis  ·  AWS  ·  OpenTelemetry
LLM providers: NVIDIA Nemotron (Nebius) · Gemini · OpenAI
STT/TTS: AssemblyAI · Edge TTS
```

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
