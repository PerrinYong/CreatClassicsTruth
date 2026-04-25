# Classics Truth Team

`classics-truth-team` 是为本仓库“名著事实提取项目”设计的 CrewBee 文件型 Agent Team。

## 目标

按章节顺序处理单本中国古典小说，生成：

1. 不丢失关键情节信息的精简复述
2. 机器可理解的 JSON 真相层
3. 可绘制人物关系图、故事发展图和时间线快照的数据层

## 角色

- `classics-truth-leader`：默认入口，持有主线、调度角色、决定冻结。
- `source-reader`：只读定位原文、状态和证据锚点。
- `truth-extractor`：生成 `chapter_truth.json`。
- `retelling-compressor`：基于 truth 生成 `chapter_retelling.txt`。
- `state-graph-keeper`：更新 `book_state.json` 并派生图数据。
- `faithfulness-auditor`：冻结前忠实性审计。

## 工作区约定

- 根目录 `workspace/` 是模板工作区。
- 实际运行应使用书籍目录下的 `workspace/`。
- 当前《西游记》的实际工作区是 `journey-to-the-west/workspace/`。
- 当前《西游记》的原文目录是 `journey-to-the-west/xiyouji_txt/`。

## CrewBee 注册示例

把本目录复制或链接到 OpenCode 配置目录下的 `teams/classics-truth-team/`，然后在 `crewbee.json` 中加入：

```json
{
  "teams": [
    { "id": "coding-team", "enabled": true, "priority": 0 },
    { "path": "@teams/classics-truth-team", "enabled": true, "priority": 1 }
  ]
}
```

`path` 必须指向包含 `team.manifest.yaml` 的目录，而不是某个单独文件。
