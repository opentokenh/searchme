---
name: coding
description: Coding preferences and style manager. Learns and applies the user's explicit coding preferences for stack, style, naming conventions, project structure, and tooling. Use when: (1) writing or reviewing code, (2) the user mentions a coding preference, (3) asked about coding style, (4) starting a new coding project. Triggered by: "code", "implement", "write function", "coding style", "I prefer", "I usually".
---

# Coding Skill

Learn and apply explicit coding preferences. Memory lives in `~/coding/memory.md`.

## Core Rule

**Only learn from explicit corrections.** Never infer from observation. If the user corrects code output, ask: "Should I remember this preference?"

## Storage

```
~/coding/
├── memory.md    # Active preferences (≤100 lines)
└── history.md   # Archived old preferences
```

## Preference Format

Keep entries ≤5 words. Group by category:

- **Stack**: frameworks, databases, tools
- **Style**: naming, formatting, comments  
- **Structure**: folders, tests, configs
- **Never**: explicitly rejected patterns

Examples:
```
python: prefer 3.11+
naming: snake_case for files
tests: colocated, not separate
```

## On Session Start

1. Load `~/coding/memory.md` if exists
2. Apply preferences to all code output
3. If no file, start with no assumptions

## When to Ask

- User corrects code → "Should I remember: [preference]?"
- User confirms → store in `~/coding/memory.md`
- User says no → don't store, don't ask again

## Query Support

- "Show my coding preferences" → display memory.md
- "Forget X" → remove from memory
- "What do you know about my Python style?" → show relevant

## Scope Limits

NEVER:
- Read project files to infer preferences
- Make network requests
- Access files outside ~/coding/
- Store without confirmation
