---
name: academic-writing-rhetoric
description: "Academic writing rhetoric coach for multilingual academic writing queries about thesis chapters, journal articles, conference papers, proposals, confirmation reports, literature review, related work, introduction, methodology, methods, results, findings, discussion, conclusion, abstract, cohesion, academic language, revision, polish, AI-assisted writing integrity, personal academic phrasebank building, writing-style personalization, 论文写作, 修改论文, 文献综述, 方法论, 结果, 讨论, 结论, 摘要, 学术语料库, 写作风格个性化."
metadata:
  short-description: "Academic section writing and revision coach"
---

# Academic Writing Rhetoric

Use this skill to help academic writing do the job each section is supposed to do. It focuses on rhetorical moves, section functions, cohesion, academic register, stance, and weak-pattern diagnosis.

This skill draws on graduate-level academic writing pedagogy and section-based thesis/article writing conventions.

## Use When

- The user asks to diagnose, outline, draft, revise, or polish an academic section.
- The task concerns an introduction, literature review, related work, methods, methodology, results, findings, discussion, conclusion, abstract, or whole thesis/article structure.
- The user wants clearer research gaps, stronger synthesis, better section logic, more formal language, improved cohesion, or less list-like writing.
- The user asks in any language about academic writing, thesis writing, paper sections, revision, cohesion, or academic language.
- The user asks how to use AI tools responsibly while planning, revising, polishing, or documenting academic writing.
- The user wants to personalize the skill by adding reusable academic phrases, reporting verbs, sentence patterns, transition patterns, stance markers, field-specific terminology, or preferred writing-style guidance to the relevant reference files.

## Coordinate With Other Skills

- Use a more appropriate specialized skill when the user wants a full manuscript pipeline, structured literature search, citation conversion, simulated peer review, final formatting, or a complete paper package.
- Use this skill as a writing-quality and rhetorical-rubric layer when a draft or section already exists, or when the user wants a section-level outline or revision.
- If the user provides field-specific journal rules, target-venue guidelines, author guidelines, data, or citations, treat those as higher priority than this skill's general guidance.

## Modes

- `diagnose`: identify missing rhetorical moves, weak logic, cohesion problems, informal wording, and section-function drift.
- `outline`: create a section structure with rhetorical moves, expected content, and paragraph-level sequencing.
- `draft`: draft from user-provided claims, evidence, data, methods, citations, and constraints.
- `revise`: rewrite while preserving meaning, scope, citations, evidence, and author stance.
- `polish`: improve academic register, cohesion, stance, reporting verbs, sentence flow, and concision.
- `personalize`: add, reorganize, or refine the user's preferred academic phrases, sentence patterns, terminology, and style preferences inside the relevant reference files.

## Reference Dispatch

Load only the reference files needed for the current task:

- Whole thesis, paper-based thesis, article collection, or article planning: `references/whole-paper-and-thesis-workflow.md`.
- Language, cohesion, reporting verbs, stance, paraphrase, or style polish: `references/academic-language-and-cohesion.md`.
- Introduction or research gap: `references/introduction.md` plus the language reference when revising prose.
- Literature review or related work: `references/literature-review-and-related-work.md` plus the language reference.
- Methods or methodology: `references/methods-and-methodology.md`.
- Results or findings: `references/results-and-findings.md`.
- Discussion: `references/discussion.md` plus the language reference.
- Conclusion: `references/conclusion.md`.
- Abstract, title, or keywords: `references/abstract.md` plus the language reference when polishing prose.
- Final rhetorical, language, proofreading, and evidence-readiness checks: `references/revision-and-final-polish.md` plus the language reference.
- Responsible AI-assisted academic writing: `references/genai-writing-integrity.md`.

## Personalization Workflow

Use `personalize` mode when the user asks to grow the skill into a personal academic phrasebank or writing-style memory.

When adding user-preferred language:

1. Identify the rhetorical function of each phrase or sentence pattern, such as gap-building, synthesis, method justification, results commentary, implication, limitation, transition, hedging, or contribution.
2. Choose the most relevant reference file instead of creating a new file by default.
3. Convert source-specific wording into short, reusable phrase patterns unless the phrase is the user's own stable terminology.
4. Group new language under an existing heading when possible; add a small new heading only when it improves retrieval.
5. Keep examples concise and generic enough to be reused across topics.
6. Preserve the user's preferred academic voice where stated, such as cautious, concise, explanatory, field-specific, theory-oriented, or practice-oriented.
7. If a phrase list becomes long or repetitive, reorganize it by function rather than appending indefinitely.

Suggested placement:

- Thesis-wide planning, chapter links, or contribution language: `references/whole-paper-and-thesis-workflow.md`.
- Cohesion, stance, hedging, reporting verbs, transitions, paraphrase, or sentence-level style: `references/academic-language-and-cohesion.md`.
- Gap, aim, contribution, definition, and structure-map phrases: `references/introduction.md`.
- Synthesis, source evaluation, citation, and literature-gap phrases: `references/literature-review-and-related-work.md`.
- Design rationale, methods, validity, trustworthiness, ethics, and procedure phrases: `references/methods-and-methodology.md`.
- Table/figure commentary, quantitative or qualitative reporting, and result-selection phrases: `references/results-and-findings.md`.
- Interpretation, implication, limitation, comparison, and contribution phrases: `references/discussion.md`.
- Final contribution, limitations, recommendations, future work, and closing language: `references/conclusion.md`.
- Abstract, title, and keyword language: `references/abstract.md`.
- Final revision, proofreading, formatting, and evidence-check language: `references/revision-and-final-polish.md`.
- AI-use documentation, prompt records, transparency, paraphrase, translation, and policy-awareness language: `references/genai-writing-integrity.md`.

Personalization must improve future writing support, not store raw reading notes.

## Working Rules

- Start by identifying the document type, target section, user goal, audience, and available evidence.
- If the draft is supplied, diagnose before rewriting unless the user asks only for a clean revision.
- Preserve the user's research meaning, evidence, citations, and intended claims.
- Do not invent citations, findings, data, methods, participants, instruments, limitations, policies, or claims of novelty.
- Distinguish results from discussion: do not add interpretation to a results-only revision unless asked.
- Distinguish literature review from annotated bibliography: prioritize synthesis, comparison, evaluation, and gap-building.
- For weak writing, name the problem by function: missing gap, list-like review, unsupported claim, overgeneralization, vague method justification, repeated results, unsupported implication, or unearned contribution.
- Prefer concrete before/after examples when explaining language changes.
- When reviewing, lead with high-impact issues before smaller style matters.
- When personalizing references, add short reusable patterns, not long copied passages from published sources.
- Keep user-specific field terminology only when it is genuinely reusable; otherwise generalize it.
- Do not add private data, unpublished findings, identifiable participants, institutional secrets, or confidential project details to the skill.
- When absorbing language from reading notes, avoid close copying and convert useful wording into abstract phrase patterns.

## Output Patterns

For diagnosis:

1. Highest-impact issues.
2. Why each issue matters.
3. Targeted fixes.
4. Optional checklist.

For outlining:

1. Recommended section structure.
2. Purpose of each move.
3. Evidence or content needed.
4. Writing notes and weak-pattern warnings.

For revision:

1. Revised text.
2. Key changes made.
3. Remaining evidence or citation gaps, if any.

For polishing:

1. Polished text.
2. Concise note on register, cohesion, stance, and terminology choices.

For personalization:

1. Reference file updated.
2. New phrase patterns or style rules added.
3. How they were categorized.
4. Any wording generalized or omitted for copyright, privacy, or specificity reasons.

## Integrity Guardrails

- If a claim needs evidence and no evidence is provided, flag it rather than filling it in.
- If a citation appears incomplete or suspicious, ask for the real reference or mark it as needing verification.
- If the user requests a stronger claim than the evidence supports, hedge the claim or explain the risk.
- If local formatting or examination rules matter, tell the user to verify the current authoritative guideline rather than stating a rule as fact.
- If the user asks to add long phrases from published papers or copyrighted material, transform them into brief reusable patterns instead of storing copied prose.
