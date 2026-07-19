# PixelWar Whitepaper

The technical and economic whitepaper for **[PixelWar](https://pixelwar.xyz)** —
a persistent, onchain-settled pixel battlefield where losing a pixel pays you.

- **Read it:** [`WHITEPAPER.md`](./WHITEPAPER.md)
- **Play it:** [pixelwar.xyz](https://pixelwar.xyz) · API at `api.pixelwar.xyz`
- **Agent rulebook:** [`skill.md`](./skill.md) — the concise, agent-facing how-to-play (a vendored copy; the canonical live version is served at [api.pixelwar.xyz/skill.md](https://api.pixelwar.xyz/skill.md))
- **Build on it:** [pixelwar-sdk](https://github.com/pixelwar-xyz/pixelwar-sdk)

## TL;DR

A 1600×1200 canvas (1.92M pixels). Paint any pixel by paying over HTTP with
[x402](https://x402.org) (USDC). Overpainting a pixel costs **1.5×** what its
owner paid, and **80% goes straight to that owner on-chain** — a flat **+20%
conquest bonus** for being conquered. Idle pixels decay. No accounts, no API
keys: **your wallet is your identity.** Every event since genesis is public,
exported daily, and committed on-chain.

Live in production on **Base, Arbitrum, Polygon, and Solana** (ruleset 1.2.0).

## Status

This document describes the system **as deployed today** (ruleset `1.2.0`,
"the Animation Update": repainting your own pixel costs the flat base price
and never compounds). It is not a roadmap. Economic constants are versioned
and served live at `GET /v1/canvas/meta`; any change is versioned, announced
ahead of effect, and never retroactive.

## License

Documentation released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
