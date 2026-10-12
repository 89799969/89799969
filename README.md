<p align="center">
  <img src="assets/profile-banner.svg" alt="halaxy — AI Agent、LLM 应用与开源工程" width="100%" />
</p>

<p align="center">
  <strong>把模型接入真实工具，把问题修到可验证。</strong><br />
  AI Agent / LLM 应用工程 · 工具调用 · 流式协议 · 回归测试
</p>

<p align="center">
  <a href="https://github.com/89799969?tab=repositories">项目仓库</a> ·
  <a href="https://github.com/pulls?q=is%3Apr+author%3A89799969+is%3Amerged">已合并贡献</a> ·
  <a href="https://github.com/89799969/spacedeletor/issues">项目交流</a>
</p>

## 👋 关于我

我是 **halaxy**，关注 **AI Agent / LLM 应用工程**，也参与开发者工具与后端系统的开源维护。

- **应用落地**：在 [SpaceDeletor](https://github.com/89799969/spacedeletor) 中接入 LLM 分析、Function Calling 与桌面交互，将文件扫描、建议生成和人工确认串成完整流程。
- **Agent 工程**：通过 ANOLISA、nanocoder 的上游贡献，处理 Responses / SSE 解析、Token 统计、MCP 配置来源与调度生命周期问题。
- **工程习惯**：围绕具体缺陷定位数据流、补充回归测试，并在 PR 中说明验证结果与边界。

**求职方向**：AI Agent / LLM 应用开发、AI 开发者工具，以及与 AI 应用相关的后端工程岗位。

## 🧩 重点项目

### [SpaceDeletor](https://github.com/89799969/spacedeletor) · AI 辅助磁盘清理工具

`Python` `PySide6 / Qt` `LLM API` `Function Calling` `pytest`

面向本地大文件整理场景，将文件元数据分析与可操作的清理建议结合，提供 **Qt GUI 与 CLI** 两种入口。

- **模型接入**：支持可配置的 OpenAI 兼容接口；对指定模型使用 JSON Schema 约束输出。
- **工具调用**：对不确定文件启动多轮 Agent 分析，提供文件元数据查询和网页搜索工具。
- **请求可靠性**：实现批处理、并发与限速、超时和指数退避；校验返回条目，对缺失结果补提，并保留需要复核的项。
- **执行交互**：展示建议动作与原因，通过用户确认执行清理；包含配置、扫描、AI 客户端和清理流程的测试文件。

[查看代码](https://github.com/89799969/spacedeletor/tree/main/spacedeletor) · [使用说明](https://github.com/89799969/spacedeletor#readme) · [测试用例](https://github.com/89799969/spacedeletor/tree/main/tests)

### 其他实践

| 项目 | 内容 | 技术 |
| :--- | :--- | :--- |
| [Memory Game](https://github.com/89799969/memory-game) | 记忆翻牌游戏，包含后端游戏状态、难度选择和实时计分 | Python · Flask · JavaScript |
| [Binary Multiplication](https://github.com/89799969/binary-multiplication-manim) | 用寄存器与移位动画解释二进制乘法过程 | Python · Manim |

## 🔀 开源贡献精选

以下为我向上游提交、**已合并**的代表性 PR。项目名称链接到上游仓库，PR 链接展示具体改动。

| 上游项目 | 具体贡献 | PR |
| :--- | :--- | :--- |
| [ANOLISA / AgentSight](https://github.com/agentic-os-org/ANOLISA) | 修复 Responses SSE 中并行工具调用丢失，保留调用 ID、名称与参数，并补充回归测试 | [#4116](https://github.com/agentic-os-org/ANOLISA/pull/4116) |
| [ANOLISA / AgentSight](https://github.com/agentic-os-org/ANOLISA) | 补齐 Responses 缓存 Token 读取、供应商识别与字段解析，修正计数语义 | [#4249](https://github.com/agentic-os-org/ANOLISA/pull/4249) |
| [nanocoder](https://github.com/Nano-Collective/nanocoder) | 保留 MCP 配置来源，使项目级配置进入凭据安全校验 | [#1256](https://github.com/Nano-Collective/nanocoder/pull/1256) |
| [nanocoder](https://github.com/Nano-Collective/nanocoder) | 为共享 cron 表达式增加引用计数，避免取消一个订阅后影响其他订阅 | [#1255](https://github.com/Nano-Collective/nanocoder/pull/1255) |
| [Apache RocketMQ Dashboard](https://github.com/apache/rocketmq-dashboard) | 在实例删除事务提交后清理数据源缓存，补充缓存与提交时序的回归覆盖 | [#4202](https://github.com/apache/rocketmq-dashboard/pull/4202) |
| [Subtitle Edit](https://github.com/SubtitleEdit/subtitleedit) | 修复 DeepSeek 翻译请求中自定义 Prompt 缺少 JSON 编码的问题 | [#11150](https://github.com/SubtitleEdit/subtitleedit/pull/11150) |

## 🛠 技术与实践

| 方向 | 公开项目 / 贡献中使用的技术 | 对应实践 |
| :--- | :--- | :--- |
| LLM 应用与 Agent | LLM API · Function Calling · JSON Schema · MCP · SSE | 模型接入、工具调用、结构化结果与流式事件处理 |
| 应用开发 | Python · PySide6 · Flask · JavaScript | 桌面交互、CLI 与 Web 应用 |
| 开源代码维护 | Rust · TypeScript · Java · C# | Agent 可观测性、配置与调度、事务缓存、翻译请求 |
| 质量保障 | pytest · Cargo test · TypeScript 测试 · Maven / JUnit | 缺陷复现、回归覆盖与 PR 验证说明 |

---

<p align="center">
  欢迎围绕 AI 应用、Agent 工具链与开源协作交流。<br />
  <a href="https://github.com/89799969">GitHub @89799969</a>
</p>
