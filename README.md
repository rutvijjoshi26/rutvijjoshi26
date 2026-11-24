### Hi, I'm Rutvij. I build software and AI systems and get them through production.

Software engineer looking for a **founding or early engineer role** at a startup, from **February 2027**. I build AI systems and the backend under them. MS in Computer Science at the University of Chicago, finishing December 2026.

**Before grad school:** I was a Software Development Engineer at [Callmatic](https://callmatic.ai) (Jan 2024 to Aug 2025), a voice AI startup whose phone agents handle calls for enterprise clients.

- Scaled the platform from 200K to **1M+ daily calls** by breaking a Next.js monolith into separately deployable services.
- Cut OpenAI costs **90%** and response latency **80%** with a Redis caching layer in the FastAPI backend.
- Let the agent act mid-call, calling clients' own APIs through MCP tool connections, and grounded its answers in each client's verified data with RAG.
- Deployed the platform into 6 enterprise clients' own environments, working directly with their teams.

**Now:** I'm an ML research assistant at UChicago's TMW Center. I found a data leak that was inflating the production model's reported accuracy, then built an infant cry/laugh audio classifier that reaches 89.1% accuracy.

### Things I've built (each README has the numbers and how to check them)

- **[multi-agent-issue-resolver](https://github.com/rutvijjoshi26/multi-agent-issue-resolver)**: when a bug report comes in, LangGraph agents find similar issues that were already fixed and propose a fix with citations. I tested it on 100 held-out issues against the real merged fixes. It declines to answer when unsure: it answered 29% of cases and was right on 66% of those.
- **[rowback](https://github.com/rutvijjoshi26/rowback)**: an undo button for PostgreSQL. When a bad `DELETE` (yours or an AI agent's) hits production, it reverses just that transaction and keeps every later write. In benchmarks it was 9.5x faster than restoring from backup, with every row checked by md5.
- **[route-dispatch-platform](https://github.com/rutvijjoshi26/route-dispatch-platform)**: plans delivery routes on real roads and re-plans while vans are driving. On a 200-stop Chicago day it cut driving distance 44% versus nearest-neighbor and delivered all 200 stops inside their time windows. A mid-shift re-plan takes 1.5 s.
- **[agent-pin](https://github.com/rutvijjoshi26/agent-pin)**: an always-on-top overlay for my coding agents (Claude Code, Codex). It shows every session, puts the ones waiting on my approval first, recaps what changed since I last looked, and warns when two sessions edit the same file. Runs on macOS, Windows and Linux.
- **[parallel-compressor-go](https://github.com/rutvijjoshi26/parallel-compressor-go)**: a parallel block compressor in Go with work stealing, a checksummed format and bounded memory, fuzz- and race-tested. Against `gzip -1` it compresses 2.4 to 4.2x faster and decompresses 1.9 to 2.2x faster; the README also shows where zstd still wins.
- **Cirgle**: a habit-tracking app with friends that grew to 140+ users in 3 countries (React Native, FastAPI, Supabase).

### How I work

I get a working version in front of users fast, on simple tools that are cheap to change, then scale what real load demands. At Callmatic that meant growing the platform from 200K to 1M+ daily calls as the traffic arrived. I also write down what didn't work: [listing-search-ranking](https://github.com/rutvijjoshi26/listing-search-ranking) documents a label-leakage bug I found in my own pipeline.

**Stack I use most:** Python, TypeScript, Go · FastAPI, Node.js, React · Postgres, Redis · LangChain/LangGraph, RAG, MCP, PyTorch · Docker, AWS.

[rutvijjoshi5@gmail.com](mailto:rutvijjoshi5@gmail.com) · [LinkedIn](https://linkedin.com/in/rutvij-joshi5). I usually reply within a day.
