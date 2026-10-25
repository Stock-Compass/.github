<p align="center">
  <a href="https://stock-compass.app/zh"><img src="https://raw.githubusercontent.com/Stock-Compass/stock-compass-plugin/main/assets/icon.png" width="88" alt="Stock Compass"></a>
</p>

<h3 align="center">Stock Compass</h3>

<p align="center">把你的选股和止损规则写成策略：回测、每日扫描、记录交易。支持港股、美股和 A 股。</p>

<p align="center"><a href="https://github.com/Stock-Compass">English</a> · <b>简体中文</b></p>

<p align="center">
  <a href="https://stock-compass.app/zh">官网</a> ·
  <a href="https://stock-compass.app/zh/privacy">隐私政策</a> ·
  <a href="mailto:support@stock-compass.app">support@stock-compass.app</a>
</p>

---

把选股和止损规则写成策略，在真实日线上回测，财报日和跳空都算在内。之后 Stock Compass 每个交易日扫描你的股票池，给出买入、加仓、减仓、清仓信号，并帮你记录交易和交易日志。不连券商，不荐股。

### 连接 AI 应用

Stock Compass 提供一个 MCP 服务器，任何支持远程 MCP 和 OAuth 的 AI 应用都能使用你自己的记录：

- **读取**：自选股、持仓、交易、信号和价格提醒。
- **修改（需你允许）**：加入或移出自选股、记录买卖、改止损和目标、设价格提醒。

不会去券商下单。连接需要 Stock Compass Pro。

**MCP 地址：** `https://stock-compass.app/api/mcp`

| 应用 | 怎么连接 |
| --- | --- |
| **Claude**（网页版、桌面版、Cowork） | 安装 [Stock Compass 插件](https://github.com/Stock-Compass/stock-compass-plugin/blob/main/README.zh-CN.md)：Customize → Plugins → Add → Add marketplace → `Stock-Compass/stock-compass-plugin`。插件会装好连接器，并附带一个说明使用规则的 skill。 |
| **Claude Code** | `claude plugin install stock-compass --marketplace Stock-Compass/stock-compass-plugin`，然后运行 `/mcp` 登录。 |
| **ChatGPT** | 打开 [chatgpt.com/plugins](https://chatgpt.com/plugins) → + → Add custom MCP server，粘贴上面的地址，认证选 OAuth。 |
| **其它 MCP 客户端** | 把地址添加为远程 MCP 服务器（Streamable HTTP），认证选 OAuth。 |

每个应用都会把你带到 stock-compass.app 登录并确认授权。默认只读，勾选后才允许修改。随时可以在「设置 → AI 应用与 API」里断开。
