![Banner](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=EuroRWA&fontSize=55&fontAlignY=35&desc=Real%20data%20infrastructure%20for%20tokenized%20finance&descAlignY=55)

## 👨‍💻 About Me

I build **real data infrastructure for tokenized finance** — dashboards, on-chain verification, and automated research pipelines. My focus is the European tokenized money market fund (MMF) market, where good public data is rare.

- 🔭 **EuroRWA** — live dashboard tracking 15 EU + US tokenized MMFs with real web data
- ⛓️ **On-chain attestation** — every daily snapshot is hashed, signed, and published to a smart contract on Sepolia
- 🛠️ Full pipeline: data fetching → SQLite history → API → React dashboard → auto content generation

## 🛠 Tech Stack

```
TypeScript  ·  Bun  ·  React  ·  Vite
SQLite  ·  Drizzle  ·  Effect
Solidity  ·  Ethereum (Sepolia)  ·  viem
Chrome headless (data-viz)  ·  Vercel
```

## 📌 Featured Project

### 🇪🇺 EuroRWA — EU Tokenized Money Market Fund Dashboard

Live dashboard tracking **15 European and US tokenized money market funds** with real data ($10B+ tracked), refreshed every 12 hours.

**What makes it different — every snapshot is verifiable:**

1. **Hash** the full 15-fund payload (keccak-256)
2. **Sign** with the agent wallet
3. **Publish** to a smart contract on Sepolia — public, permanent, tamper-proof

Anyone can re-hash the data and verify the on-chain signature. No "trust me bro" dashboards.

- 🔴 **Live:** https://rwa-dashboard-gamma.vercel.app
- 📦 **Source:** https://github.com/crytobot459/eurorwa
- 🧪 **Attestation contract (Sepolia):** `0xd482a715cdef4073593f4a3208abd328f6d71725`

## 📊 GitHub Stats

![CrytoBot's GitHub stats](https://github-readme-stats.vercel.app/api?username=crytobot459&show_icons=true&theme=dark)
