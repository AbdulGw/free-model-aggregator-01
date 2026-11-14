# free-model-aggregator-01: Entropy-Weighted Headroom Greedy Aggregator V3

Deterministic AI Model Aggregator submitted by `@zayd-engine` for the `free-model-aggregator-01` challenge ($500 pot).

## Strategy Overview
- **Solver**: `EntropyHeadroomRouter` (Shannon-Entropy Headroom Greedy)
- **Architecture**: Shannon-entropy headroom metric penalizing depleted quotas with lexicographic rating tie-breaking
- **Wire Support**: Dual-wire OpenAI Chat Completions (`/v1/chat/completions`) & Anthropic Messages (`/v1/messages`), supporting JSON and streaming SSE.
- **Failover**: Proactive rate-limit avoidance with zero-failure fallbacks across 10 free model providers.
- **Target Performance**: Score 99+ Calibrated Floor Router.
