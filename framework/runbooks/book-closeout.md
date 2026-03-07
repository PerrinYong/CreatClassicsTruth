# Book Closeout Runbook

适用于全书逐章完成后的收束阶段。

主要工作：

1. 拼接并轻量统一所有 `chapter_retelling.txt`
2. 生成 `book_retelling.txt`
3. 输出 `entity_registry.json`
4. 输出 `relation_history.json`
5. 输出 `object_history.json`
6. 输出 `timeline_snapshots.json`
7. 输出 `story_flow_graph.json`
8. 输出 `open_threads_report.json`
9. 输出 `book_audit_report.json`

注意：

- 不重新从整本原文生成全书文本
- 优先基于已审计通过的章节产物做收束
- 收束结果仍需通过一致性检查
