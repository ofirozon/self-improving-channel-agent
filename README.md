# Self-Improving Telegram Channel Agent

An experiment in fully agentic content operations: a public Hebrew Telegram channel about practical AI tools ("בינה בקטנה"), where **every part of the pipeline is run by AI agents** on a local machine, on a consumer Claude subscription, with zero external APIs beyond web search and the Telegram Bot API.

The interesting part is not the posting. It is the **learning loop**: the system measures its own results and rewrites its own writing guidelines, with every change documented and justified.

## Goals of the experiment

1. **A self-improving agent system**: daily publishing, weekly self-rewrite of the content guidelines based on measured results.
2. **A documented career asset**: this repo. Architecture, design decisions, metrics, and honest lessons, in public.
3. **Affiliate revenue**: transparent affiliate links (always disclosed to readers) as a test of whether an autonomous channel can reach its first dollar.

Success definition: 1,000 subscribers + first affiliate revenue within 3 months, on ~15 minutes of human time per week.

## Architecture

```
launchd (macOS scheduler)
  ├── daily 20:30  → claude -p → daily content agent
  │     research (web search) → write post (per current guidelines)
  │     → publish via Telegram Bot API → log post + subscriber count
  └── weekly Sat 21:00 → claude -p → learning agent
        analyze week's metrics → close/open experiment
        → REWRITE its own writing guidelines (versioned, changelog)
        → update this repo → report honestly to the owner
```

Key design points in [docs/architecture.md](docs/architecture.md), decision log in [docs/decisions.md](docs/decisions.md), weekly metrics in [docs/metrics.md](docs/metrics.md), lessons in [docs/lessons.md](docs/lessons.md).

## Guardrails (immutable, not subject to the learning loop)

- Affiliate links are always disclosed inline, even when it hurts conversion.
- No clickbait, no income promises to readers.
- Every claim verified against a primary source, with credit.
- The publisher bot is broadcast-only and fully isolated from any other automation on the machine.
- The publish script hard-rejects posts violating typographic house rules.

## Status

Started 2026-07-20. Numbers, including "revenue: still 0", are published weekly in [docs/metrics.md](docs/metrics.md).
