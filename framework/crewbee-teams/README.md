# CrewBee Teams

本目录保存按 CrewBee 文件型 Team 格式编写的项目团队定义。

CrewBee Team 目录约定：

```text
<team-dir>/
  team.manifest.yaml
  team.policy.yaml
  *.agent.md
  TEAM.md
```

当前 Team：

- `classics-truth-team/`：名著事实提取、精简复述、状态维护、图数据派生与忠实性审计 Team。

注意：

- `*.agent.md` 必须和 `team.manifest.yaml`、`team.policy.yaml` 放在同一目录根部。
- 若要让 CrewBee 加载该 Team，需要把目录复制/链接到 OpenCode 配置目录的 `teams/` 下，并在 `crewbee.json` 中注册。
