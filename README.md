## Anthropic

Anthropic 官方 skills。

- **[agent-identifier](./skills/anthropic/agent-identifier/SKILL.md)** — 当用户要求"创建 agent"、"添加 agent"、"编写 subagent"或需要 agent 结构、触发条件、开发最佳实践指导时使用。
- **[algorithmic-art](./skills/anthropic/algorithmic-art/SKILL.md)** — 使用 p5.js 创建算法艺术，含种子随机性和交互式参数探索，用于生成艺术、流场、粒子系统等。
- **[brand-guidelines](./skills/anthropic/brand-guidelines/SKILL.md)** — 应用 Anthropic 官方品牌颜色和字体风格，适用于需要 Anthropic 视觉风格的各种产出物。
- **[canvas-design](./skills/anthropic/canvas-design/SKILL.md)** — 使用设计理念创建精美的 .png 和 .pdf 视觉艺术作品，如海报、静态设计等。
- **[claude-api](./skills/anthropic/claude-api/SKILL.md)** — Claude API / Anthropic SDK 参考：模型 ID、定价、参数、流式、工具调用、MCP、Agent、缓存、Token 计数、模型迁移。
- **[doc-coauthoring](./skills/anthropic/doc-coauthoring/SKILL.md)** — 结构化文档协作编写流程：高效传递上下文、迭代精炼内容、验证文档对读者的可用性。
- **[docx](./skills/anthropic/docx/SKILL.md)** — Word 文档全生命周期处理：创建、读取、编辑、格式化 .docx，支持目录、页眉、页码、信头、修订标记和注释。
- **[find-skills](./skills/anthropic/find-skills/SKILL.md)** — 帮助用户发现和安装 Agent Skill，回答"有没有能做 X 的 skill"类问题。
- **[frontend-design](./skills/anthropic/frontend-design/SKILL.md)** — 构建或重塑 UI 时的独特视觉设计指导：美学方向、字体排版，避免模板化默认设计。
- **[fund-advisor](./skills/anthropic/fund-advisor/SKILL.md)** — 基金定投顾问：定投计算（复利+真实年化）、收益模拟、资产配置、再平衡建议、止盈策略、基金类型科普。
- **[hello-world](./skills/anthropic/hello-world/SKILL.md)** — 当用户输入 hello-world 时，直接输出 hello world!
- **[internal-comms](./skills/anthropic/internal-comms/SKILL.md)** — 内部沟通文档写作工具包：状态报告、领导层更新、公司新闻简报、FAQ、事故报告、项目更新等。
- **[mcp-builder](./skills/anthropic/mcp-builder/SKILL.md)** — MCP 服务器构建指南：为 LLM 集成外部 API 和服务创建高质量的工具，支持 Python (FastMCP) 和 Node/TypeScript (MCP SDK)。
- **[pdf](./skills/anthropic/pdf/SKILL.md)** — PDF 全功能处理：读取/提取文字表格、合并、拆分、旋转、水印、创建、填表、加密/解密、扫描件 OCR。
- **[pptx](./skills/anthropic/pptx/SKILL.md)** — .pptx 全生命周期处理：创建、编辑演示文稿，提取文本，合并/拆分幻灯片，处理模板、布局、演讲者备注。
- **[prompt-lookup](./skills/anthropic/prompt-lookup/SKILL.md)** — 当用户咨询 AI 提示词、需要提示词模板、搜索提示词或提及 prompts.chat 时激活。
- **[skill-creator](./skills/anthropic/skill-creator/SKILL.md)** — 创建、修改和优化 Skill：从零创建、编辑现有 Skill、运行评估、基准测试、优化触发准确率。
- **[slack-gif-creator](./skills/anthropic/slack-gif-creator/SKILL.md)** — 创建 Slack 优化的动画 GIF：提供约束、验证工具和动画概念。
- **[theme-factory](./skills/anthropic/theme-factory/SKILL.md)** — 为各种产出物应用主题样式，含 10 套预设主题（颜色/字体），也可即时生成新主题。
- **[web-artifacts-builder](./skills/anthropic/web-artifacts-builder/SKILL.md)** — 使用 React、Tailwind CSS、shadcn/ui 创建复杂多组件的 claude.ai HTML 制品。
- **[webapp-testing](./skills/anthropic/webapp-testing/SKILL.md)** — 使用 Playwright 与本地 Web 应用交互测试：验证前端功能、调试 UI 行为、浏览器截图、查看日志。
- **[xlsx](./skills/anthropic/xlsx/SKILL.md)** — 电子表格全生命周期处理：.xlsx/.xlsm/.csv/.tsv 的创建、读取、编辑、格式化、图表、数据清理与格式转换。

## Engineering

日常代码工作。

- **[diagnose](./skills/engineering/diagnose/SKILL.md)** — 规范化调试流程：复现 → 最小化 → 假设 → 插桩 → 修复 → 回归测试，用于处理疑难 Bug 和性能退化。
- **[grill-with-docs](./skills/engineering/grill-with-docs/SKILL.md)** — 深度质询会话：对照现有领域模型挑战你的方案，打磨术语，同步更新 `CONTEXT.md` 和 ADR。
- **[improve-codebase-architecture](./skills/engineering/improve-codebase-architecture/SKILL.md)** — 在代码库中发现深化设计的机会，基于 `CONTEXT.md` 中的领域语言和 `docs/adr/` 中的决策。
- **[prototype](./skills/engineering/prototype/SKILL.md)** — 构建一次性原型以验证设计——可以是用于状态/业务逻辑问题的可运行终端应用，也可以是从同一路由切换的多个截然不同的 UI 方案。
- **[setup-matt-pocock-skills](./skills/engineering/setup-matt-pocock-skills/SKILL.md)** — 为每个仓库搭建配置（Issue 追踪器、Triage 标签词汇表、领域文档布局），是其他工程类 skill 的前置依赖。
- **[tdd](./skills/engineering/tdd/SKILL.md)** — 测试驱动开发，红-绿-重构循环。每次构建一个垂直切片的功能或修复一个 Bug。
- **[to-issues](./skills/engineering/to-issues/SKILL.md)** — 将任何计划、规格说明或 PRD 拆分为可独立领取的 GitHub Issue，采用垂直切片方式。
- **[to-prd](./skills/engineering/to-prd/SKILL.md)** — 将当前会话上下文转化为 PRD 并提交为 GitHub Issue。无需访谈——直接综合已讨论的内容。
- **[triage](./skills/engineering/triage/SKILL.md)** — 通过状态机驱动的分类角色对 Issue 进行分类处理。
- **[zoom-out](./skills/engineering/zoom-out/SKILL.md)** — 让 Agent 跳出细节，对不熟悉的代码段给出更宏观的上下文或高层次视角。

## Productivity

日常非代码工作流程工具。

- **[caveman](./skills/productivity/caveman/SKILL.md)** — 极致压缩沟通模式。砍掉填充词，节省约 75% token，保持完整技术准确性。
- **[llm-wiki](./skills/productivity/llm-wiki/SKILL.md)** — 用 LLM 构建和维护个人知识库 Wiki。支持资料导入、智能查询、健康检查，以 Markdown 文件 + Git 版本管理。
- **[caveman-zh](./skills/productivity/caveman-zh/SKILL.md)** — 中文极致压缩模式。砍掉客套话、填充词、冗余修饰，节省约 60-70% token，保留全部技术准确性。
- **[grill-me](./skills/productivity/grill-me/SKILL.md)** — 对方案或设计进行无死角质询，直到决策树的每个分支都被解决。
- **[handoff](./skills/productivity/handoff/SKILL.md)** — 将当前会话压缩为交接文档，让另一个 Agent 可以接续工作。
- **[teach](./skills/productivity/teach/SKILL.md)** — 多阶段教学：以当前目录为状态化教学空间，分多次会话教授新技能或概念。
- **[write-a-skill](./skills/productivity/write-a-skill/SKILL.md)** — 创建结构规范、遵循渐进披露原则并附带资源的 Skill。

## Misc

保留但很少使用。

- **[git-guardrails-claude-code](./skills/misc/git-guardrails-claude-code/SKILL.md)** — 配置 Claude Code hooks，在执行危险 git 命令（push、reset --hard、clean 等）前拦截确认。
- **[migrate-to-shoehorn](./skills/misc/migrate-to-shoehorn/SKILL.md)** — 将测试文件中的 `as` 类型断言迁移为 @total-typescript/shoehorn。
- **[scaffold-exercises](./skills/misc/scaffold-exercises/SKILL.md)** — 创建练习目录结构，包含章节、问题、解答和说明。
- **[setup-pre-commit](./skills/misc/setup-pre-commit/SKILL.md)** — 配置 Husky pre-commit hooks，含 lint-staged、Prettier、类型检查和测试。

---

本仓库为个人日常收集的实用 skills 合集，包含自己编写和从社区精选的 skills，仅供学习与使用便利，非抄袭。

来源包括但不限于：
- [mattpocock/skills](https://github.com/mattpocock/skills)
- [anthropics/skills](https://github.com/anthropics/skills)
