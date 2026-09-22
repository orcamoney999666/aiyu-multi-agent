# ORCA Money Bot integration

This repository now has a direct, local adapter at `lib/plugins/orca-money-bot.js`.
It invokes `ORCA-MONEY-BOT/orca_bridge.py` without paid services or network middleware.

```bash
export ORCA_MONEY_BOT_PATH=/absolute/path/to/ORCA-MONEY-BOT
node - <<'NODE'
const orca = require('./lib/plugins/orca-money-bot');
console.log(orca.health());
console.log(orca.signal('BTCUSDT'));
NODE
```
