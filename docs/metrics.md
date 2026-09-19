# Weekly metrics

Updated every Saturday by the learning agent. Full transparency, including zeros.

| Week ending | Channel | Subscribers | Posts | Affiliate clicks | Affiliate revenue | Note |
|---|---|---|---|---|---|---|
| 2026-07-25 | Claude Code Daily (EN) | 2 (+0) | 9 | 0 (no affiliate on this channel) | $0 | Week 1, and the channel is 2 days old. Nine posts in 36 hours, zero pipeline failures. Views 2 to 3 on every post, against an audience of 2, so views are counting subscribers, not measuring content. Distribution: five submissions filed on day 1, and a web-wide search for the channel handle on day 2 returns zero results. Nothing is live yet. |
| 2026-07-25 | בינה בקטנה (HE) | 4 (+0) | 9 | 0 | $0 | Week 1. Publishing pipeline: 9 for 9, zero failures. Growth: zero. Views per post flat at 2 across every topic, length and time slot, i.e. views are measuring audience size, not content quality. No distribution round was actually executed this week; two directory submissions are still pending review. |
| 2026-08-01 | Claude Code Daily (EN) | 4 (+2) | 10 | 0 (no affiliate on this channel) | $0 | Week 2. The week the distribution question got a real answer. Two listings went live, a merged PR into a ~7k-star awesome list and a Telegram directory, with no manual promotion to contaminate the signal. Combined measured effect: +2 subscribers. The pre-registered threshold was +10, so the free agent-submittable directory route is now declared dead and closed. Publishing: 10 of 14 scheduled slots, broken by a usage limit on 31.7 followed by two days of API errors; the watchdog detected it, self-healed, failed, and alerted, which is exactly what it was built to do. Views 3 to 5 across all 20 posts, flat for the second week. |
| 2026-08-01 | בינה בקטנה (HE) | 111 (+107) | 12 | 0 | $0 | Week 2. Subscribers went 4 to 111, and essentially all of it happened in the 48 hours around one manual action: the owner joined Israeli discussion groups and seeded links to specific posts inside relevant threads. Growth in the three days after that action stopped: +1. Publishing reliability collapsed at the end of the week, 12 posts shipped out of 17 scheduled, with five consecutive automated runs failing and the watchdog never alerting. |
| 2026-08-29 | Claude Code Daily (EN) | 19 (+3) | 41 | 0 (no affiliate on this channel) | $0 | Weeks 5 and 6, a fortnight because the 22.8 run did not happen. Publishing was perfect: 41 of 41 slots, second clean fortnight running, though three posts landed over two hours late in a GitHub cron degradation and three more went out through a rescue path that records nothing, so the publish log under-counts. Growth was not: +3, against +12 in the previous fortnight under identical conditions of zero distribution. Experiment 4 closed in its middle band (18 subscribers on the 23.8 checkpoint, threshold 25) but the fortnight totals answer it better than the checkpoint did: the +12 was an event, not a rate, and acquisition fell fourfold while the archive grew from 56 posts to 98. A web search for the channel handle returns zero organic mentions for the sixth week; 98 posts have bought no discovery surface outside Telegram. Views: mature cohort means 4.55, flat against 4.1 a fortnight ago. Fourth consecutive report that nothing can be concluded about writing. |

## Per-post views, week 1, Claude Code Daily (EN)

| Message id | Topic | Views |
|---|---|---|
| 4 | Welcome / what this channel is (pinned) | 3 |
| 6 | CLAUDE.md project memory | 3 |
| 7 | Plan mode before building | 3 |
| 8 | Hooks for auto lint and test feedback | 3 |
| 9 | Mini-guide: your first custom skill in 5 minutes | 3 |
| 10 | Resuming sessions (--continue, --resume) | 3 |
| 11 | /fork background sessions and /subtask | 2 |
| 12 | Forcing a subagent with @agent-name | 2 |
| 13 | /code-review no longer auto-runs | 2 |

Same shape as the Hebrew channel, one channel over: a flat line. The 3s are older posts, the 2s are newer ones. The mini-guide, which took the most work, scored exactly what the shortest tip scored. There is no content signal in this table, and saying so is the only honest thing to do with it.

## Per-post views, week 1, בינה בקטנה (HE)

| Message id | Topic | Views |
|---|---|---|
| 163 | Reboot post (pinned) | 3 |
| 166 | Spotting phishing/smishing with ChatGPT | 2 |
| 167 | NotebookLM: PDF to summary and audio overview | 2 |
| 168 | Excel/Sheets formulas from plain language | 2 |
| 169 | GPT-Live voice engine | 2 |
| 170 | Prompt pattern: three options, then attack each | 2 |
| 171 | Gamma: a full deck from one block of text | 2 |
| 172 | Email thread to an accountability table | 2 |
| 173 | ChatGPT unified search | 1 (30 minutes old) |

Baseline for comparison: posts 150 to 159, produced by the legacy translated-news automation that was shut down before this system started, scored 1 to 4 views. The new content sits in the same band. At this audience size the difference between 2 and 3 views is noise, not signal.

## What this means for the learning loop

A learning loop needs variance to learn from. Week 1 produced none: every post landed on the same number. Any style rule the system "learned" from this data would be invented, not derived. That is why week 1 changed nothing in the writing guidelines and moved the entire experiment budget to distribution instead.

## Per-post views at 24 hours, week 2, בינה בקטנה (HE)

Cumulative views are a function of post age, not post quality, so week 2 switches to a single comparable metric: **views at 24 hours old**, reconstructed from timestamped snapshots.

| Message id | Topic | Published | Views at 24h | Context |
|---|---|---|---|---|
| 180 | Checkpoints and /rewind | 27.7 20:32 | ~105 | inside the distribution wave |
| 181 | skills.sh | 28.7 12:24 | ~68 | tail of the wave |
| 182 | /doctor | 28.7 13:28 | ~48 | tail of the wave |
| 183 | Anthropic's course site | 29.7 07:50 | ~31 | organic |
| 184 | Plan mode | 29.7 12:47 | ~29 | organic |
| 185 | /usage | 29.7 20:00 | ~28 | organic |
| 186 | Claude Cowork | 30.7 10:52 | ~24 | organic |

**Clean organic baseline: 24 to 31 views per post at 24 hours, against 111 subscribers. That is a 22 to 28 percent open rate, which is unremarkable and healthy for a Telegram channel.**

The drop from ~105 to ~24 over four days is the most misreadable number in this repo. It looks like content decay. It is not. It is an external traffic tap being switched off. The 100+ posts did not earn those views by being better written; they happened to be the archive that the distribution traffic landed on. A learning loop that read this curve without the distribution timeline would confidently derive the wrong style rules, which is the specific failure mode this repo exists to document.

## What week 2 could and could not measure

Could: the growth engine. Isolated almost cleanly, because the input was a single dated manual action and the output stopped within 24 hours of it stopping.

Could not: whether three posts a day dilutes. The pace change was decided on 29.7, and exactly one day since then actually published three posts. That day produced 88 total views against 24 on a one-post day, with no drop in the per-post average, which supports the no-dilution hypothesis at n=1 day. Not significant. Moved to experiment 3 with thresholds written in advance.

## Per-post views, week 2, Claude Code Daily (EN)

All 20 posts, read at 2026-08-01 21:30. The audience went from 2 to 4 during the week.

| Message id | Slot | Topic | Views |
|---|---|---|---|
| 4 | pinned | Welcome / what this channel is | 5 |
| 6 to 13 | week 1 | (see week 1 table above) | 4 to 5 |
| 14 | 26.7 16:00 | Nested subagents, depth 3 by default | 5 |
| 15 | 26.7 20:00 | sandbox.credentials, denying ~/.ssh and ~/.aws | 5 |
| 16 | 27.7 16:00 | --max-budget-usd spend cap for headless runs | 5 |
| 17 | 27.7 20:00 | MCP failures now print HTTP status and error text | 5 |
| 18 | 28.7 16:00 | The 200-call session WebSearch cap | 5 |
| 19 | 28.7 20:00 | Fast mode billing: enable it at session start | 5 |
| 20 | 29.7 16:00 | The space before `*` in Bash permission rules | 3 |
| 21 | 29.7 20:00 | What /rewind does not restore | 3 |
| 22 | 30.7 16:00 | Git worktrees and .worktreeinclude | 4 |
| 23 | 30.7 20:00 | Backgrounding a Bash command with Ctrl+B | 3 |

Week 1's whole distribution sat at 2 to 3. Week 2's sits at 3 to 5. The audience doubled and every post moved up together, which is the signature of a metric that is counting people rather than measuring writing. The 16:00 posts averaged 4.4 and the 20:00 posts 4.2, one view apart on one day out of five. The mini-guide (msg 9), the most expensive post to produce, sits at 5, tied with the cheapest tips.

Second consecutive week with no content signal, and therefore the second consecutive week with no change to the writing guidelines.

## What week 2 measured on the English channel

Could: whether free directory listings move a niche English dev channel. Cleanly, and for the first time, because the precondition finally became true. Two listings went live, nothing else was done, and the number moved by 2.

Could not: anything about the writing. Twenty posts, four subscribers, a 2-view spread. It also could not measure the archive-conversion hypothesis on its own terms, because the launch round it was waiting for never happened; what it got instead was a weaker natural version of the same test, two low-traffic listings pointing at a 20-post archive, and that produced +2.

## Weeks 3 and 4, בינה בקטנה (HE) — 2026-08-02 to 2026-08-15

No weekly run happened on 8.8. It fell inside a run of eight consecutive agent failures, so this covers two weeks rather than one. That absence is itself the headline finding.

| Metric | Value |
|---|---|
| Subscribers 1.8 | 111 |
| Subscribers 15.8 | 110 |
| Delta over two weeks | -1 |
| Peak | 111, held 4.8 to 9.8 |
| Posts published 2.8 to 15.8 | 21 (ids 194 to 214) |
| Posts the schedule called for | 34 |
| Days with zero posts | 3 |
| Affiliate clicks | 0 (no affiliate links in any post) |
| Revenue | 0 |

### Views at 24 hours, by slot

The only two days on which three posts actually went out are 13.8 and 14.8. That is the entire dataset on the new cadence.

| Day | Morning 09:00 | Noon 13:00 | Evening 20:30 | Mean |
|---|---|---|---|---|
| 13.8 (Thu) | 22 | 23 | 21 | 22.0 |
| 14.8 (Fri) | 20 | 19 | 20 | 19.7 |
| **Slot mean** | **21.0** | **21.0** | **20.5** | |

Organic baseline set on 1.8: 24 to 31, mean ~28.

### What weeks 3 and 4 measured

Could: whether one publishing slot beats another. Cleanly, and the answer is no. 21.0 vs 21.0 vs 20.5 across six measurements, against a pre-written threshold of a 30% gap over at least five. That is a rare thing in this log — a negative result strong enough to close a question rather than defer it. The time-of-day question is settled for now.

Could not: whether three posts a day dilutes. Experiment 3 was closed as void by a condition written into it in advance — "if fewer than 15 of 21 posts publish, this is a reliability problem, not a cadence problem." Eight of 21 published. The drop from 22.0 to 19.7 lands exactly on Friday and Saturday, and an identical weekend dip was already observed once (the 8-9.8 posts closed at 16 to 20 and later crawled to 26 to 33). n=2 days, one of them contaminated. Not significant. Rerun as experiment 4 over three consecutive weekdays, 16 to 18.8, thresholds written in advance.

Also could not: anything about growth. Two weeks of steady publishing, including three days at the higher cadence, produced minus one subscriber. Experiment 2 already isolated the cause: the only proven growth engine is manual seeding in discussion groups, and none has happened since 28.7.

## Weeks 3 and 4, Claude Code Daily (EN) — 2026-08-02 to 2026-08-15

Same missing weekly run as the Hebrew channel, same cause, so this is a two-week report.

| Metric | Value |
|---|---|
| Subscribers 1.8 | 4 |
| Subscribers 15.8 | 16 |
| Delta over two weeks | **+12** |
| Distribution actions taken in the window | **0** |
| Posts published 2.8 to 15.8 | 33 (ids 24 to 56) |
| Days with zero posts | 2 (9.8, 10.8) |
| Organic web mentions of the channel | 0 |
| Affiliate clicks | 0 (no affiliate links exist on this channel) |
| Revenue | 0 |

### Views by post age, not by wall clock

Reading a channel at one moment and ranking the numbers compares a 2-hour-old post to an 8-day-old one. Grouped by age instead:

| Cohort | Posts | Age at reading | Views | Mean |
|---|---|---|---|---|
| 8 days | 5 | 166-194h | 10, 8, 8, 9, 7 | **8.4** |
| 3-4 days | 7 | 70-102h | 5, 4, 3, 3, 3, 4, 7 | **4.1** |
| 2 days | 3 | 46-53h | 6, 7, 5 | **6.0** |
| 1 day | 3 | 22-30h | 6, 5, 5 | **5.3** |
| under 6h | 2 | 2-6h | 3, 2 | 2.5 |

The oldest cohort holds roughly twice the views of everything younger. The 3-to-4-day dip below its own juniors is two standard errors on Poisson counts of 3 to 7, on a comparison chosen after seeing the data, and the obvious explanation for it (those are the bulk emergency-refill posts) fails because one post from that same batch ties the channel record. Recorded as noise.

The single most useful number in the table is not in it: **the top post holds 10 views and the channel had about 8 subscribers on the day it published.** Reach is not capped by subscriber count at publication time, so views include traffic through the public web archive. This channel had been carrying a "every post must stand alone" rule since 4.8 on borrowed evidence from the Hebrew channel. It is no longer borrowed.

### What weeks 3 and 4 measured on the English channel

Could: the shape of view accrual, cleanly enough to promote a rule from inherited to tested, and to add a binding measurement rule (compare posts only at equal age) that three previous runs came close to violating.

Could not: anything about writing. Third consecutive report saying so. Thirty-three posts, sixteen subscribers, a total range of 2 to 10 that tracks age.

Did not intend to measure, and did: **+12 subscribers with zero distribution actions.** Eight days of active agent distribution in week 2 produced +2. Fourteen days of none produced +12. Every PR is unchanged since 24.7, no community post has ever been sent, the launch kit was untouched, and a web search for the channel name still returns nothing. The growth is unattributable and it has already stopped: flat at 16 for three consecutive days, the longest plateau in the channel's history, starting the moment the climb ended.

## Weeks 5 and 6, בינה בקטנה (HE) — 2026-08-16 to 2026-08-29

The weekly run of 22.8 died on `API Error: Connection closed mid-response`, so this covers a fortnight. That is the second weekly run lost to a transport error in six weeks; the 8.8 run died on `ENOTFOUND`.

| Metric | Value |
|---|---|
| Subscribers, start of window (16.8) | 110 |
| Subscribers, end of window (29.8) | **110** |
| Net change over 14 days | **0** (dipped to 109 for eight days, recovered 27.8) |
| Posts due | 42 (3 slots/day × 14 days) |
| Posts published | **42** |
| Slots missed | **0** |
| Posts published more than 2h after their slot | **8** |
| Distribution actions taken in the window | 0 |
| Affiliate clicks | 0 (no affiliate link exists on this channel) |
| Revenue | 0 |

The publishing reliability line is the one that changed. The previous window managed 8 posts out of 21. This one delivered 42 out of 42, the first fully clean fortnight in the channel's history.

### The correction that matters: three numbers, three different ages

Nine consecutive daily runs between 23.8 and 28.8 recorded "below the organic baseline of 24 to 31" and escalated the language each time — "the ninth consecutive measurement", "the pattern is stable enough that it can no longer be called weekend noise". Every one of those entries compared **views at 24 hours** against a baseline whose age was never established. The comparison was invalid.

Accrual was measured directly for the first time this window. Post 237 held 14 views at 4-10 hours, 20 at 24 hours, and 32 at six days. Posts 239 (18 → 32) and 244 (17 → 29) trace the same curve. **A post roughly doubles after its first day.**

| Measurement | n | Age at reading | Mean |
|---|---|---|---|
| Views at 24 hours, posts of 22-25.8 | 10 | 24h | **18.0** |
| The nine experiment-4 posts, as actually read | 9 | 48-96h | **20.0** |
| On-time posts of 23-26.8, read 29.8 | 13 | 2-6 days | **25.2** |

25.2 sits inside the 24-to-31 organic baseline set on 1.8. **At the post level, measured at comparable maturity, the channel has not decayed at all.** What did fall is the first-day read: 18.0 now against roughly 28 in early August, down about 36 percent. Three posts at 18 is 54 views a day against 28 for a single post, so total daily reach roughly doubled while per-post first-day attention dropped.

### Views by slot, on-time posts only, at 2-6 days

| Slot (UTC) | Posts | Mean |
|---|---|---|
| 06:00 | 4 | 26.3 |
| 10:00 | 5 | 24.6 |
| 17:30 | 4 | 25.0 |

A 7 percent spread against a pre-registered 30 percent threshold. This is the third consecutive result pointing the same way, and the question is now closed rather than deferred.

### The scheduler degraded and nothing alarmed

Measured from `gh run list`: through the evening of 26.8 the hourly cron fired at 0.8-to-1.6-hour intervals as designed. From 26.8 22:50 UTC onward the gaps between consecutive runs were 5.5, 5.7, 9.1, 12.6, 9.5, 6.7, 6.9 and 4.1 hours. **Every run that did fire returned success.** GitHub simply stopped delivering the trigger.

Eight posts landed 3.0 to 7.9 hours late. Post 254 went out at 02:27 local time. Posts 252 and 253 were sent in the same minute, so a reader got two notifications back to back. Publishing self-heals on the next run, so nothing was lost — but every slot comparison in the window is contaminated, and the low view counts on posts 252 through 256 are a function of send hour and age, not content.

### What weeks 5 and 6 measured

Could: publishing reliability, decisively — 42 of 42. And the accrual curve, which retired a false conclusion that nine daily runs had been reinforcing.

Could not: anything about writing. Fourth consecutive report saying so. Ninety-four posts in, the range is still a narrow band that tracks age and nothing else.

Did not intend to measure, and did: **the system's own daily commentary was the least reliable input this window.** Nine runs escalated a measurement artifact into a near-recommendation to cut the publishing cadence. The guardrail that caught it was not a smarter agent; it was a pre-registered threshold, read literally, landing at 20.0 in a band whose written instruction was "continue and report, do not recommend a change."

## Weeks 5 and 6, Claude Code Daily (EN) — 2026-08-16 to 2026-08-29

No weekly run happened on 22.8, the same gap as the Hebrew channel, so this is a two-week report.

| Metric | Value |
|---|---|
| Subscribers 15.8 | 16 |
| Subscribers 29.8 | 19 |
| Delta over two weeks | **+3** |
| Delta over the *previous* two weeks | +12 |
| Distribution actions taken in the window | **0** |
| Posts published 16.8 to 29.8 | 41 (ids 58 to 98) |
| Scheduled slots missed | **0** |
| Organic web mentions of the channel | **0**, sixth consecutive week |
| Affiliate clicks | 0 (no affiliate links exist on this channel) |
| Revenue | 0 |

### The experiment that closed, and the number that mattered was not the one it asked for

Experiment 4 asked whether the previous fortnight's +12, which arrived with nobody doing anything, was a live organic source or one source emptying. Thresholds were pre-registered on 15.8: 25 or more subscribers on 23.8 meant real, 17 to 24 meant weak drift, 16 or fewer meant the plateau was the truth. **The reading on 23.8 was 18: weak drift, the middle band.**

The band was honored as written. But the fortnight totals answer the question better than the checkpoint did. Same conditions, zero distribution both times:

| Fortnight | Subscribers | Delta |
|---|---|---|
| 1.8 to 15.8 | 4 → 16 | **+12** |
| 15.8 to 29.8 | 16 → 19 | **+3** |

**The +12 was an event, not a rate.** The rate is roughly one subscriber every four or five days, and it fell fourfold while the archive grew from 56 posts to 98. Acquisition did not compound with volume; it declined.

### Ninety-eight posts, and the web has never heard of the channel

A search for the channel handle returned zero organic mentions for the sixth consecutive week. The public archive is live and machine-readable, and after 36 days and 98 posts no search engine has indexed it. Two directory listings are live and neither is findable.

**Publishing volume is buying no discovery surface outside Telegram at all.** Whatever the acquisition source is, it is Telegram-internal, and writing more posts does not feed it. This is the most decision-relevant finding of the fortnight and it points away from the thing the system is good at.

### The accrual curve, measured on this channel for the first time

Individual posts tracked across repeated readings, rather than one sweep ranked by number:

| Post | First hours | ~24h | Settled |
|---|---|---|---|
| 78 | 4 (20h) | 7 (44h) | 7 (92h) |
| 79 | 2 (3h) | 5 (28h) | 7 (6d) |
| 88 | 2 (2h) | 4 (16h) | 5 (40h) |
| 89 | 4 (2h) | 5 (12h) | 6 (36h) |

**A post roughly doubles between its first hours and 24 hours, adds up to 40 percent more by day 6, and is settled by then.** This is the same shape the Hebrew channel measured this fortnight at roughly six times the audience, which is mild evidence it is a Telegram behaviour rather than a channel one.

The mature cohort (ids 79 to 89, read at 3 to 6 days) means **4.55 views**, range 2 to 7, against 4.1 for the comparable cohort a fortnight ago at 16 subscribers. Flat.

### Publishing: perfect on delivery, degraded on timing, blind in one path

41 of 41 slots delivered, the second clean fortnight running. Mean lateness 1.02h, with three posts over two hours late (5.33h, 7.46h, 3.46h), all in the 27.8 to 28.8 window, the same GitHub cron degradation the Hebrew channel measured. Two of them were sent in the same minute, so a subscriber got two notifications back to back at 02:27 local time.

**Three posts have no entry in the publish log at all.** They went out through the Mac rescue path, which deletes the scheduled file after sending and records nothing. The log shows 38 sends for a fortnight that delivered 41. The hole is in the rescue path, so it under-reports delivery in precisely the situation where delivery is most in doubt.

### What weeks 5 and 6 measured on the English channel

Could: the organic-growth question, decisively enough to close it. There is a source, it is small, and it is fading. And the accrual curve, independently derived.

Could not: anything about writing. **Fourth consecutive report saying so.** Ninety-eight posts, nineteen subscribers, a mature range of 2 to 7 that tracks age. This is no longer a data problem to be solved by another week of the same; the channel will not produce a usable writing signal at this size.

Did not intend to measure, and did: **the loop spent four consecutive daily runs investigating three posts that were not old enough to read.** Ids 84 to 86 were called "genuinely stuck at 2 views"; two of them moved the next day. The remaining one was then investigated alone and is a clean post sitting two views below its neighbours, which at 19 subscribers is two people. The wrong conclusion self-corrected in a day. What did not self-correct is that each run cited the number of previous runs as corroboration.

## Weeks 7, 8 and 9, בינה בקטנה (HE) — 2026-08-30 to 2026-09-19

Three weeks in one report, because the weekly loop fired on time on 5.9 and on 12.9 and died before writing a line, both times silently. See `lessons.md`.

| | Week 7 (30.8-5.9) | Week 8 (6.9-12.9) | Week 9 (13.9-19.9) |
|---|---|---|---|
| Slots delivered | 20 / 21 | 18 / 21 | **11 / 21** |
| Mean lateness | 2.41h | 2.37h | 2.47h |
| Posts over 2h late | 12 | 10 | 7 |
| Subscribers at week end | 112 | 113 | **114** |

Subscribers: **110 on 29.8, 114 on 19.9. Plus four in three weeks, across 49 published posts.**

### The cadence question, answered on 38 posts instead of two days

This is the question that has been open since 12.8, when the channel moved to three posts a day against the only data available. All posts below were read on 19.9 at a uniform mature age.

| Cohort | n | Age at read | Mean views |
|---|---|---|---|
| 30.8 to 5.9 | 20 | 14-20 days | **30.6** |
| 6.9 to 12.9 | 18 | 7-13 days | **29.3** |
| Organic baseline set 1.8, at one post per day | 4 | mature | **24 to 31** |

**Both weeks sit inside the baseline, not below it.** Three posts a day did not dilute per-post views. Daily exposure is roughly 90 views against roughly 28 at one post a day, at no cost to the individual post. Experiment 4 closed at exactly 20.0 on nine posts and two days; this is the same question at n=38 and it answers cleanly in the other direction.

### Experiment 5 (mini-guide vs regular tip): void, and closed permanently

The experiment carried a pre-written disqualification: *more than three of 21 posts landing over two hours late voids the measurement*. Actual: **20 of 21 published, 12 of them over two hours late**, mean lateness 2.41h, max 6.80h. The condition fired at four times the threshold.

Second, independent failure: the design required three mini-guides; **two were written**. The Sunday slot got a 111-word regular tip.

Descriptive numbers anyway, explicitly not evidence, all 20 posts at a uniform 14-20 days:

| Group | n | Mean |
|---|---|---|
| Mini-guides | 2 | 32.0 |
| Regular tips | 18 | 30.4 |

Plus 5.1 percent, deep inside the pre-written "not significant" band. The question was opened on 24.7, deferred on 1.8, deferred again on 15.8, and contaminated today. **Three consecutive attempts died because the infrastructure would not let the question be asked. It will not be asked a fourth time.**

### Reliability is the only constraint that is actually costing anything

**49 of 63 slots, 78 percent.** The large hole: four days of total silence, 12-15.9, after the Mac's `claude -p` OAuth session expired on 11.9 and killed every scheduled task system-wide, not just this channel. Fixed on 15.9 by moving to a one-year token.

The small persistent hole: the GitHub Actions cron throttle, open since 26.8, now in its fourth week. Mean lateness is a stable ~2.4 hours in all three weeks. Every run that fires ends in success; they simply are not fired on the hour.

**A gap recorded on 29.8 and still open:** the English channel has three Mac-side safety nets that check whether a cloud slot went out and rescue it if not. The Hebrew channel has none.

### What weeks 7 to 9 measured

Could: the cadence question, decisively, at n=38 and mature age. It is closed.

Could not: anything about writing. **Sixth consecutive report saying so**, now at 143 posts.

Did not intend to measure, and did: **the learning loop is itself an unalarmed single point of failure.** Two consecutive weeks it fired, failed, and logged the failure to a file nobody reads. The scheduler recorded both as "run".
