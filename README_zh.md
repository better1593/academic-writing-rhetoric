# Academic Writing Rhetoric Skill

`academic-writing-rhetoric` 是一个 AI agent skill，主要用于博士论文、学术论文和章节级的**英语**学术写作和修改润色。它是由我在上我们学校 PhD Thesis Writing 课程中，根据课堂材料和写作训练内容蒸馏整理而成。

请注意：这个skill不是用来代写研究内容的。它的作用是帮你诊断写作中的逻辑、结构与修辞问题，优化章节衔接，调整学术语气，并支持在负责任的前提下，用 AI 辅助提升文字表达——同时完全保留你的研究观点、证据、引用和个人风格。



English documentation: [README.md](README.md)

## 平台兼容性

这个 skill 的可移植核心是：

```text
academic-writing-rhetoric/
|-- SKILL.md
`-- references/
```

`agents/openai.yaml` 只是给兼容 OpenAI/Codex 的环境使用的可选元数据。Claude Code 不需要它；它也不会让这个 skill 变成 OpenAI 专属。Claude Code 和其他 agent 可以直接使用同一份 `SKILL.md` 和 `references/`。

## 安装方法

很多 AI coding 或 writing agent 可以通过仓库链接自动安装。通常可以直接对 agent 说：

```text
Please install this repository as an AI agent skill.
The installable skill folder is academic-writing-rhetoric/.
```

如果需要手动安装，可以 clone 仓库，然后把 `academic-writing-rhetoric` 文件夹复制到相应 agent 的 skills 目录。

### Codex

Codex 的 skill 一般放在 Codex skills 目录下。如果设置了 `CODEX_HOME`，可使用 `$CODEX_HOME/skills`；否则通常是 `~/.codex/skills`。


### Claude Code

Claude Code 支持 personal skills 和 project skills。Personal skill 放在：

```text
~/.claude/skills/<skill-name>/SKILL.md
```

Project skill 放在：

```text
.claude/skills/<skill-name>/SKILL.md
```


如果安装后 agent 没有立刻识别 skill，可以重启当前 agent 会话。


## 目录结构

```text
academic-writing-rhetoric/
|-- SKILL.md
|-- agents/
|   `-- openai.yaml
`-- references/
    |-- abstract.md
    |-- academic-language-and-cohesion.md
    |-- conclusion.md
    |-- discussion.md
    |-- genai-writing-integrity.md
    |-- introduction.md
    |-- literature-review-and-related-work.md
    |-- methods-and-methodology.md
    |-- results-and-findings.md
    |-- revision-and-final-polish.md
    `-- whole-paper-and-thesis-workflow.md
```

- `SKILL.md`: skill 的核心说明，包括触发场景、工作规则和 reference 分发。
- `agents/openai.yaml`: 兼容 OpenAI/Codex 环境的可选元数据。
- `references/`: 各章节和写作任务的详细参考资料，按需加载。

## 功能和定位

这个 skill 适合用于：

- 诊断章节功能缺失，例如 gap 不清、review 太像 annotated bibliography、discussion 只重复 results；
- 设计论文或章节大纲；
- 修改 introduction、literature review、methods、results、discussion、conclusion、abstract；
- 改善 cohesion、stance、hedging、reporting verbs 和 academic register；
- 检查 aim、research questions、methods、findings 和 claims 是否对齐；
- 记录和控制负责任的 AI 辅助写作；
- 在不改变研究含义、证据、引用和 claim strength 的前提下润色语言。

它的定位是 academic writing rhetoric coach，而不是完整论文流水线。它不能替代文献检索、同行评审、统计分析、引用核验或学校正式格式要求。

## 使用方法

可以明确要求 AI agent 使用这个 skill：

```text
请使用 academic-writing-rhetoric skill 诊断我的 introduction。
重点看 research gap、aim、contribution 和章节逻辑。
```

```text
请用这个 skill 修改我的 literature review 段落。
保留引用，不要新增文献或研究结论。
```

```text
请检查我的 discussion 是否只是重复 results，以及 implication 是否有证据支持。
```

常用模式包括：

- `diagnose`: 识别高影响的修辞、结构和 cohesion 问题。
- `outline`: 搭建章节或 section 结构。
- `draft`: 基于使用者提供的 claims、evidence、citations 和限制条件起草。
- `revise`: 在保留含义和证据的前提下改写。
- `polish`: 改善 register、cohesion、stance 和 sentence flow。

## 个性化你的 Skill

`references/` 中包含很多 academic language、短语、词汇、reporting verbs、transition patterns、hedging forms 和章节句式。后续你可以把它逐渐发展成自己的学术语料库。

例如，在读文献或修改自己文章时，可以让 AI agent 这样做：

```text
我在读文献时觉得这些表达适合我的写作风格。
请把它们整理成通用句式，加入 academic-writing-rhetoric 中最合适的 reference 文件。
不要加入整段原文，只保留可复用的 phrase pattern。
```

```text
请把这些 discussion 中表达 implication 的短语加入 references/discussion.md。
按照 implication、limitation、contribution 分类整理，保持通用、简洁、可复用。
```

个性化建议：

- 加入短语、句式、词汇搭配，不要加入大段原文。
- 尽量保留通用表达，除非是你自己领域中稳定使用的术语。
- 按章节放入对应 reference 文件。
- 删除不符合你写作风格的表达。
- 当 phrasebank 变大时，让 AI 帮你重新分类整理。
- 尽量区分领域术语和通用写作技巧。

目标是让这个 skill 慢慢贴近你的写作偏好：更谨慎或更有主张，更简洁或更解释性，更偏理论或更偏应用。这会让 AI agent 在修改你的文本时，更像是在延续你的 academic voice，而不是套用普通模板。

## 注意事项

- 不要让 skill 虚构引用、数据、方法、结果或创新点。
- 学校、期刊、学院或出版社的格式要求必须以当前官方规则为准。
- AI 修改建议应作为写作反馈，而不是自动正确答案。
- 如果从已发表论文中吸收表达，建议只保留短语模式和可泛化句式，避免复制受版权保护的长文本。
