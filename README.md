# codex的优化包

适合非专业开发者的 Codex 项目复用与提效配置：先找成熟项目，优先直接使用或少量修改，减少从零开发、重复搜索和无效试错。

## 使用方式

1. 把 skills/reuse-first 文件夹复制到当前用户的 .agents/skills/ 下。
2. 将 templates/AGENTS.md 中的规则合并到 Codex 用户目录的 AGENTS.md，修改前备份，不覆盖原有规则。
3. 新开本地 Codex 会话，描述需求即可；也可明确说“使用 $reuse-first”。

详细安装、验证及回滚步骤见 [安装说明](docs/安装说明.md)。

## 默认流程

理解需求 → 查项目已有资源与复用记录 → 用中英文有限检索 GitHub → 深入核实最相关的 2—3 个候选 → 选择并实施 → 必要验证 → 保存 docs/reuse-decisions.md。

实施优先级：直接使用 → 配置 → 修改 → 少量组件复用 → 从零开发。没有合适方案时继续必要开发，不为复用强行采用复杂系统。

错别字、颜色、少量字段等小改直接处理。已调查的方案在需求和版本未变时直接复用。

## 工具原则

优先已有网页搜索、Git、文件搜索和浏览器。GitHub MCP、Context7、Playwright、Serena 按实际需求评估，不默认全部安装；不默认开启多 Agent。

见 [工具评估](docs/工具评估.md) 和 [验证结果](docs/验证结果.md)。

本包不包含模型、登录、订阅、密钥、个人 config.toml、电脑原始备份或会话日志；不会降低审批权限。不承诺固定额度节省比例。

## 适用范围与官方依据

本包在 Windows 本地 Codex 环境完成行为验证，日期为 2026-10-16。其他系统与未来版本使用前应核对官方文档。全局规则是指导，项目规则与用户明确要求会影响具体行为。

- [全局 AGENTS.md](https://developers.openai.com/codex/guides/agents-md)
- [Skills](https://developers.openai.com/codex/skills)
- [配置路径](https://developers.openai.com/codex/config-basic)
