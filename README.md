# Hi, I'm Amin

Backend & automation developer with a strong mathematics and logic background. I came to software through C and MATLAB, work primarily in **Python** and **JavaScript (Cloudflare Workers)**, and I build retrieval and automation systems end to end — including the unglamorous parts: caching, deduplication, capacity management, and regression tooling.

## Featured project

### [open-classical-text-worker](https://github.com/aminbm1919/open-classical-text-worker)

A serverless **RAG backend** that turns a Custom GPT into a philosophy research assistant — a single Cloudflare Worker (~36.7k lines, ~716 functions) engineered to run entirely on free-tier infrastructure.

- Hybrid retrieval: SQLite FTS5 + dense vectors, fused with weighted **Reciprocal Rank Fusion**
- Vector storage across free tiers: Neon **pgvector** (`halfvec`, topic-sharded) + **Qdrant** (int8), with capacity-derived eviction and guaranteed tombstone deletes
- **SimHash** near-duplicate detection (Manku et al., WWW 2007 thresholds) before anything gets embedded
- Evidence-gated pipeline: only actually-read text is citable — candidates are never evidence
- 9-shard D1 storage with R2 full-text offload, 4 lock-aware cron pipelines, ~90 ledgered deploys

**→ Try it live: [hybrid search demo](https://chunking.aminbm1919.workers.dev/demo)** · **Case study: [Engineering a Production RAG Backend on $0/month](https://github.com/aminbm1919/open-classical-text-worker/blob/main/docs/CASE_STUDY.md)**

## What I build

- **RAG chatbots & Custom GPT backends** — document Q&A over your own content, with citations
- **Web scraping & data pipelines** — collection, cleaning, and delivery to Excel/CSV/database
- **Telegram bots & workflow automation** — from simple order bots to LLM-connected assistants
- **Scientific computing** — MATLAB → Python migration, numerical methods, optimization

## Tools I use

`Python` · `JavaScript` · `Cloudflare Workers` · `SQL / SQLite / Postgres` · `pgvector` · `Qdrant` · `FTS5 / information retrieval` · `embeddings & LLM APIs` · `pandas` · `FastAPI` · `C` · `MATLAB`

## Contact

📫 aminbm1919@gmail.com — open to freelance projects.
