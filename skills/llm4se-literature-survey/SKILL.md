---
name: llm4se-literature-survey
description: Use when conducting multi-paper literature surveys for LLM4SE software engineering research, including related-work mapping, paper filtering, venue and publication-status checking, method taxonomy, benchmark comparison, and research-gap synthesis.
---

# LLM4SE Literature Survey

## Scope

Use this skill for multi-paper literature survey tasks in LLM4SE research.

Typical tasks include:

- finding relevant papers in an LLM4SE subarea
- filtering papers by venue, publication status, topic fit, benchmark, or time range
- organizing papers into a taxonomy
- comparing methods, datasets, metrics, baselines, and artifacts
- identifying research gaps for a manuscript or future project
- checking whether papers are formal CCF-A/high-quality venue publications or only preprints

Do not use this skill for single-paper deep reading, manuscript rewriting, rebuttal drafting, or detailed metric verification unless the user explicitly asks for a literature-survey view.

## Output Language

Default to English for all survey outputs, tables, summaries, and research-gap analysis.

## First Step

Clarify or infer the survey target:

- research area or keyword set
- venue scope, such as CCF-A, FSE, ASE, ICSE, ISSTA, TSE, TOSEM, OOPSLA, PLDI, or relevant AI/NLP venues
- time range, if relevant
- required benchmark, dataset, task, method family, or artifact type
- output purpose: related work, topic discovery, citation support, venue filtering, or metric comparison

If local materials are available, inspect them first:

- manuscript sections
- bibliography files
- notes
- paper lists
- reviewer comments
- experiment tables
- prior survey documents

## Core Workflow

1. Build a candidate paper set from user-provided sources, local files, and external search.
2. Filter papers by topic fit, publication status, venue quality, and relevance to the user's research question.
3. Separate confirmed formal publications from arXiv/preprints, technical reports, workshop papers, and unpublished repositories.
4. Extract comparable information: problem, method, benchmark, metrics, baselines, artifacts, and relationship to the user's work.
5. Organize papers into a taxonomy based on research problem, technical approach, interaction pattern, or evaluation setting.
6. Synthesize gaps cautiously, using evidence from the surveyed papers rather than broad unsupported claims.
7. Produce output that can be reused in related work, research notes, or paper planning.

## Evidence Discipline

- Do not invent papers, venues, authors, claims, metrics, datasets, baselines, tools, or experimental results.
- When publication status matters, verify it using authoritative sources rather than relying only on discovery tools.
- When a paper is only available as arXiv/preprint or has uncertain status, label it clearly.
- When evidence is insufficient, state the uncertainty and avoid overstating the claim.
- For citation support, match each claim to the most specific paper. If one paper cannot support the whole sentence, split or soften the sentence.

## References

Read `references/venue-scope.md` when the task asks for CCF-A/high-quality venue filtering, formal publication status, or papers from venues such as FSE, ASE, ICSE, ISSTA, TSE, TOSEM, OOPSLA, PLDI, NeurIPS, ICML, ICLR, ACL, EMNLP, AAAI, IJCAI, or related SE/PL/AI venues.

## Preferred Output Formats

For paper filtering:

| Paper | Venue/Status | Task | Method | Dataset/Benchmark | Metrics | Relevance | Notes |
|---|---|---|---|---|---|---|---|

For taxonomy:

| Category | Representative Papers | Shared Idea | Difference | Limitation |
|---|---|---|---|---|

For related-work support:

| Claim | Best Supporting Paper | Evidence | Caveat |
|---|---|---|---|

For gap synthesis:

| Prior Work Cluster | What It Solves | What Remains Weak | Opportunity |
|---|---|---|---|
