# Novel Project Template

This workspace is a reusable long-form fiction template for `VS Code + WSL + Codex` or any other AI writing assistant.

## Structure

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

## How To Use

1. Fill out `01_bible/` first. This is the stable identity of the novel.
2. Build the world in `02_world/` as one-file-per-entity.
3. Keep the macro plot in `03_outline/`.
4. Draft only after the current scene card is ready.
5. Track problems in `05_review/` instead of scattering notes through the draft.

## Recommended Writing Loop

1. Update the current scene card in `03_outline/scene_cards/`.
2. Ask the AI to produce 5 to 8 scene beats.
3. Confirm the beats.
4. Ask the AI to draft only that scene or chapter section.
5. Review continuity, style drift, and unresolved clues.
6. Record any canon changes in `00_system/changelog.md`.

## Git Tip

Commit by chapter, scene, or revision pass. Small commits make it much easier to recover experiments and compare rewrites.
