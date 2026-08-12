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

## Current Upstream Sources

The unversioned filenames track the protocol-maintained current IDL. Files explicitly named
`legacy`, `011`, `015`, or another historical version remain pinned snapshots.

| File | Official upstream | Version | Canonical SHA-256 |
|------|-------------------|---------|------------------|
| `pump.json` | `pump-fun/pump-public-docs/idl/pump.json` | 0.1.0 | `ab1b3b5a85b2bb3aade5dc7bacb2f5e75e62a242db6f2828d9addbf09d8d864e` |
| `pump_amm.json` | `pump-fun/pump-public-docs/idl/pump_amm.json` | 0.1.0 | `b85ddba5f4611e9e2cd0695d1204a40f16db15d48b1b8ad4177abee194dc5141` |
| `pump_fees.json` | `pump-fun/pump-public-docs/idl/pump_fees.json` | 0.1.0 | `1177093f22cfef08d5474025b44ace9ba97960ecd04dc87b4530a33072194bb5` |
| `raydium_clmm.json` | `raydium-io/raydium-idl/raydium_clmm/raydium_clmm.json` | 0.1.0 | `ce860422ec1e3284e89e165d9740c9f19f861ab45e0ad5bfc7ca647b6af39496` |
| `raydium_cpmm.json` | `raydium-io/raydium-idl/raydium_cpmm/raydium_cp_swap.json` | 0.2.0 | `a4cc67efdc1374a3d6f8a1d7f16627bcda2deecdb65b2413fa336e973b97b52f` |
| `raydium_launchpad.json` | `raydium-io/raydium-idl/raydium_launchpad/raydium_launchpad.json` | 0.2.0 | `03713b809cd62272f63ebf5ca5ad06a64f6f7a3ac493a9f49d2c3b2aa43aca68` |
| `meteora_dlmm.json` / `meteora_lb_clmm.json` | `MeteoraAg/dlmm-sdk/idls/dlmm.json` | 0.12.0 | `1bc4333e5702dddb51d9ad92b6e9298940c9d9ff7f92fd761b634a03cf2d7daf` |
| `meteora_damm_v2.json` | `MeteoraAg/damm-v2-sdk/src/idl/cp_amm.json` | 0.2.2 | `44cba19689609a51e3c0ab44fb04f7c85e9eacf72f05fd013f0f4c753eb42f0a` |
| `meteora_dynamic_bonding_curve.json` | `MeteoraAg/dynamic-bonding-curve-sdk/packages/dynamic-bonding-curve/src/idl/dynamic-bonding-curve/idl.json` | 0.2.0 | `b28d0683f164e8ebc510190a605be493ea2ecd39c02c8852960e41120847a822` |
| `meteora_amm.json` | `MeteoraAg/dynamic-bonding-curve/idls/dynamic_amm.json` | 0.5.2 | `21f59f98c8a593ac2a9d976889cff8d8b618fe3aa1fb5c0132d5ca598c59a833` |
| `orca_whirlpool.json` | `@orca-so/whirlpools-sdk@0.22.0/dist/artifacts/whirlpool.json` | 0.9.0 | `301335733544288d52aae316827c4e2bbf4e27edbd3d87bd1711de1251e3b1ee` |

Canonical hashes are calculated with `jq -S -c . | sha256sum`, so formatting differences do not
change the result. Raydium AMM V4 is not an Anchor program; `raydium_amm.json` remains a
compatibility reference, while current instruction and `ray_log` layouts are defined by
`raydium-io/raydium-amm`.
