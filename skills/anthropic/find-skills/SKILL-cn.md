---

name: find-skills 
description: 当用户提出类似“我该如何做 X”、“寻找关于 X 的技能”、“是否有可以...的技能”等问题，或表现出扩展能力的兴趣时，帮助用户发现并安装 Agent 技能。当用户寻找可能以可安装技能形式存在的功能时，应使用此技能。

---

# 寻找技能 (Find Skills)

此技能可帮助你从开放的 Agent 技能生态系统中发现并安装技能。

## 何时使用此技能

当用户出现以下情况时使用：

* 询问“我该如何做 X”，而 X 可能是已有技能覆盖的常见任务
* 说“寻找关于 X 的技能”或“有关于 X 的技能吗”
* 询问“你能做 X 吗”，而 X 是一项专业能力
* 表现出扩展 Agent 能力的兴趣
* 想要搜索工具、模板或工作流
* 提到希望在特定领域（设计、测试、部署等）获得帮助

## 什么是 Skills CLI？

Skills CLI (`npx skills`) 是开放 Agent 技能生态系统的包管理器。技能是模块化的软件包，通过专业的知识、工作流和工具来扩展 Agent 的能力。

**核心命令：**

* `npx skills find [query]` - 通过交互方式或关键词搜索技能
* `npx skills add <package>` - 从 GitHub 或其他来源安装技能
* `npx skills check` - 检查技能更新
* `npx skills update` - 更新所有已安装的技能

**浏览技能地址：** [https://skills.sh/](https://skills.sh/)

## 如何帮助用户寻找技能

### 第一步：了解他们的需求

当用户寻求帮助时，请确认：

1. 领域（例如：React, 测试, 设计, 部署）
2. 具体任务（例如：编写测试, 创建动画, 审查 PR）
3. 这是否是一个可能有现成技能支持的常见任务

### 第二步：搜索技能

运行带有相关查询词的查找命令：

```bash
npx skills find [query]

```

例如：

* 用户问“如何让我的 React 应用更快？” → `npx skills find react performance`
* 用户问“你能帮我审查 PR 吗？” → `npx skills find pr review`
* 用户问“我需要创建一个变更日志” → `npx skills find changelog`

该命令将返回如下结果：

```
使用 npx skills add <owner/repo@skill> 进行安装

vercel-labs/agent-skills@vercel-react-best-practices
└ https://skills.sh/vercel-labs/agent-skills/vercel-react-best-practices

```

### 第三步：向用户展示选项

当你找到相关的技能时，向用户展示：

1. 技能名称及其功能
2. 他们可以运行的安装命令
3. 在 skills.sh 了解更多详情的链接

示例回复：

```
我找到了一个可能有所帮助的技能！"vercel-react-best-practices" 技能提供了来自 Vercel 工程团队的 React 和 Next.js 性能优化指南。

安装命令：
npx skills add vercel-labs/agent-skills@vercel-react-best-practices

了解更多：https://skills.sh/vercel-labs/agent-skills/vercel-react-best-practices

```

### 第四步：提供安装建议

如果用户希望继续，你可以为他们安装该技能：

```bash
npx skills add <owner/repo@skill> -g -y

```

`-g` 标志表示全局安装（用户级），`-y` 表示跳过确认提示。

## 常见技能类别

搜索时，请考虑以下常见类别：

| 类别 | 示例查询词 |
| --- | --- |
| Web 开发 | react, nextjs, typescript, css, tailwind |
| 测试 | testing, jest, playwright, e2e |
| DevOps | deploy, docker, kubernetes, ci-cd |
| 文档 | docs, readme, changelog, api-docs |
| 代码质量 | review, lint, refactor, best-practices |
| 设计 | ui, ux, design-system, accessibility |
| 生产力 | workflow, automation, git |

## 高效搜索技巧

1. **使用特定关键词**：“react testing” 比单纯的 “testing” 更好
2. **尝试替代词**：如果 “deploy” 没结果，尝试 “deployment” 或 “ci-cd”
3. **检查热门来源**：许多技能来自 `vercel-labs/agent-skills` 或 `ComposioHQ/awesome-claude-skills`

## 未找到技能时

如果没有相关的技能存在：

1. 告知用户未找到匹配的现有技能
2. 提议使用你的通用能力直接帮助完成任务
3. 建议用户可以使用 `npx skills init` 创建自己的技能

示例：

```
我搜索了与 "xyz" 相关的技能，但没有找到匹配项。
不过我仍可以直接帮你完成这项任务！需要我开始吗？

如果这是你经常需要处理的事情，你也可以创建自己的技能：
npx skills init my-xyz-skill

```
