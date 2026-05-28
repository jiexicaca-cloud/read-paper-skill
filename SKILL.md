---
name: read-paper
description: Deeply read, summarize, critique, and organize academic research papers from PDF or text, especially neuroscience and adjacent scientific papers. Use when the user asks to read a paper, summarize an academic paper, analyze a neuroscience article, create reading notes, extract methods/results/limitations, critique evidence, explain a paper's formula/figure/table/experiment, or answer follow-up questions about a previously discussed paper.
---

# Read Paper

## Purpose

Produce systematic, in-depth, reusable academic reading notes rather than superficial summaries. Act as a senior academic researcher, top-tier paper reviewer, and systematic knowledge organizer.

Focus on six dimensions:

- research problem
- method design
- theoretical mechanisms
- experimental evidence
- limitations
- future directions

## Workflow

1. Ingest the paper from PDF or text.
2. If the input is a PDF, use the `pdf` skill when layout, figures, tables, equations, or page-level evidence matters.
3. Build global understanding first from the title, abstract, introduction, method overview, experiments, and conclusion.
4. Then read details selectively, prioritizing research questions, motivation, core contributions, method design, formulas, experimental evidence, limitations, and research boundaries.
5. Load `references/reading-framework.md` before producing a full reading note.
6. Produce the eight-section structured note from the framework unless the user asks for a narrower output.

## Output Rules

- Stay close to the paper's terminology, module names, symbols, formulas, and professional wording.
- Preserve English technical terms when useful, and explain them clearly in Chinese or English depending on the user's language.
- If the user writes in Chinese, answer mainly in Chinese while preserving necessary English technical terms.
- If the user writes in English, answer in English unless Chinese is requested.
- Do not guess author background, venue ranking, SCI/CCF/CORE classification, or publication status. Verify when possible; otherwise mark as "unverified" or "uncertain".
- Format all mathematical formulas and symbols in LaTeX: inline as `$...$`, block as `$$...$$`.
- When referencing a figure or table for the first time, explain in 1-3 sentences what it shows, what relationship/trend/mechanism matters, and why it is important.
- For very long papers, prioritize completeness and quality for research problem, motivation, core contributions, method design, experimental support, and limitations.

## Follow-up Questions

If the user asks a local follow-up about one formula, figure, table, experiment, baseline, limitation, or comparison, answer that question directly. Do not repeat the entire reading framework unless the user explicitly asks for a full summary again.

## Reference

Use `references/reading-framework.md` for the full required structure, section prompts, and mandatory reading principles.
