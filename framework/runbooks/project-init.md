# Project Initialization Runbook

目标：建立单书工程规则与初始状态。

初始化时需要固定：

- `book_id`
- 章节列表
- `chapter_id` 规则
- 事件 ID 规则
- 快照 ID 规则
- 关系类型表
- 物品流转类型表
- 环境约束表达规范
- 状态变化字段规范
- 输出文件清单

初始化后至少应具备：

- `workspace/state/book_state.json`
- `framework/contracts/*.schema.json`
- `framework/prompts/*.md`
- `workspace/checkpoints/_template/`

完成标准：

- 当前书的工作状态可进入第一章
- 文件命名和目录约定已固定
- 审计与冻结规则已确定
