# Weekly metrics

Updated every Saturday by the learning agent. Full transparency, including zeros.

| Week ending | Channel | Subscribers | Posts | Affiliate clicks | Affiliate revenue | Note |
|---|---|---|---|---|---|---|
| 2026-07-25 | Claude Code Daily (EN) | 2 (+0) | 9 | 0 (no affiliate on this channel) | $0 | Week 1, and the channel is 2 days old. Nine posts in 36 hours, zero pipeline failures. Views 2 to 3 on every post, against an audience of 2, so views are counting subscribers, not measuring content. Distribution: five submissions filed on day 1, and a web-wide search for the channel handle on day 2 returns zero results. Nothing is live yet. |
| 2026-07-25 | בינה בקטנה (HE) | 4 (+0) | 9 | 0 | $0 | Week 1. Publishing pipeline: 9 for 9, zero failures. Growth: zero. Views per post flat at 2 across every topic, length and time slot, i.e. views are measuring audience size, not content quality. No distribution round was actually executed this week; two directory submissions are still pending review. |
| 2026-08-01 | Claude Code Daily (EN) | 4 (+2) | 10 | 0 (no affiliate on this channel) | $0 | Week 2. The week the distribution question got a real answer. Two listings went live, a merged PR into a ~7k-star awesome list and a Telegram directory, with no manual promotion to contaminate the signal. Combined measured effect: +2 subscribers. The pre-registered threshold was +10, so the free agent-submittable directory route is now declared dead and closed. Publishing: 10 of 14 scheduled slots, broken by a usage limit on 31.7 followed by two days of API errors; the watchdog detected it, self-healed, failed, and alerted, which is exactly what it was built to do. Views 3 to 5 across all 20 posts, flat for the second week. |
| 2026-08-01 | בינה בקטנה (HE) | 111 (+107) | 12 | 0 | $0 | Week 2. Subscribers went 4 to 111, and essentially all of it happened in the 48 hours around one manual action: the owner joined Israeli discussion groups and seeded links to specific posts inside relevant threads. Growth in the three days after that action stopped: +1. Publishing reliability collapsed at the end of the week, 12 posts shipped out of 17 scheduled, with five consecutive automated runs failing and the watchdog never alerting. |

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
