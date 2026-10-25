<p align="center">
  <a href="https://stock-compass.app"><img src="https://raw.githubusercontent.com/Stock-Compass/stock-compass-plugin/main/assets/icon.png" width="88" alt="Stock Compass"></a>
</p>

<h3 align="center">Stock Compass</h3>

<p align="center">Rule-based stock strategies for Hong Kong, US and China A-share investors.</p>

<p align="center"><b>English</b> · <a href="https://github.com/Stock-Compass/.github/blob/main/profile/README.zh-CN.md">简体中文</a></p>

<p align="center">
  <a href="https://stock-compass.app/en">Website</a> ·
  <a href="https://stock-compass.app/en/privacy">Privacy</a> ·
  <a href="mailto:support@stock-compass.app">support@stock-compass.app</a>
</p>

---

Write your stock-picking and stop-loss rules as a strategy. Backtest them on real daily prices, with earnings days and gaps included. Then Stock Compass scans your watchlist every trading day for buy, add, trim and exit signals, and keeps your trades and trade journal. No broker link, no stock tips.

### Connect AI apps

Stock Compass runs an MCP server, so any AI app that supports remote MCP servers with OAuth can work with your own records:

- **Read**: your watchlist, holdings, trades, signals and price alerts.
- **Change, if you allow it**: record trades, change stops and targets, and set price alerts.

It never places an order with a broker. Connecting needs Stock Compass Pro.

**MCP address:** `https://stock-compass.app/api/mcp`

| App | How to connect |
| --- | --- |
| **Claude** (web, desktop app, Cowork) | Install the [Stock Compass plugin](https://github.com/Stock-Compass/stock-compass-plugin): Customize → Plugins → Add → Add marketplace → `Stock-Compass/stock-compass-plugin`. The plugin adds the connector and a skill with the rules for using it. |
| **Claude Code** | `claude plugin install stock-compass --marketplace Stock-Compass/stock-compass-plugin`, then run `/mcp` to sign in. |
| **ChatGPT** | [chatgpt.com/plugins](https://chatgpt.com/plugins) → + → Add custom MCP server. Paste the address and choose OAuth. |
| **Other MCP clients** | Add the address as a remote MCP server (Streamable HTTP) with OAuth. |

Every app sends you to stock-compass.app to sign in and approve it. Approval is read only by default; you tick changes to allow them. Disconnect at any time in Settings → AI apps & API.
