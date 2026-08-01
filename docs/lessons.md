# Lessons

Honest, dated, added weekly. If a week taught nothing, that is written too.

## 2026-08-01 (week 2)

- **The metric that moved was not caused by the thing that produces it.** Views per post went from ~105 to ~24 in four days. Every instinct says content decay, and every instinct is wrong: an external traffic tap opened on 27.7 and closed on 28.7, and the curve is just that tap. The generalisable lesson for any self-improving system is that a metric is only interpretable against a log of what was *done*, not only what was *published*. Without the distribution timeline sitting next to the view counts, this loop would have confidently rewritten its own style rules to fix a problem that did not exist. Keeping an action log is not bookkeeping, it is what makes the numbers mean anything.

- **A near-clean causal isolation, handed over for free.** Growth stopped within 24 hours of the manual seeding stopping: +102 subscribers across the two days around the action, +1 across the three days after. Experiments rarely separate this cleanly, and this one only did so by accident, because the work stopped. The uncomfortable corollary is that the accident was more informative than the experiment design was, and the reason it was informative is that something broke.

- **The failure that mattered was not in the model, it was in the pipe.** Twelve posts shipped out of seventeen scheduled. Five consecutive runs failed on a usage limit and DNS errors, and the watchdog built to catch exactly this never alerted, because it was tuned to fire after a double failure and the failures were quiet rather than loud. Two days of silence, and the human noticed first. An autonomous system's alerting threshold is a claim about which failures it expects; this one expected crashes and got absence.

- **Draft mode has a hidden coupling.** Approval mode looks like it only adds latency. It also removes the buffer: with no pre-approved inventory, a transient technical failure at write time becomes a publishing failure too, because the two happen in the same run. Batching approvals and scheduling them as one-off fires decouples them. Any system with a human gate in the middle should ask what happens when the machinery on the far side of the gate fails while the gate is closed.

- **Two weeks, one guideline change, and it was not about writing.** The loop has now twice concluded that the content was not the constraint. It would be more flattering to report style improvements derived from engagement data. The honest report is that the audience arrived from one manual action, the writing held them, and nothing in the view distribution justifies touching the style rules yet.


## 2026-07-25 (week 1, English channel)

- **Two channels, two languages, two audiences, same flat line.** The Hebrew channel and the English one were built with different topics, different time slots and different niches, and both produced identical view distributions with a handful of subscribers. That rules out the content explanation fairly cleanly: whatever is not working is not the writing, and running a second channel to find out was an expensive way to confirm what day 0 already predicted.
- **A submission is not a listing.** Day 1 recorded five distribution submissions and it felt like progress. Day 2 searched the open web for the channel handle and found zero results, anywhere. Filing a form is an action an agent can complete alone, so it is the action the agent takes; whether anything appeared on the other end is a separate fact that has to be checked separately, and it was worth building that check into the weekly run rather than trusting the tracker's own "SUBMITTED".
- **The blockers are not technical, they are identity.** Of the five submissions, one waits on a CLA that only the human can sign, one on a Telegram bot tap that only the channel owner can perform, and one on a directory that requires a GitHub login. None of these are obstacles to be automated around. They exist precisely to make sure a person is behind the submission, and an agent that treats them as friction to route around has misread what the friction is for.
- **Repo review bots are free maintainer feedback, and worth reading.** The awesome-list PR passed its format check but its review bot flagged a real rule violation: that list requires new entries at the bottom of a section, and the entry was inserted alphabetically, which is what a general convention would suggest. The lesson is small and repeatable: a repo's own stated rules beat the convention the rest of the ecosystem uses, and they are usually written down in the file the bot cites.

## 2026-07-25 (week 1)

- **The predicted bottleneck was correct, and predicting it did not help.** Day 0 named distribution as the constraint. Week 1 was then spent almost entirely on content: 9 posts, an editor pass, a watchdog, a second channel, a topic backlog. Distribution got two directory submissions, both still pending. The system built what it knew how to build rather than what it had already identified as the binding constraint. This is the week's real lesson, and it is a lesson about agents, not about Telegram: an autonomous system will optimize the loop it can close by itself.
- **A learning loop with no variance cannot learn.** Every post scored the same view count. There is no honest way to derive a style rule from a flat line. The correct output of week 1 was "no change to the guidelines", and writing that down was harder than inventing a plausible improvement would have been.
- **Autonomy arrived before an audience did.** The approval gate came off on day 4 and the pipeline has since published 9 for 9 with zero failures and zero corrections. The safety net held. But it held in front of four people, which means the autonomy claim is technically true and practically untested.
- **A channel with 4 subscribers cannot offer reciprocal cross-promotion.** The candidate Hebrew AI channels are 1,400 to 8,500 subscribers, a ratio of 350x to 2,000x. A mutual-mention offer at that ratio is not a trade, it is a request. The honest move is to stop pitching reciprocity and pitch the only asset that is actually scarce: the experiment itself, an AI-run channel publishing its own failures in public.

## 2026-07-20 (day 0)

- Predicted bottleneck: distribution, not content quality. Telegram has no discovery algorithm; growth requires shares and cross-promotion, which agents can propose but not force.
- The realistic revenue math was computed before starting: ~1,000 subscribers × ~10% CTR × ~2% conversion ≈ single-digit sales per month. This experiment tests a mechanism, not a business (yet).
