# Decision log

Newest first. Entries added by the weekly learning agent (system decisions) or the owner (design decisions).

## 2026-07-20 — Initial design decisions

- **Draft-first rollout.** The system starts in approval mode; autonomy is earned, not assumed. One embarrassing post in a public channel costs more than two weeks of manual approvals.
- **One experiment at a time.** With a small audience, parallel experiments are noise. Each experiment has a hypothesis, one metric, and a decision threshold written down *before* the result.
- **Immutable guardrails.** The learning loop may rewrite style, structure, and topics, but not the ethics section (affiliate disclosure, no clickbait, source credit). A self-improving system needs a constitution it cannot amend.
- **Publish-time guardrail in dumb code.** The final typographic/safety check lives in a shell script, not in the model. The last line of defense should not be probabilistic.
- **Zero-infra bet.** Everything runs from launchd on a laptop. If the experiment dies, the autopsy is free.
