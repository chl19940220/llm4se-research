---
name: ccfa-paper-writing
description: Use when writing or revising CCF-A-oriented software engineering research papers, including LaTeX manuscript text, motivation, introduction, related work, method description, evaluation narrative, claim-evidence alignment, and paper-ready academic wording.
---

# CCF-A Paper Writing

## Scope

Use this skill for writing and revising software engineering research papers targeting high-quality venues such as FSE, ASE, ICSE, ISSTA, TSE, TOSEM, OOPSLA, PLDI, and related venues.

Typical tasks include:

- drafting or revising introduction, motivation, related work, method, evaluation, discussion, or limitation sections
- improving paper story, contribution framing, and section logic
- aligning claims with evidence
- turning notes, experimental results, or method sketches into paper-ready text
- improving academic wording without overstating novelty or results
- producing LaTeX-compatible manuscript text

Do not use this skill for broad literature search, single-paper deep reading, rebuttal drafting, or raw metric verification unless the user explicitly asks for writing-oriented synthesis.

## Output Language

Default to English for manuscript text, section drafts, revisions, and paper-ready wording.

If the user discusses the task in Chinese, explain briefly in Chinese if useful, but produce the main manuscript content in English unless the user explicitly requests Chinese.

## LaTeX Writing Rules

When drafting or revising manuscript text, produce LaTeX-compatible output by default.

- Preserve existing LaTeX commands, labels, citations, macros, and section structure unless the user asks to change them.
- Use existing citation commands from the local manuscript, such as `\cite{}`, `\citep{}`, `\citet{}`, or project-specific commands.
- Do not invent citation keys, labels, macros, figure names, table names, theorem names, or algorithm names.
- Use LaTeX syntax for references to figures, tables, sections, equations, algorithms, and listings when the local manuscript uses them.
- Escape LaTeX-sensitive characters when needed: `%`, `_`, `&`, `#`.
- Do not wrap normal prose in Markdown when the output is intended to be pasted into a `.tex` file.
- Keep math notation consistent with the surrounding manuscript.
- Inspect nearby manuscript text before choosing citation commands, cross-reference commands, terminology, capitalization, notation, and section naming.

Use common cross-reference forms only when they match the local manuscript style:

- `Section~\ref{sec:name}`
- `Figure~\ref{fig:name}`
- `Table~\ref{tab:name}`
- `Equation~\ref{eq:name}`
- `Algorithm~\ref{alg:name}`
- `Listing~\ref{lst:name}`

If a citation key or label is needed but not available, use a clear placeholder such as `[citation needed: paper title]` or `[label needed: target]` rather than inventing one.
