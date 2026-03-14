# 小说项目模板

这个工作区是一套适用于 `VS Code + WSL + Codex` 或其他 AI 写作助手的长篇小说模板。

## 目录结构

```text
.
|-- AGENTS.md
|-- README.md
|-- .gitignore
|-- .vscode/
|   `-- settings.json
|-- 00_system/
|   |-- workflow.md
|   |-- prompts.md
|   `-- changelog.md
|-- 01_bible/
|   |-- premise.md
|   |-- style.md
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

1. 先填写 `01_bible/`，这里定义小说最稳定的核心身份。
2. 在 `02_world/` 中逐个建立世界设定文件，每个对象一个文件。
3. 把宏观剧情放在 `03_outline/` 中维护。
4. 只有当前场景卡准备好以后，再开始写正文。
5. 把问题记录在 `05_review/`，不要把零碎备注散落进正文里。

## 推荐写作流程

1. 更新 `03_outline/scene_cards/` 里的当前场景卡。
2. 先让 AI 产出 5 到 8 条场景节拍。
3. 确认节拍方向正确。
4. 再让 AI 只写这一场戏，或这一章中的一个片段。
5. 检查连续性、文风漂移和未回收线索。
6. 把影响正典的变更记录进 `00_system/changelog.md`。

## Git 建议

按章节、场景或修订轮次提交。小而清晰的提交更方便回溯实验版本，也更适合比较不同重写方案。
