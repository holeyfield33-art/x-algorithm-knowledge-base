# RAG / Indexing Notes

This folder is reserved for scripts and configuration that turn the prioritized upstream files into a searchable knowledge base.

## Suggested Approach
1. Clone or periodically sync the highest-priority files listed in `docs/PRIORITY_FILES.md`
2. Chunk by function / logical block for `.rs` files, keep file path + symbol as metadata
3. Embed and store in a local vector DB (Chroma, FAISS, Qdrant, etc.) or use directly in an LLM project
4. Re-index weekly or on significant upstream commits

## Minimal Viable Index
Start with only:
- README.md (upstream)
- home-mixer/params/param.rs
- home-mixer/scorers/value_model.rs
- visibility-filtering core rules
- This repo’s `docs/SCORING_WEIGHTS.md` and playbooks

That set already answers the majority of practical questions about ranking and growth strategy.
