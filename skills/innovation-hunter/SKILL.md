---
name: innovation-hunter
description: Cross-domain innovation connection finder for multimodal LLMs, LLM agents, and Beidou/satellite communication. Use when: (1) finding unexpected connections between these three research areas, (2) generating novel research ideas at field intersections, (3) evaluating research direction promise, (4) finding gaps in current literature, (5) lateral thinking about research. Triggers on: "any interesting connections", "innovation", "research gap", "can X help Y", "what if we combined", "novel research idea", cross-domain brainstorming, thinking laterally.
---

# Innovation Hunter

Find unexpected connections between multimodal LLMs, LLM agents, and Beidou/satellite communication — the researcher's core differentiation.

## Core Protocol

1. Read `references/connection-patterns.md` for the four connection strategies
2. Search ArXiv for recent papers bridging these fields
3. Pick the most promising connection
4. Output a Connection Brief (see `references/brief-template.md`)

## Four Connection Strategies

1. **Transplant** — Apply X domain's idea to Y
2. **Combine** — Merge two mature technologies into new product
3. **Analogy** — What problem in X is like Y?
4. **Reverse** — Flip the assumption

See `references/connection-patterns.md` for specific examples and false-positive filtering.

## Output Format

For each promising connection, output a Connection Brief:

```
== 连接确认 ==
== 为什么有意思 ==
== 最大风险 ==
== 需要的条件 ==
== 相关论文 ==
```

Use `references/brief-template.md` for full format and examples.

## Quality Filter

A real connection must have:
- ✅ Genuine technical challenge (not obvious)
- ✅ Potential for unique contribution
- ✅ Feasible next steps

False positive examples:
- ❌ "Use Agent for satellite data parsing" — just method transplant
- ❌ "Multimodal + Beidou = map with images" — too simple
