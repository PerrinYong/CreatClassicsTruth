# CreatClassicsTruth

面向中国古典小说的高保真事实提取工程。

项目目标：

1. 生成不丢失关键情节信息的精简版纯文本
2. 生成机器可理解的 JSON 真相层
3. 生成可直接用于人物关系图、故事发展图、时间线快照图的数据层

当前工程采用文档驱动框架：

- `docs/项目书.md`：项目方案书
- `docs/执行框架.md`：执行框架
- `framework/`：结构契约、Prompt 基线、Runbook、校验与展示边界
- `workspace/`：通用模板工作区
- `journey-to-the-west/`：《西游记》小说工作空间
- `journey-to-the-west/xiyouji_txt/`：《西游记》原文章节源文本
- `journey-to-the-west/workspace/`：《西游记》实际运行工作区

执行原则：

- 单书立项
- 首轮逐章顺序推进
- 先抽取真相层，再生成精简文本
- 图数据从真相层和状态层派生
- 审计通过后再冻结章节结果

本地代码只承担：

- 数据格式校验
- 由结构化数据到图和 Web 展示的生成

不在本仓库中自研：

- LLM API 调用器
- Agent 编排器
- 工作流引擎

详情见 `docs/项目书.md` 与 `docs/执行框架.md`。
