# Skills

**用途**：AI Agent Skills 收藏，按类别管理可复用的 Agent 技能定义。

**格式**：`skills/<bucket>/<name>/SKILL.md`，每个 skill 必须有 `name`、`description` 和完整指令。

**收录流程**：
1. 确认 bucket 归属（anthropic / engineering / productivity / misc / personal / in-progress / deprecated）
2. 创建 `skills/<bucket>/<name>/SKILL.md`
3. 更新 `skills/<bucket>/README.md`（bucket 级索引）
4. 更新 `skills/README.md`（总索引）

## Bucket 分类

- `anthropic/` — Anthropic 官方 skills
- `engineering/` — 日常代码工作
- `productivity/` — 日常非代码工作流程工具
- `misc/` — 保留但很少使用
- `personal/` — 与个人环境相关，不予推广
- `in-progress/` — 尚未就绪的草稿
- `deprecated/` — 不再使用

## 索引维护

- `skills/README.md` — 所有 bucket 所有 skill 的统一索引
- `skills/<bucket>/README.md` — 该 bucket 下所有 skill 的列表，名称链接到 `SKILL.md`，附一行描述
