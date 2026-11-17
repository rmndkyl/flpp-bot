# FLPP Bot

**Versi:** 1.0.0 · **Harga:** Rp 120.000 (~$8) · **Kontak pembelian:** [@rmndkyl](https://t.me/rmndkyl)

Automated Solana swap volume farming bot for **FLPP.io** (Flipper DEX) — an AI-powered DEX aggregator on Solana.

## Kebutuhan

| Item | Detail |
|---|---|
| Runtime | Node.js 18+ |
| Wallet | EVM / sesuai chain proyek (kamu sendiri) |
| Proxy | opsional (1 proxy per akun) |
| Captcha | tidak perlu |
| Akses | akun proyek yang kamu kelola sendiri |

## Pembayaran

E-Wallet: DANA / GoPay / ShopeePay · Bank: BCA / Seabank · Crypto: contact for wallet address.
Pembeli menghubungi [@rmndkyl](https://t.me/rmndkyl), kirim bukti transfer, lalu terima license key.

---

🌐 **Website:** https://flpp.io

## Features

- **Swap Quote** — Get best route across multiple DEXes (Whirlpool, Quantum, AlphaQ, Manifest)
- **Swap Execution** — Build and send Solana swap transactions via Flipper program
- **Volume Farming** — Multi-round buy/sell cycles for leaderboard volume
- **Wallet Info** — Check wallet tokens, whitelist status, orders, swap events
- **Top Tokens** — Browse trending tokens by organic score
- **Daily Mode** — `--daily` flag for unattended cron execution

## API Endpoints

| Endpoint | Auth | Description |
|----------|------|-------------|
| `GET /api/v1/health` | Public | API health check |
| `GET /api/v1/swap/quote` | Public | Swap routing quote |
| `POST /api/v1/swap/swap-instructions` | Public | Build swap transaction |
| `GET /api/v1/wallet/{addr}` | Public | Wallet token holdings |
| `GET /api/v1/whitelist/wallets/{addr}` | Public | Whitelist status |
| `GET /api/v1/orders?maker=` | Public | Open orders |
| `GET /api/v1/tokens` | Public | Token list |
| `GET /api/v1/market-pulse/tokens/{cat}` | Public | Market pulse data |

**Platform Fee:** 30 bps (0.3%) per swap

## Setup

```bash
npm install
```

```
```

## Usage

```bash
# Interactive mode
node index.js

node index.js --daily
```

### Menu Options

1. **Show Wallet Info** — Check tokens, whitelist, orders
2. **Show Top Tokens** — Browse trending tokens
3. **Single Swap** — Execute one swap with custom amount
4. **Farm Volume** — Multi-round buy/sell cycles
5. **Run All Wallets** — Volume farm for all wallets
6. **Exit**

## Configuration

Edit `config.json`:

```json
{
    "base_url": "https://api-staging.flpp.io",
    "rpc_url": "https://api.mainnet-beta.solana.com",
    "slippage_bps": 50,
    "delay_min": 2000,
    "delay_max": 5000,
    "farm_rounds": 5,
    "farm_amount_lamports": 1000000,
    "input_mint": "So11111111111111111111111111111111111111112",
    "output_mint": "EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v"
}
```

## Requirements

- Node.js 18+
- Solana wallet with SOL for gas (mainnet)
- Private key in base58 format

## Contact

- Telegram: [@rmndkyl](https://t.me/rmndkyl)
- Channel: [@layerairdrop](https://t.me/layerairdrop)
- Group: [@layerairdropdiskusi](https://t.me/layerairdropdiskusi)

## 💰 Harga

| Lisensi | Harga | Fitur |
|---------|-------|-------|
| **Single** | Rp 120.000 / ~$8 | 1 device, lifetime |
| **Bundle (3 bot)** | Rp 120.000 / ~$16 | Pilih 3 bot, hemat 20% |
| **Pro (semua bot)** | Rp 120.000 / ~$70 | Semua bot + update, hemat 30% |

**Cara beli:** Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) di Telegram → /buy

**Bayar pakai:**
- 🇮🇩 DANA / GoPay / ShopeePay / BCA / Seabank
- 🌐 Crypto (USDT/SOL/ETH)

## 🔧 Troubleshooting

| Masalah | Solusi |
|---------|--------|
| `Cannot find module` | Jalankan `npm install` di folder bot |
| `insufficient balance` | Pastikan wallet punya cukup token untuk gas |
| `429 Too Many Requests` | Tunggu 30-60 detik, bot auto-retry |
| Bot diam/tidak jalan | Cek `config.json` — pastikan API key valid |
| License invalid | Chat [@OG_LYID_bot](https://t.me/OG_LYID_bot) → /verify |

**Butuh bantuan?** Join [Discord](https://discord.gg/ZK2NVkfSNn) atau chat [@layerairdrop](https://t.me/layerairdrop)
