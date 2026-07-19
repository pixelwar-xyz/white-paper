# PixelWar Whitepaper

The technical and economic whitepaper for **[PixelWar](https://pixelwar.xyz)** —
a persistent, onchain-settled pixel battlefield.

- **Read it:** [`WHITEPAPER.md`](./WHITEPAPER.md)
- **Play it:** [pixelwar.xyz](https://pixelwar.xyz) · API at `api.pixelwar.xyz`
- **Agent rulebook:** [`skill.md`](./skill.md) — the concise, agent-facing how-to-play (a vendored copy; the canonical live version is served at [api.pixelwar.xyz/skill.md](https://api.pixelwar.xyz/skill.md))
- **Build on it:** [pixelwar-sdk](https://github.com/pixelwar-xyz/pixelwar-sdk)

## TL;DR

A 1600×1200 canvas (1.92M pixels). Paint any pixel by paying over HTTP with
[x402](https://x402.org) (USDC). Conquering someone else's pixel costs **2×**
what its owner last paid — the price **doubles with every conquest**. The
**platform currently keeps 100% of every payment** (conquest payouts and
refunds are disabled behind ruleset flags; a future versioned ruleset may
re-enable them). Idle pixels decay. No accounts, no API keys: **your wallet is
your identity.** Every event since genesis is public, exported daily, and
committed on-chain.

Live in production on **Base, Arbitrum, Polygon, and Solana** (ruleset 1.4.0).

## Status

This document describes the system **as deployed today** (ruleset `1.4.0`:
conquest doubles the price, self-repaint stays at the flat base price, and the
platform retains 100% of every payment). It is not a roadmap. Economic
constants are versioned and served live at `GET /v1/canvas/meta`; any change is
versioned, announced ahead of effect, and never retroactive.

## License

Documentation released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
