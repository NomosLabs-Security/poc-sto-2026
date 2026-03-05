# STO — Flawed Burn Mechanism Price Manipulation — PoC

> **Educational Purpose Only** — This PoC is created solely for security
> research and educational purposes. It runs against a fork, not mainnet.

## Quick Start

```bash
git clone https://github.com/NomosLabs-Security/poc-sto-2026
cd poc-sto-2026
forge install foundry-rs/forge-std --no-git
forge test -vvvv
```

## Details

- **Exploit Date:** 2026-02-23
- **Fork Block:** #82890986 (one block before attack)
- **Expected Output:** ~26.57 WBNB profit (~$17.5K) via burn-triggered price manipulation
- **Full Analysis:** [NomosLabs Security Intelligence Archive](https://nomoslabs.io/archive/sto-2026)

## RPC Providers

This PoC uses a BNB Smart Chain mainnet fork. You need an RPC endpoint:

| Provider | Free Tier | URL Format |
|----------|-----------|------------|
| [Alchemy](https://www.alchemy.com/) | 300M compute units/mo | `https://bnb-mainnet.g.alchemy.com/v2/YOUR_KEY` |
| [QuickNode](https://www.quicknode.com/) | 10M API credits/mo | `https://YOUR_ENDPOINT.bsc.quiknode.pro/YOUR_KEY` |
| [Public RPC](https://docs.bnbchain.org/docs/rpc/) | Rate limited | `https://bsc-dataseed.binance.org/` |

Update `eth_rpc_url` in `foundry.toml` with your own endpoint.

## License

MIT — For educational use only.
