# Prompt Baselines

本目录保存角色 Prompt 基线文件。

这些 Prompt 不是简单的“执行说明”，而是包含：

- 项目定位
- 项目目标
- 整体方案与原因
- 角色职责
- 约束与禁止项
- 输出要求
- 质量标准

当前角色文件包括：

- `coordinator.md`
- `extractor.md`
- `compressor.md`
- `state_keeper.md`
- `auditor.md`

使用原则：

- 全部使用中文
- 每个角色在执行自己任务前，先理解项目全局目标
- Prompt 既要交代角色分工，也要交代为什么这么做
- 不把 Prompt 写成空泛原则或只有命令列表的薄说明
