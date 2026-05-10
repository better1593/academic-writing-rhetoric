# Academic Writing Rhetoric Skill

`academic-writing-rhetoric` is an AI agent skill mainly for PhD thesis writing, research articles, and section-level **English** academic writing, revision, and polishing. It was distilled from my university PhD Thesis Writing course materials and writing practice notes.

Please note: this skill is not designed to ghostwrite research content. Its purpose is to help diagnose logic, structure, and rhetorical problems in academic writing, improve section transitions, calibrate academic tone, and support responsible AI-assisted improvement of expression while fully preserving the user's research ideas, evidence, citations, and personal style.

Chinese documentation: [README_zh.md](README_zh.md)

## Platform Compatibility

The portable core of this skill is:

```text
academic-writing-rhetoric/
|-- SKILL.md
`-- references/
```

The optional `agents/openai.yaml` file provides metadata for compatible OpenAI/Codex environments. It is not required for Claude Code, and it does not make the skill OpenAI-exclusive. Claude Code and other agents can use the same `SKILL.md` and `references/` files.

## Installation

Many AI coding or writing agents can install a skill if you give them the repository URL and ask them to install the `academic-writing-rhetoric/` folder as an agent skill:

```text
Please install this repository as an AI agent skill.
The installable skill folder is academic-writing-rhetoric/.
```

If manual installation is needed, clone the repository and copy the `academic-writing-rhetoric` folder into your agent's skills directory.

### Codex

For Codex, place the skill folder under your Codex skills directory. If `CODEX_HOME` is set, use `$CODEX_HOME/skills`; otherwise the usual location is `~/.codex/skills`.

### Claude Code

Claude Code supports both personal and project skills. Personal skills are placed under:

```text
~/.claude/skills/<skill-name>/SKILL.md
```

Project skills are placed under:

```text
.claude/skills/<skill-name>/SKILL.md
```

If the skill is not detected immediately, restart the agent session.

## Directory Structure

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

- `SKILL.md`: main skill instructions, trigger conditions, working rules, and reference dispatch.
- `agents/openai.yaml`: optional metadata for compatible OpenAI/Codex environments.
- `references/`: section-specific writing guidance loaded only when needed.

## What This Skill Does

This skill helps with:

- diagnosing weak academic writing by rhetorical function;
- building outlines for thesis chapters and article sections;
- revising introductions, literature reviews, methods, results, discussions, conclusions, and abstracts;
- improving cohesion, stance, hedging, reporting verbs, and academic register;
- checking whether aims, research questions, methods, findings, and claims are aligned;
- documenting and controlling responsible AI-assisted writing;
- polishing text while preserving meaning, evidence, citations, and claim strength.

It is best used as a writing-quality and rhetoric layer. It does not replace literature search, peer review, statistical analysis, citation verification, or institutional formatting rules.

## How To Use

Ask your AI agent to use the skill explicitly:

```text
Use the academic-writing-rhetoric skill to diagnose this Introduction.
Focus on research gap, aim, contribution, and section flow.
```

```text
Use this skill to revise my Literature Review paragraph.
Preserve citations and do not add new claims.
```

```text
Use academic-writing-rhetoric to check whether my Results section over-interprets the findings.
```

Useful modes include:

- `diagnose`: identify high-impact rhetorical and cohesion problems.
- `outline`: build a section or chapter structure.
- `draft`: draft from user-provided claims, evidence, citations, and constraints.
- `revise`: rewrite while preserving meaning and evidence.
- `polish`: improve register, cohesion, stance, and sentence flow.

## Personalization

The references include examples of academic language, phrase patterns, reporting verbs, transition patterns, hedging forms, and section-specific sentence frames. Over time, you can turn this skill into your own academic phrasebank.

For example, while reading papers or revising your own writing, you can ask your AI agent:

```text
I like these sentence patterns from my reading notes.
Please add them to the most relevant reference file in academic-writing-rhetoric
as reusable phrase patterns, not as copied source text.
```

```text
Please add these discussion implication phrases to references/discussion.md.
Group them under implications, limitations, or contribution as appropriate.
Keep them general and reusable.
```

Good personalization principles:

- Add short phrase patterns, not long copied passages.
- Keep examples generic unless they are your own reusable terminology.
- Place phrases in the relevant chapter reference file.
- Remove wording that does not match your preferred academic voice.
- Ask the agent to reorganize phrase lists when they grow too large.
- Keep your field-specific vocabulary separate from general writing rules when possible.

The goal is for the skill to gradually learn your preferred academic voice: cautious or assertive, concise or explanatory, theory-heavy or application-oriented, depending on your discipline and writing habits.

## Notes

- Do not ask the skill to invent citations, data, methods, findings, or novelty claims.
- Always verify local thesis, journal, department, or publisher formatting rules.
- Treat suggested revisions as writing feedback, not automatic truth.
- If you add phrases from published papers, keep them as short reusable patterns and avoid copying protected text.
