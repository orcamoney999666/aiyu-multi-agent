# ORCA Money Bot integration

Set `ORCA_MONEY_BOT_PATH` to the absolute checkout path of `ORCA-MONEY-BOT`.

```bash
export ORCA_MONEY_BOT_PATH=/absolute/path/to/ORCA-MONEY-BOT
node - <<'NODE'
const orca = require('./lib/plugins/orca-money-bot');
console.log(orca.health());
console.log(orca.signal('BTCUSDT'));
NODE
```

The adapter uses the local JSON bridge and is read-only by default. Binance credentials,
risk validation, and live execution remain owned by the main bot.
