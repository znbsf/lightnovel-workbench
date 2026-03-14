# 工作流

## 稳定的真相优先级

`00_inbox/ideas/` 是灵感池，不属于正典真相来源。

当不同文件互相冲突时，按下面的优先级判断：

1. `01_bible/`
2. `02_world/`
3. `03_outline/`
4. `04_draft/`
5. `05_review/`

如果正文和既有正典冲突，要么修改正文，要么把这次重设明确记录到 `00_system/changelog.md`。

## 点子处理

1. 新点子先存到 `00_inbox/ideas/`。
2. 点子阶段允许矛盾、允许不完整、允许只有气味和画面。
3. 只有在点子被采纳后，才把它拆进 `01_bible/`、`02_world/` 或 `03_outline/`。
4. 点子升格为正典时，要把影响记录到 `00_system/changelog.md`。

## 上下文包

不要每次都把整个项目喂给 AI，优先使用紧凑的上下文包。

### 上下文包：点子整理

- 用户刚给出的原始文字
- `00_inbox/ideas/TEMPLATE.md`
- `01_bible/style.md`
- 如有需要，再加入 `01_bible/style_spices/` 中相关风味文件

### 上下文包：点子升格

- 当前点子文件
- `01_bible/premise.md`
- `01_bible/themes.md`
- `01_bible/style.md`
- 相关人物或世界设定文件
- 当前总纲文件

### 上下文包：新场景起草

- `01_bible/premise.md`
- `01_bible/style.md`
- `01_bible/anti_ai.md`
- 如果目标是平台连载，再加入 `01_bible/plating_cn_webnovel.md`
- 如果场景卡指定了局部风味，再加入对应的 `01_bible/style_spices/*.md`
- 当前相关人物文件
- 当前相关地点文件
- 当前分幕文件
- 当前场景卡
- 正文中前一段 500 到 1500 字

### 上下文包：连续性检查

- 当前章节正文
- `02_world/timeline.md`
- 相关人物文件
- `03_outline/chapter_index.md`
- `05_review/open_loops.md`

### 上下文包：文风校正

- `01_bible/style.md`
- `01_bible/anti_ai.md`
- 如果目标是平台连载，再加入 `01_bible/plating_cn_webnovel.md`
- 如果当前段落使用了局部风味，再加入对应的 `style_spices` 文件
- 正文中 2 到 3 段质量较高的参考段落
- 需要修正的段落

### 上下文包：平台摆盘

- `01_bible/style.md`
- `01_bible/anti_ai.md`
- `01_bible/plating_cn_webnovel.md`
- 当前章节正文
- 当前场景卡

### 上下文包：风味设计

- `01_bible/style.md`
- 目标章节或场景卡
- 你想致敬或借用的作品特征说明
- `01_bible/style_spices/TEMPLATE.md`

## 每日循环

1. 如果有新点子，先决定它是暂存到 `00_inbox/ideas/`，还是已经可以升格为正典。
2. 明确下一场戏的目标。
3. 判断这一场是否需要局部风味。
4. 如有需要，创建或指定对应的 `style_spices` 文件。
5. 更新场景卡。
6. 生成节拍。
7. 起草正文。
8. 做一次连续性检查。
9. 做一次文风检查。
10. 做一次反工业味检查。
11. 如果准备发布，再做一次平台摆盘检查。
12. 记录新增的义务、线索和正典决定。

## 变更控制

正文写在草稿里。  
正典决定写进核心设定目录或世界设定目录。  
例外和问题记录在审校目录里。
