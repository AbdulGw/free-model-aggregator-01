# free-model-aggregator-01: Entropy-Weighted Headroom Greedy Aggregator V2

Deterministic AI Model Aggregator submitted by `@abdulgw` for the `free-model-aggregator-01` challenge ($500 pot).

## Strategy Overview
- **Solver**: `EntropyHeadroomRouter` (Entropy-Biased Capacity Headroom Greedy)
- **Architecture**: Non-linear entropy weighting favoring high headroom providers during candidate tie-breaking to avoid late-stage exhaustion
- **Wire Support**: Dual-wire OpenAI Chat Completions (`/v1/chat/completions`) & Anthropic Messages (`/v1/messages`), supporting JSON and streaming SSE.
- **Failover**: Proactive rate-limit avoidance with zero-failure fallbacks across 10 free model providers.
