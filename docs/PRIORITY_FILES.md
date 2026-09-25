# Highest-Priority Files to Index from xai-org/x-algorithm

Use this ordered list when building a RAG index, knowledge base, or LLM context for understanding the For You feed algorithm.

## Tier 1 – Core Understanding (Index These First)

| Priority | Path | Why it matters |
|----------|------|----------------|
| 1 | `README.md` | Full system architecture, request path, labeling path |
| 2 | `home-mixer/params/param.rs` | **Most important file** — production default weights and key configuration parameters |
| 3 | `home-mixer/scorers/value_model.rs` | How the final weighted score is calculated from Phoenix predictions |
| 4 | `home-mixer/scorers/` (all ranking/scoring files) | Complete scoring pipeline |
| 5 | `vm-ranker/scoring/value_model.rs` + `vm-ranker/params.rs` | Value model and re-ranking parameters |
| 6 | `docs/` | Human-readable notes on important changes (e.g. bidirectional boost) |

## Tier 2 – Filters & Visibility

| Priority | Path | Why it matters |
|----------|------|----------------|
| 7 | `visibility-filtering/` | ALLOW / INTERSTITIAL / DROP decisions |
| 8 | `home-mixer/filters/` | Pre-scoring and post-selection filters |
| 9 | `abuse-enforcement-service/` (especially rules YAML) | Account and post labeling / enforcement |
| 10 | `scarecrow/` + `botmaker/` + `botmaker-rules/` | Real-time labeling rules |

## Tier 3 – Supporting Systems

| Priority | Path | Why it matters |
|----------|------|----------------|
| 11 | `phoenix/` | Ranking + retrieval model code |
| 12 | `xai-value-model/` | Additional scoring logic |
| 13 | `thunder/` | In-network candidates |
| 14 | `simclusters/` | Out-of-network candidates |
| 15 | `agatha/`, `bdsm/`, `user-cred-v2/` | Account-level scoring models |
| 16 | `under-the-hood/` | Transparency tool |
| 17 | Content understanding (`grox/`, `media-model-proxy/`, `clip/`, etc.) | Safety and media classifiers |

## Recommended Indexing Order
1. Start with the six Tier 1 items.
2. Add visibility and filter systems (Tier 2).
3. Expand to Phoenix and account models only when deeper technical detail is needed.

## Notes
- Weights live primarily in `home-mixer/params/param.rs`.
- Always prefer the latest commit on `main` of the upstream repo.
- Comments in the scoring files are intentionally written to be readable by both humans and LLMs.
