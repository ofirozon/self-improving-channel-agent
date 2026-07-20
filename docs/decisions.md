# Decision log

Newest first. Entries added by the weekly learning agent (system decisions) or the owner (design decisions).

## 2026-07-20 — Affiliate frozen until a credibility threshold

No affiliate links at all until two conditions hold: 14+ days of consistent publishing AND 50+ subscribers. Suggested by the owner, adopted as policy. Rationale: trust is a new channel's only asset, and affiliate revenue at single-digit subscriber counts rounds to zero anyway. Monetization is sequenced after credibility, not alongside it.

## 2026-07-20 — Kill the legacy news automation

The channel previously had a scheduled automation posting AI news translated to Hebrew. Decision: shut it down before this system's first post. One voice per channel; the learning loop needs a clean signal (two publishers make growth unattributable); and translated news is commodity content, the opposite of this channel's positioning. Decision made autonomously by the agent, per the experiment's rules.

## 2026-07-20 — Keep the legacy posts, mark the reboot

Old translated-news posts stay. A channel with history reads as alive; an empty one reads as unproven. New subscribers see the latest few posts, so old content buries itself within days. Instead, the system's first post is a pinned "reboot" post declaring the new format and the AI-run transparency. No history rewriting.

## 2026-07-20 — Initial design decisions

- **Draft-first rollout.** The system starts in approval mode; autonomy is earned, not assumed. One embarrassing post in a public channel costs more than two weeks of manual approvals.
- **One experiment at a time.** With a small audience, parallel experiments are noise. Each experiment has a hypothesis, one metric, and a decision threshold written down *before* the result.
- **Immutable guardrails.** The learning loop may rewrite style, structure, and topics, but not the ethics section (affiliate disclosure, no clickbait, source credit). A self-improving system needs a constitution it cannot amend.
- **Publish-time guardrail in dumb code.** The final typographic/safety check lives in a shell script, not in the model. The last line of defense should not be probabilistic.
- **Zero-infra bet.** Everything runs from launchd on a laptop. If the experiment dies, the autopsy is free.
