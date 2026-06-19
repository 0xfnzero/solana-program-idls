# Solana Program IDLs

Collected Solana Program IDL files for DEX, launchpad, AMM, CLMM, and bonding-curve integrations used by FnZero parser and trading tools.

## What This Repository Provides

This repository is a lightweight IDL catalog for developers building Solana parsers, trading bots, indexers, explorers, and SDK integrations. It focuses on PumpFun, PumpSwap, Raydium, Meteora, Orca, and related Solana DEX programs.

| Area | Coverage |
|------|----------|
| Program families | PumpFun, PumpSwap, Pump Fees, Raydium AMM/CLMM/CPMM/Launchpad, Meteora AMM/DAMM/DLMM/DBC, Orca Whirlpool |
| File format | JSON IDL files suitable for code generation, parser references, account decoding, and instruction layout checks |
| Use cases | Solana DEX parsers, trading SDKs, bots, indexers, analytics pipelines, protocol integrations |
| Related projects | [`sol-parser-sdk`](https://github.com/0xfnzero/sol-parser-sdk), [`sol-trade-sdk`](https://github.com/0xfnzero/sol-trade-sdk), [`fnzero-examples`](https://github.com/0xfnzero/fnzero-examples) |

## IDL Index

### PumpFun and PumpSwap

| File | Program family |
|------|----------------|
| `pump.json` | PumpFun |
| `pump_amm.json` | PumpSwap / Pump AMM |
| `pump_fees.json` | Pump Fees |

### Raydium

| File | Program family |
|------|----------------|
| `raydium_amm.json` | Raydium AMM |
| `raydium_pool_v4.json` | Raydium Liquidity Pool V4 |
| `raydium_clmm.json` | Raydium CLMM |
| `raydium_clmm_legacy.json` | Raydium CLMM legacy |
| `raydium_cpmm.json` | Raydium CPMM |
| `raydium_launchpad.json` | Raydium Launchpad |

### Meteora

| File | Program family |
|------|----------------|
| `meteora_amm.json` | Meteora AMM |
| `meteora_amm_052.json` | Meteora AMM 0.5.2 |
| `meteora_cp_amm_011.json` | Meteora CP AMM 0.1.1 |
| `meteora_cp_amm_015.json` | Meteora CP AMM 0.1.5 |
| `meteora_damm_v2.json` | Meteora DAMM v2 |
| `meteora_dlmm.json` | Meteora DLMM |
| `meteora_lb_clmm.json` | Meteora LB CLMM |
| `meteora_dynamic_bonding_curve.json` | Meteora Dynamic Bonding Curve |

### Orca

| File | Program family |
|------|----------------|
| `orca_whirlpool.json` | Orca Whirlpool |
| `orca_whirlpool_legacy.json` | Orca Whirlpool legacy |
| `orca_lyf_orca.json` | Orca LYF |

## Notes

- IDLs are provided as reference assets. Always validate program addresses, instruction layouts, and account schemas against the version you use in production.
- For parser and bot examples, see the FnZero SDK repositories linked above.
