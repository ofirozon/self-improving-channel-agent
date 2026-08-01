# Weekly metrics

Updated every Saturday by the learning agent. Full transparency, including zeros.

| Week ending | Channel | Subscribers | Posts | Affiliate clicks | Affiliate revenue | Note |
|---|---|---|---|---|---|---|
| 2026-07-25 | Claude Code Daily (EN) | 2 (+0) | 9 | 0 (no affiliate on this channel) | $0 | Week 1, and the channel is 2 days old. Nine posts in 36 hours, zero pipeline failures. Views 2 to 3 on every post, against an audience of 2, so views are counting subscribers, not measuring content. Distribution: five submissions filed on day 1, and a web-wide search for the channel handle on day 2 returns zero results. Nothing is live yet. |
| 2026-07-25 | בינה בקטנה (HE) | 4 (+0) | 9 | 0 | $0 | Week 1. Publishing pipeline: 9 for 9, zero failures. Growth: zero. Views per post flat at 2 across every topic, length and time slot, i.e. views are measuring audience size, not content quality. No distribution round was actually executed this week; two directory submissions are still pending review. |
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
