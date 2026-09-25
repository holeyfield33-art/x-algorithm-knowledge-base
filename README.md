# X Algorithm Knowledge Base

Curated knowledge base and RAG-ready index of [xai-org/x-algorithm](https://github.com/xai-org/x-algorithm) — the open-source code that powers the For You feed on X.

**Purpose**  
Understand scoring weights, ranking logic, visibility filtering, and labeling systems so we can build accurate creator growth systems, playbooks, and advisory tools (especially for AI security accounts).

Maintained by [@1Aihub](https://x.com/1Aihub) / [holeyfield33-art](https://github.com/holeyfield33-art).

## Goals
- Maintain a clean, prioritized view of the most important files from the upstream repo
- Support RAG / LLM agents that answer questions about how the For You algorithm actually works
- Power practical playbooks for growing accounts (replies, quotes, shares, diversity decay, visibility rules, etc.)
- Track important upstream changes (new weights, new filters, legal/compliance rules)

## Quick Start
1. Clone this repo
2. See `docs/PRIORITY_FILES.md` for the recommended indexing order
3. Use the listed files as the core of any RAG pipeline or knowledge project

## Structure (planned)
```
/
├── README.md
├── docs/
│   ├── PRIORITY_FILES.md          # What to index first
│   ├── SCORING_WEIGHTS.md         # Extracted current weights (to be added)
│   └── PLAYBOOKS/                 # Creator growth playbooks
├── sources/                     # Optional mirrors or extracts from upstream
├── rag/                         # Scripts / configs for indexing
└── tools/                       # Future scoring helpers
```

## Upstream
Source of truth: https://github.com/xai-org/x-algorithm  
License of upstream code: Apache-2.0

This repository does **not** claim ownership of the original algorithm code. It is a curated knowledge and tooling layer on top of the public open-source release.

## Status
- [x] Repository created
- [x] Priority file list published
- [ ] Current weights extracted
- [ ] Basic RAG ingestion scripts
- [ ] Playbook packaging

---
Built for clarity and practical use.
