# Decision log

Newest first. Entries added by the weekly learning agent (system decisions) or the owner (design decisions).

## 2026-08-01, Guidelines v1.2: every post must stand alone

The only guideline change derived from week 2 data, and it is a structural rule, not a style rule.

Evidence: on 1.8, archive posts (174 to 182) held 62 to 137 views while fresh posts held 31 to 39. Old posts outperforming new ones by 2x to 4x is backwards for a subscriber-read channel. The only explanation consistent with the timeline is that the distribution traffic from discussion groups landed on the archive and kept seeping into it. So the typical reader of a given post is not a subscriber seeing it live; it is a stranger arriving at a four-day-old post through a link.

The rule that follows: no "as we said yesterday", no numbered series that require reading in order, no time-relative claims that age badly ("released this week" is wrong when read a fortnight later), and every post repeats the minimum context needed to stand alone, even at the cost of repetition for long-time subscribers.

## 2026-08-01, No style rules changed, and that is the second week running

Length, opening line, emoji budget, structure and posting time were all left untouched. Every organic post this week landed between 24 and 31 views at 24 hours, which is a band narrow enough that the differences inside it are noise. There is no signal that justifies rewriting a style rule, and inventing one would be the exact failure this project is supposed to demonstrate rather than commit.

This is worth stating plainly because it is the uncomfortable part: two weeks in, the learning loop has changed the writing guidelines once, and the change was about distribution surface, not about writing. The loop is working; what it keeps learning is that the content was never the constraint.

## 2026-08-01, Distribution is promoted from experiment to permanent infrastructure

Experiment 2 closed at 111 subscribers against a written-in-advance "above 25 = double down" threshold. But the sharper finding is what happened when it stopped: 8 subscribers on 27.7, 110 on 30.7, 111 on 1.8. Three days of consistent daily publishing produced one subscriber.

That isolates causality about as cleanly as this project will ever get: the growth engine is manual seeding of links inside relevant discussion groups, and daily content produces approximately zero growth on its own. Content retains whoever arrived; it does not bring anyone.

Consequence: seeding stops being a thing that happens when someone remembers, and becomes a standing line item in the owner's 15-minutes-a-day budget. The weekly share package is the artifact that feeds it.

## 2026-08-01, Draft mode needs an approved buffer, or any hiccup means zero output

Two days at the end of week 2 produced one post instead of six. Five consecutive automated runs failed, two on a weekly usage limit and three on DNS resolution. Two defects surfaced:

The watchdog, which exists precisely to catch this, alerts only after a double failure and never fired across two silent days. The owner noticed before the system did and asked where the daily post was. A system built to publish its own failures publicly was not reporting them privately to the one person who could act.

And draft mode converts every technical failure into zero published posts, because there is no pre-approved inventory to fall back on. The fix, proven on 1.8: approve three drafts in one batch and schedule them as `once` lines in the agent schedule. That decouples publishing from both approval latency and live-run success. This is now the standard operating procedure, not a workaround.


## 2026-07-25, English channel week 1: close the retention experiment before it starts, and put a falsifiable threshold on the directory strategy

The English channel's baseline experiment was written as "a short daily tip will retain subscribers once initial distribution exists". Two days and nine posts later, the clause after the comma had never become true, so the experiment was closed early as inconclusive rather than left running to produce a number that would look like evidence. Retention cannot be measured before acquisition, and an experiment whose precondition never fired has no result, only a delay.

Its replacement is deliberately written against the system's own recent work. The hypothesis states that generic Telegram directory listings produce close to zero subscribers for a niche English dev channel, and that the only route capable of moving the number requires a human to press send in a place where the audience already gathers. The threshold is written in advance: ten or more subscribers from listings alone by next Saturday keeps the directory route alive, fewer than ten kills it, and the agent stops opening new directory submissions entirely. A week of agent effort is on the line, which is the point. An experiment that cannot embarrass the thing that proposed it is not an experiment.

A verification sweep supports the pessimistic side already. Five submissions were filed on day one across directories and awesome lists. On day two, a web search for the channel handle returns zero results anywhere: no listing live, no page indexing it, nothing linking to it. Two of the five are blocked on the owner personally, one on a CLA signature and one on a bot verification tap, which is the same pattern the Hebrew channel found: the acquisition loop is the one an agent cannot close by itself.

## 2026-07-25, Week 1 learning loop: change nothing in the guidelines, move the whole budget to distribution

The first weekly learning run had the authority to rewrite its own writing rules and declined to use it. Every one of the week's nine posts scored the same view count, across different topics, lengths and time slots. A flat line contains no information about what to write differently, so any rule change would have been fabrication dressed as evidence. The changelog entry reads "no change, insufficient data".

What the data did establish is where the constraint sits. Views tracked audience size, not content quality, and the audience did not move: 4 subscribers on day 0, 4 subscribers on day 6. The system therefore closed its baseline experiment early rather than letting it run its full two weeks, and opened a replacement whose single metric is subscriber count, not engagement. Its threshold is written down in advance and is deliberately unflattering: if the number is still 4 next Saturday, the failure is not in the writing but in the assumption that a new Hebrew Telegram channel grows without a budget or a pre-existing audience, and the pivot conversation happens then instead of at the 30-day mark.

One process finding is recorded against the system itself. Day 0 correctly named distribution as the bottleneck. Week 1 was then spent building content infrastructure, a second channel, an editor pass, a watchdog, a topic backlog, while distribution received two directory submissions that are still pending. An autonomous system optimizes the loop it can close alone, and this one closed the writing loop beautifully while the acquisition loop, which requires a human to press send, stayed open.

## 2026-07-24, Approval gate removed: full autonomy, ahead of schedule

The original plan was two weeks of human-approved drafts. The owner chose to remove the gate on day 4, explicitly accepting the risk: posts now publish directly with no human review, on both channels. What remains between the model and the public: the immutable hard-rules section of the guidelines, the adversarial editor pass, the dumb-code publish-time guardrail, and the watchdogs. This is the experiment's most honest stress test: the safety net is now made only of the things we built, not of a human reading every word.

## 2026-07-24, Second channel: Claude Code Daily (English)

The experiment gains a sibling: t.me/DailyClaudeTips, one practical Claude Code tip per day in English, run by the same architecture (separate bot, separate state, separate learning loop, shared public repo). Niche chosen deliberately narrow: "AI tips" in English is a saturated ocean, but a channel about Claude Code that is itself run by Claude Code is a story only this system can tell. Extra guardrail for this channel: it is explicitly unofficial, never speaks as Anthropic, and every behavioral claim must be verified against primary docs before posting. Posting time 16:00 Israel (morning US, midday EU). No affiliate on this channel. The Hebrew channel is untouched.

## 2026-07-20, Identity and continuity: logo, topic backlog, state backup

The channel avatar was generated by the system itself (programmatic SVG rendered to PNG, uploaded via the Bot API) rather than by a human designer; on-brand for an AI-run channel. A ranked topic backlog now feeds the daily agent so no evening starts from zero, with the weekly agent replenishing it based on what got views. The entire private state (guidelines, logs, queue) is version-controlled locally after every run, so the history the learning loop depends on cannot be silently lost. LinkedIn remains draft-only by owner decision: the system writes, only the human publishes there.

## 2026-07-20, Reliability and measurement upgrades before day one

Four additions chosen as critical (and several rejected): per-post views via the public preview page (the learning loop was otherwise blind, optimizing only subscriber count); a self-healing watchdog that verifies outcome and retries before ever alerting the owner; an adversarial editor pass inside the daily agent; a weekly distribution package targeting the real bottleneck, acquisition. Rejected for now: discussion group, interactive bot, AI images per post, multi-channel. Reason: each adds surface area without attacking the current constraint.

## 2026-07-20, Affiliate frozen until a credibility threshold

No affiliate links at all until two conditions hold: 14+ days of consistent publishing AND 50+ subscribers. Suggested by the owner, adopted as policy. Rationale: trust is a new channel's only asset, and affiliate revenue at single-digit subscriber counts rounds to zero anyway. Monetization is sequenced after credibility, not alongside it.

## 2026-07-20, Kill the legacy news automation

The channel previously had a scheduled automation posting AI news translated to Hebrew. Decision: shut it down before this system's first post. One voice per channel; the learning loop needs a clean signal (two publishers make growth unattributable); and translated news is commodity content, the opposite of this channel's positioning. Decision made autonomously by the agent, per the experiment's rules.

## 2026-07-20, Keep the legacy posts, mark the reboot

Old translated-news posts stay. A channel with history reads as alive; an empty one reads as unproven. New subscribers see the latest few posts, so old content buries itself within days. Instead, the system's first post is a pinned "reboot" post declaring the new format and the AI-run transparency. No history rewriting.

## 2026-07-20, Initial design decisions

- **Draft-first rollout.** The system starts in approval mode; autonomy is earned, not assumed. One embarrassing post in a public channel costs more than two weeks of manual approvals.
- **One experiment at a time.** With a small audience, parallel experiments are noise. Each experiment has a hypothesis, one metric, and a decision threshold written down *before* the result.
- **Immutable guardrails.** The learning loop may rewrite style, structure, and topics, but not the ethics section (affiliate disclosure, no clickbait, source credit). A self-improving system needs a constitution it cannot amend.
- **Publish-time guardrail in dumb code.** The final typographic/safety check lives in a shell script, not in the model. The last line of defense should not be probabilistic.
- **Zero-infra bet.** Everything runs from launchd on a laptop. If the experiment dies, the autopsy is free.
