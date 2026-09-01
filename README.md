# Workmint — Mint Your Labor, Claim Your Worth

[![Go Version](https://img.shields.io/badge/Go-1.21+-00ADD8?style=flat&logo=go)](https://go.dev/)
[![Solidity](https://img.shields.io/badge/Solidity-^0.8.0-363636?style=flat&logo=solidity)](https://soliditylang.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Workmint** is a decentralized platform that turns real‑world labor into verifiable on‑chain credentials.  
> We empower delivery riders, cleaners, ride‑hailing drivers, and all unsung workers to own their work history and receive fair compensation — free from exorbitant platform fees.

---

## 🚀 The Problem

Millions of gig workers (food deliverers, domestic cleaners, ride‑hailing drivers) are the backbone of our daily lives. Yet they face:

- **High commission fees** — platforms take 20‑30% of their earnings.
- **No portable reputation** — their hard‑earned trust and ratings are locked inside closed platforms.
- **Delayed or opaque payments** — no real‑time visibility into settlement rules.
- **No voice in governance** — platform policies change unilaterally, affecting their livelihoods.

These workers generate immense real value, but the value flows disproportionately to intermediaries.

---

## 💡 Our Vision

**Workmint re‑imagines the relationship between workers and platforms.**

We use blockchain as a **transparent, immutable ledger** to record every completed task (with cryptographic proof). Workers own their work records as **portable credentials** — they can take their reputation anywhere. Smart contracts automate fair fee structures and instant settlements. A community‑driven DAO gives workers a direct vote on platform rules.

**This is not about speculation. This is about dignity, transparency, and economic justice for the people who move our world.**

---

## 🛠️ How It Works (Technical Overview)

- **Proof of Physical Work** — A lightweight Go service captures geo‑hashed timestamps and task metadata, generating a unique `taskHash` that represents the actual labor.
- **On‑chain Settlement** — Smart contracts (Solidity) record the `taskHash` on an Ethereum L2 testnet (Sepolia) with the worker’s address, making it tamper‑proof and publicly verifiable.
- **Backend & API** — Written in Go following **Clean Architecture**, the backend handles user management, off‑chain caching, and orchestrates the interaction with the blockchain.
- **Frontend (coming soon)** — A simple web/mobile interface for workers to view their records and receive payments.

Our development environment runs on a ThinkPad X280 (i5‑8350U, 16GB RAM) — proving that decent Web3 development does **not** require expensive hardware.

---

## 🗺️ Roadmap

| Phase | Milestone |
|-------|-----------|
| **Phase 0 (Done)** | Concept validation, basic Solidity contract + Go client to record labor proofs on Sepolia testnet. |
| **Phase 1** | Build Clean Architecture backend (domain, usecase, adapters) with PostgreSQL for off‑chain worker profiles. |
| **Phase 2** | Deploy a minimal DAO governance contract for fee voting. |
| **Phase 3** | Develop a mobile‑first frontend (React Native or PWA) with account abstraction (ERC‑4337) for phone‑number login. |
| **Phase 4** | Pilot with a small group of real workers, iterate based on feedback. |
| **Phase 5** | Explore multi‑chain support and integration with stablecoin payments. |

---

## 🧱 Project Structure (Clean Architecture)
