# elonmusk-repost-skill

A prompt/skill that **scores how well your content matches patterns Elon Musk (@elonmusk) tends to repost on X**, then **generates tweet drafts optimized for engagement/repost** (plus recommended media and posting strategy).

- **What you get**: a 0–100 “Repost Score” breakdown, 3 tweet variants you can post immediately, suggested media (video/GIF/screenshot), and timing/thread guidance.
- **Best for**: AI product launches, visual demos, AI agents, interactive/playable projects, traction milestones, and “challenger” positioning vs incumbents.

> Disclaimer: This project is based on public behavior patterns. It does not guarantee reposts. Not affiliated with X/xAI/Tesla/SpaceX.

---

## Install

```bash
npx skills add https://github.com/mingyouagi/elonmusk-repost-skill --skill elonmusk-repost
```

> Replace the repo URL with the actual GitHub URL if you've forked this.

---

## Quickstart

The core artifact is a single file:

- `SKILL.md`: triggers, workflow, scoring rubric, templates, and output format.

### Usage A: Drop into your agent / prompt library

1. Put `SKILL.md` into your prompts/skills directory (e.g. `skills/`, `prompts/`, `system-prompts/` — depends on your stack).
2. Load it into your agent (or make it retrievable).
3. Trigger it by intent (e.g. “musk repost”, “viral X post”) or explicitly: “Follow `SKILL.md` and produce the standard output.”

### Usage B: Manual (no framework required)

Use `SKILL.md` as your system/workflow prompt and ask the model:

- “Follow `SKILL.md`: ask me the 4 intake questions, score fit for @elonmusk repost patterns, then generate 3 tweet variants + recommended media + posting strategy.”

---

## What to prepare (recommended)

To maximize “wow factor”, provide:

- **Project/product name**
- **One-sentence description**
- **A visual demo** (video/GIF/screenshot) — strongly recommended
- **Links** (landing page, demo, waitlist, video) — optional but helpful
- **Hard metrics** (users, growth, speed, cost comparison) — optional

---

## Output format

By default, the skill produces:

1. **Repost Score (0–100)** with a weighted breakdown (e.g. AI Visual Demo, AI Agent, Wow Factor, Playable, Grok/xAI adjacency)
2. **3 tweet variants** using different templates (launch / milestone / challenger / pure demo)
3. **Recommended media** to attach
4. **Posting strategy** (timing, thread structure, where to put the link)
5. **Risk assessment + improvement suggestions**

---

## Best practices (high impact)

- **Lead with the demo, not the pitch**: first tweet should be instantly understandable
- **Keep it tight**: aim for < 50 words (similar information density)
- **Don’t beg-tag**: mention @elonmusk only when it feels organic
- **Avoid hashtag spam**
- **Thread tactic**: Tweet 1 = hook + demo; Reply 1 = link + details + metrics

---

## Copy‑paste prompts

- “Here’s my product: … (one sentence). I have a 20s demo video. Follow `SKILL.md`: score fit for @elonmusk repost patterns, then generate 3 tweet variants + recommended media + posting strategy.”

---

## Files

- `SKILL.md`: the skill definition (workflow + rubric + templates)
- `README.md`: this file

---

## License

No license file is included yet. If you want this to be truly open source, add a `LICENSE` (MIT / Apache-2.0 / etc.) based on your preference.

