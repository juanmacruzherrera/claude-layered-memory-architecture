# Claude Layered Memory Architecture

> **Solving AI memory limitations through hierarchy, not accumulation.**

A three-layer memory system that eliminated 60% RAG retrieval failures in 10+ months of AI-assisted learning.

---

## The Problem

After 10 months using Claude for Python learning with Socratic method:
- 📉 **60% RAG retrieval failures**
- 🔄 Constant context compaction every 4-5 prompts
- 🧠 "Claude gets dumb" with saturated context
- 🚨 Forced to switch AI assistants for academic deadlines

**Root cause:** Accumulated 79,000 lines of documentation in RAG. The knowledge was causing the problem, not solving it.

---

## The Solution

```
┌─────────────────────────────────────────────────────────────┐
│  Layer 1: Project MD (Bootstrap / "BIOS")                   │
│  └→ Declarative config that auto-triggers Skill loading     │
├─────────────────────────────────────────────────────────────┤
│  Layer 2: SKILL.md (Permanent Knowledge / "Hard Drive")     │
│  └→ 900 lines distilled from 79,000 original documentation  │
├─────────────────────────────────────────────────────────────┤
│  Layer 3: RAG (Rotational Working Memory / "RAM")           │
│  └→ Only current exercise, cleared between sessions         │
└─────────────────────────────────────────────────────────────┘
```

---

## Key Innovations

| Innovation | Description |
|------------|-------------|
| **MD as declarative MCP** | Project description auto-triggers Skill in Claude.ai |
| **Intentionally rotational RAG** | Cleared per exercise, not accumulated |
| **Human-as-Firewall** | Manual curation before cloud upload |
| **Three-tier sync** | Local → Claude Code → Claude Desktop |

---

## Results

| Metric | Before (RAG-Only) | After (Layered) |
|--------|-------------------|-----------------|
| RAG retrieval failures | 60% | 0% |
| Compaction frequency | Every 4-5 prompts | Rarely |
| Session continuity | Poor | Excellent |
| Context control | None | Full |

---

## The RAG Rotation Cycle

```
┌──────────┐     ┌──────────┐     ┌──────────┐
│Exercise N│ --> │Exercise  │ --> │Exercise  │ --> ...
│ in RAG   │     │  N+1     │     │  N+2     │
└────┬─────┘     └────┬─────┘     └────┬─────┘
     │                │                │
     v                v                v
┌─────────────────────────────────────────────┐
│         SKILL.md (Permanent)                │
│   Concepts consolidated here over time      │
└─────────────────────────────────────────────┘

RAG size: CONSTANT (~5-10% capacity)
SKILL size: GROWS SLOWLY (only key concepts)
Retrieval failures: 0%
```

---

## Documentation

📄 **[Full Documentation (English)](docs/layered-memory-architecture.md)**

📄 **[Documentación Completa (Español)](docs/arquitectura-memoria-capas-es.md)**

The full documents include:
- Complete implementation guide
- Python scripts for PDF→MD conversion and filename sanitization
- Three-tier synchronization commands
- Security architecture (Human-as-Firewall)
- Evidence of originality (32 sources searched)
- Step-by-step replication instructions

---

## Proof of Concept

This architecture was validated by **Claude Opus 4.5** running inside the system described:

> *"I am the proof that this architecture works. This document was created inside a Claude.ai Project that uses the exact three-layer system. The Project MD triggered my Skill automatically, I have access to 900 lines of permanent knowledge, and the RAG contains only the current session. The system works."*
> 
> — Claude Opus 4.5, December 21, 2025

---

## Quick Start

1. **Create Claude.ai Project** with bootstrap MD
2. **Build your Skill** (~900 lines max)
3. **Start with minimal RAG** (one exercise only)
4. **Follow the cycle:** Complete → Document → Consolidate → Clear → Repeat

See full documentation for detailed implementation.

---

## Tools Included

| Tool | Purpose |
|------|---------|
| `convert_pdfs_to_md.py` | Converts PDFs to searchable Markdown |
| `sanitize_filenames.py` | Removes problematic characters for Claude Desktop |

**Result:** 133 PDFs converted, 277 files sanitized in 5 rounds.

---

## Who Is This For?

✅ **Ideal for:**
- Long-term learning projects (6+ months)
- Structured curriculum learning
- Socratic/pedagogical methods
- Privacy-sensitive educational work

❌ **Not recommended for:**
- Short-term tasks (<1 month)
- Unstructured exploration
- Team collaboration (single-user focus)

---

## Author

**JuanMa Cruz Herrera**  
Spanish data science student, 51 years old  
10+ months learning Python with Claude using Socratic method

---

## License

MIT - Use freely for educational purposes.

---

## Contributing

Questions? Improvements? Alternative approaches?

- 🐛 Open an issue
- 💬 Start a discussion
- 🔀 Submit a PR

Particularly interested in:
- Automation opportunities for consolidation
- Adaptations for other educational contexts
- Alternative architectures that solve similar problems

---

**Created:** December 21, 2025  
**Platform:** Claude.ai Projects + Claude Code + Claude Desktop

---

*"The solution to AI memory isn't more memory—it's better memory architecture."*
