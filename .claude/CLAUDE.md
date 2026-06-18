Skills 按照文件夹归类在 `skills/` 目录下：

- `engineering/` —— 日常代码工作

- `productivity/` —— 日常非代码工作流程工具

- `misc/` —— 保留但很少使用

- `personal/` —— 与个人环境相关，不予推广

- `in-progress/` —— 尚未就绪的草稿

- `deprecated/` —— 不再使用

`engineering/`、`productivity/` 或 `misc/` 中的每个 skill 都必须在顶层 `README.md` 中有引用，并在 `.claude-plugin/plugin.json` 中有条目。`personal/`、`in-progress/` 和 `deprecated/` 中的 skill 不得出现在上述任一文件中。

顶层 `README.md` 中的每个 skill 条目必须将 skill 名称链接到其 `SKILL.md`。

每个 bucket 文件夹下都有一个 `README.md`，列出该 bucket 中的所有 skill，并附上一行描述，其中 skill 名称链接到其 `SKILL.md`。