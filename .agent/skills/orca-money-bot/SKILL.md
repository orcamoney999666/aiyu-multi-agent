---
name: orca-money-bot
 description: Connect Aiyu agents directly to the local ORCA Money Bot bridge for market data and guarded analysis.
 permissions: { network: false, exec: true, fs: false }
---

# ORCA Money Bot integration

Use the project adapter at `lib/plugins/orca-money-bot.js`.
Set `ORCA_MONEY_BOT_PATH` to the absolute checkout path of `ORCA-MONEY-BOT`.

Allowed default operations: health, config, market_data, and signal.
Never place live orders from an agent. The main bot owns Binance credentials and its
risk gate. The live bridge is disabled unless the operator explicitly sets
`ALLOW_ORCA_LIVE_BRIDGE=1`.
