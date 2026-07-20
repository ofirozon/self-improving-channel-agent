# Architecture

## Constraints (chosen deliberately)

- Runs entirely on a personal Mac via `launchd`; no cloud infrastructure, no paid APIs.
- Uses a consumer Claude subscription (`claude -p` headless runs) as the only intelligence layer.
- The publisher Telegram bot is **broadcast-only**: it never polls for updates and is never wired into any conversational loop. Its token lives in an isolated env file (chmod 600), separate from any other automation.

## Components

| Component | Role |
|---|---|
| Daily content agent (20:30) | Web research → pick one high-value topic → write a Hebrew post per the *current* guidelines → publish → log post + subscriber count |
| Weekly learning agent (Sat 21:00) | Analyze the week → close the open experiment, open a new one → rewrite the writing guidelines if evidence justifies it → update this repo → send the owner an honest report |
| Writing guidelines file | The system's "prompt DNA". Versioned, with a changelog. An immutable "hard rules" section the learning loop may not touch. |
| Experiment log | One experiment at a time: hypothesis, metric, decision threshold, result, decision. |
| Publish script | Thin shell wrapper over the Bot API with a final guardrail check before sending. |

## Human in the loop

- Weeks 1-2: every post is delivered to the owner as a draft for one-tap approval (`PUBLISH_MODE=draft`).
- After that: fully automatic (`PUBLISH_MODE=auto`), with a weekly human checkpoint (~15 min): read the report, check the affiliate dashboard, approve the LinkedIn draft.

## Measurement honesty

The Bot API exposes subscriber count but not per-post views. The system tracks what is actually measurable (subscribers, posts, manually-read affiliate clicks) and is explicitly instructed to say "not statistically meaningful" rather than invent patterns from small numbers.
