# Keep Workspace Tidy

给 Codex 用的 Skill。修代码、排障或打包时，默认原地修改，把临时文件放到工作区外，并在交付前检查新增文件。

## 使用

把 `keep-workspace-tidy` 文件夹放到 `~/.agents/skills/`，或放进目标项目的 `.agents/skills/`。在 Codex 的任务提示里写 `$keep-workspace-tidy` 即可明确调用。

```text
$keep-workspace-tidy 帮我修复报告导出。直接改现有代码，按项目约定验证，把最终交付物放在现有输出目录。
```

修一个普通配置项时，直接编辑原文件并检查 diff。需要回滚的生产迁移按项目约定保存必要备份。清理旧备份属于单独的任务，执行前先明确清理范围。
