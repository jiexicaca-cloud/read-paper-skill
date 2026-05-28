# read-paper-skill

A Codex skill for deep, structured academic paper reading notes.

This skill is designed for researchers who want more than a surface summary. It guides Codex to read academic papers through six dimensions:

- research problem
- method design
- theoretical mechanisms
- experimental evidence
- limitations
- future directions

It is especially useful for neuroscience and adjacent scientific papers, but can be used for broader academic literature.

## What It Does

When you ask Codex to read, summarize, analyze, or critique a paper, this skill asks Codex to produce a structured note covering:

1. Bibliographic information
2. Overall overview
3. Methods and technical details
4. Experimental results and analysis
5. Figures and tables interpretation
6. Limitations and research boundaries
7. Extensions and future directions
8. Core conclusion

It also instructs Codex to:

- stay close to the paper's terminology and equations
- use LaTeX for formulas
- explain figures and tables when first referenced
- mark unverifiable metadata as `unverified` or `uncertain`
- answer local follow-up questions directly instead of repeating the full framework

## Installation

Copy this repository into your Codex skills directory:

```powershell
git clone https://github.com/jiexicaca-cloud/read-paper-skill.git C:\Users\<YOUR_USER>\.codex\skills\read-paper
```

Or copy the files manually into:

```text
~/.codex/skills/read-paper
```

Then restart Codex so the skill is discovered.

## Example Prompts

```text
Read this paper and produce a structured critical reading note.
```

```text
Summarize this neuroscience PDF, focusing on method design, experimental evidence, and limitations.
```

```text
Explain Figure 2 from this paper and why it matters.
```

```text
What does this formula mean in the paper's method?
```

## Files

- `SKILL.md`: trigger description and core workflow
- `agents/openai.yaml`: UI metadata
- `references/reading-framework.md`: full academic paper reading framework
