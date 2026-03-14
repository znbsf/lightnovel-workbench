# Novel Project Rules

This repository is a fiction-writing workspace. Any AI agent working here should treat it as a continuity-sensitive project, not a generic chat session.

## Primary Goal

Help produce a coherent long-form novel while preserving canon, voice, pacing, and unresolved plot threads.

## Read Order Before Writing

Before drafting any new prose, read the smallest relevant context set:

1. `01_bible/premise.md`
2. `01_bible/style.md`
3. `01_bible/taboo.md`
4. Relevant files in `02_world/`
5. Relevant outline files in `03_outline/`
6. The latest draft section in `04_draft/`
7. `05_review/open_loops.md` if the scene touches a mystery or setup

## Drafting Rules

1. Do not invent new world rules unless explicitly asked.
2. Do not resolve a major mystery earlier than the outline allows.
3. Keep point of view, tense, and tone consistent with `01_bible/style.md`.
4. When asked to continue a chapter, first propose scene beats unless the user asks for direct drafting.
5. Prefer one scene at a time over full-chapter generation.
6. If continuity is uncertain, flag it before writing.

## Revision Rules

1. Separate line-level polish from structural rewrite.
2. When revising, preserve canon facts unless the user requests a retcon.
3. Record meaningful canon changes in `00_system/changelog.md`.
4. Record dangling clues, contradictions, and callback obligations in `05_review/`.

## File Discipline

1. Keep one major subject per file.
2. Prefer updating the correct reference file instead of burying canon in draft prose.
3. Use scene cards to control local intent before writing long passages.

## Default Assistance Modes

- Brainstorming: offer multiple options with tradeoffs.
- Drafting: write to the current scene card and style guide.
- Continuity check: compare draft text against world files and outline.
- Rewrite: explain what changes in rhythm, clarity, and subtext.
