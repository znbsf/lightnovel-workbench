# LightNovel Workbench

一个面向 `VS Code + WSL + Codex` 或其他 AI 写作助手的小说创作工作台。

它不是单篇小说成稿，而是一套可复用的方法论和项目结构，用来稳定管理：

- 点子库
- 基础文风
- 局部“佐料文风”
- 去 AI 味规则
- 中国网文平台摆盘适配
- 设定、纲要、正文、审校的分层协作

## 这个仓库适合做什么

- 用 AI 辅助长篇小说创作，但不想每次靠聊天记忆硬续写
- 想把文风、设定、伏笔和重写记录都项目化管理
- 想同时兼顾日轻翻译风写法、局部文风变调和中国网文平台阅读习惯
- 想把一套写作工作流长期复用到不同小说项目里

## 核心模块

- `00_inbox/ideas/`
  - 存放还没进入正典的点子、画面、关系火花和开场感
- `01_bible/style.md`
  - 定义全书最稳定的基础文风
- `01_bible/style_spices/`
  - 管理单章、单场、单段使用的局部“佐料风格”
- `01_bible/anti_ai.md`
  - 约束常见工业味和模板味
- `01_bible/plating_cn_webnovel.md`
  - 把同一内容适配成更适合中国网文平台的“摆盘”
- `03_outline/scene_cards/`
  - 用场景卡控制局部目标、冲突和节拍
- `05_review/`
  - 管理连续性、风格问题、未回收线索和重写任务

## 快速开始

1. 如果你现在只有一段文字、一个画面或一个模糊想法，先存进 `00_inbox/ideas/`
2. 再把稳定下来的点子提炼成 `01_bible/premise.md`、`01_bible/style.md`、`01_bible/taboo.md`
3. 在 `02_world/` 里建立角色、地点、组织和规则文件
4. 在 `03_outline/` 里写总纲、章节索引和场景卡
5. 写正文前先读 `style.md`、`anti_ai.md` 和当前场景相关文件
6. 写完后把问题记到 `05_review/`，把正典变更记到 `00_system/changelog.md`

## 仓库里已经包含

- 点子库模板
- 中文模板文件
- 多种 `style_spices` 示例
- 去 AI 味规则
- 中国网文平台摆盘指南
- 多组 demo、重写版和摆盘版对照

## 目录结构

```text
.
|-- AGENTS.md
|-- README.md
|-- .gitignore
|-- .vscode/
|   `-- settings.json
|-- 00_inbox/
|   `-- ideas/
|       |-- INDEX.md
|       |-- README.md
|       `-- TEMPLATE.md
|-- 00_system/
|   |-- workflow.md
|   |-- prompts.md
|   `-- changelog.md
|-- 01_bible/
|   |-- anti_ai.md
|   |-- premise.md
|   |-- plating_cn_webnovel.md
|   |-- style.md
|   |-- style_spices/
|   |   |-- README.md
|   |   `-- TEMPLATE.md
|   |-- themes.md
|   `-- taboo.md
|-- 02_world/
|   |-- timeline.md
|   |-- glossary.md
|   |-- characters/
|   |   `-- TEMPLATE.md
|   |-- locations/
|   |   `-- TEMPLATE.md
|   |-- factions/
|   |   `-- TEMPLATE.md
|   `-- rules/
|       `-- TEMPLATE.md
|-- 03_outline/
|   |-- master_outline.md
|   |-- chapter_index.md
|   |-- arc_01.md
|   `-- scene_cards/
|       `-- TEMPLATE.md
|-- 04_draft/
|   `-- volume_01/
|       |-- README.md
|       `-- chapter_01.md
`-- 05_review/
    |-- continuity.md
    |-- open_loops.md
    |-- style_issues.md
    `-- rewrite_tasks.md
```

## 使用方法

1. 还没成型的灵感、画面和关系火花，先放进 `00_inbox/ideas/`，不要直接写进正典文件。
2. 先填写 `01_bible/`，这里定义小说最稳定的核心身份。
3. 用 `01_bible/style.md` 固定全书基础文风，再用 `01_bible/style_spices/` 管理局部“佐料风格”。
4. 用 `01_bible/anti_ai.md` 约束“不要写出工业味”的常见错误。
5. 如果准备发布到中国网文平台，用 `01_bible/plating_cn_webnovel.md` 做平台适配。
6. 在 `02_world/` 中逐个建立世界设定文件，每个对象一个文件。
7. 把宏观剧情放在 `03_outline/` 中维护。
8. 只有当前场景卡准备好以后，再开始写正文。
9. 把问题记录在 `05_review/`，不要把零碎备注散落进正文里。

## 推荐写作流程

1. 更新 `03_outline/scene_cards/` 里的当前场景卡。
2. 如果这一场需要特殊风味，在场景卡里指定对应的 `style_spices` 文件和混合强度。
3. 先让 AI 产出 5 到 8 条场景节拍。
4. 确认节拍方向正确。
5. 再让 AI 只写这一场戏，或这一章中的一个片段。
6. 检查连续性、文风漂移和未回收线索。
7. 把影响正典的变更记录进 `00_system/changelog.md`。

## Git 建议

按章节、场景或修订轮次提交。小而清晰的提交更方便回溯实验版本，也更适合比较不同重写方案。
