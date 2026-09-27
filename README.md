# skill

自建 Codex Skills。

## skill-visibility

在对话中提示主代理实际使用的技能。

- 项目内使用：`.agents/skills/skill-visibility/SKILL.md` 与根目录 `AGENTS.md` 共同生效。
- 所有项目使用：将该 `SKILL.md` 复制到 `$CODEX_HOME/skills/skill-visibility/SKILL.md`，并把本仓库 `AGENTS.md` 的规则合并到 `$CODEX_HOME/AGENTS.md`。
- 提示由模型指引实现，不是系统级技能调用事件。
