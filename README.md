# SmartMoneyOracle — Whale & Institutional Flow Intelligence MCP Server

> Protocol TVL flows, institutional tracking, alpha signals, cross-chain capital movement, stablecoin supply. 8 tools.

**Part of [ToolOracle](https://tooloracle.io) — Policy-enforced, tier-gated, usage-metered tool execution**

[![SmartMoneyOracle MCP server](https://glama.ai/mcp/servers/ToolOracle/smartmoneyoracle/badges/card.svg)](https://glama.ai/mcp/servers/ToolOracle/smartmoneyoracle)

## Connect

```bash
npx -y mcp-remote https://tooloracle.io/smart/mcp/
```

## x402 Pay-per-call (autonomous agents)

```
POST https://tooloracle.io/x402/smart/mcp/
→ 402 with structured pricing → Send USDC on Base → Retry with X-PAYMENT header
```

## 8 Tools · 1 unit = $0.01

| Tool | Units | Price | Tier |
|------|-------|-------|------|
| `institutional` | 10 | $0.10 | Premium |
| `alpha_signal` | 10 | $0.10 | Premium |
| `flow_scan` | 5 | $0.05 | Deep |
| `protocol_flows` | 5 | $0.05 | Deep |
| `top_whales` | 3 | $0.03 | Standard |
| `chain_flows` | 3 | $0.03 | Standard |
| `stablecoin_flows` | 3 | $0.03 | Standard |
| `health_check` | 0 | free | — |

## Alpha scoring

`alpha_signal` combines price momentum + volume surge + buy pressure + whale boost activity into a single score: COLD → WARMING → HOT → EXPLOSIVE.

## Tier gating

| Tier | Max/call | Blocked |
|------|----------|---------|
| Free ($0) | 3 units | institutional, alpha_signal |
| Starter ($49/mo) | 8 units | — |
| Pro+ / x402 | 15 units | — |

## Data sources (all free)

DeFiLlama (TVL, protocols, stablecoins) · DexScreener (whale boosts, CTOs) · CoinGecko (trending)

## Links

- [ToolOracle](https://tooloracle.io) · [x402 Gateway](https://tooloracle.io/x402/)
- [RankOracle](https://github.com/ToolOracle/rankoracle) · [ShopOracle](https://github.com/ToolOracle/shoporacle) · [MemeOracle](https://github.com/ToolOracle/memeoracle) · [YieldOracle](https://github.com/ToolOracle/yieldoracle)