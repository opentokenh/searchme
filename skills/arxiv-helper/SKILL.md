---
name: arxiv-helper
description: ArXiv paper search and summarization for multimodal LLMs, LLM agents, and Beidou/satellite communication. Use when: searching ArXiv for papers, summarizing paper abstracts, finding related works, getting paper recommendations, analyzing arXiv links shared by the user. Triggers on: "search arxiv", "find papers on", "what's new on arXiv", "paper about", "arXiv link", "最新论文", "找相关工作".
---

# ArXiv Helper

Search and summarize ArXiv papers in the researcher's three domains.

## Search

Use web search with `site:arxiv.org` queries. See `references/search-queries.md` for categorized query lists by research area.

Quick examples:
- `site:arxiv.org "multimodal large language model" 2026`
- `site:arxiv.org "LLM agent" planning tool use`
- `site:arxiv.org "Beidou" navigation deep learning`

## Summarize

For each promising paper:

```
## [Title]
- **ArXiv**: arXiv:XXXXX.XXXXX
- **One-line**: [核心创新点]
- **Method**: [主要方法]
- **Key Result**: [关键数字]
- **Relevance**: [与研究的关联]
- **Link**: https://arxiv.org/abs/XXXXX
```

## On Every Paper

Always:
1. 1-2 sentence summary
2. Connection to researcher's interests (multimodal × agent ×北斗)
3. 2-3 follow-up paper suggestions
4. Note any cross-domain connections
