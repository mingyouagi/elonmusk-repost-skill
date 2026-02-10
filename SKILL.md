---
name: elonmusk-repost
description: Analyze Elon Musk's repost patterns on X and generate tweets optimized for getting reposted by @elonmusk. Use when users want to craft viral AI/tech product launches targeting Musk's attention.
category: technique
triggers: [musk, repost, retweet, viral tweet, x post, twitter, elonmusk]
version: "1.2"
author: mingyouagi
last_updated: 2026-02-10
---

# Elon Musk Repost Skill

Analyze what Elon Musk reposts on X and generate tweets optimized for his engagement.

## How to Use

When invoked, **go straight to scoring and tweet generation in a single response**. Do NOT ask clarifying questions unless critical info is truly missing (no product name AND no description at all). Extract everything you can from the user's message — product name, what it does, media, metrics, draft text — and immediately produce the full output (score + tweets + strategy).

**Speed is critical.** The user expects one message in, one message out. Never split the analysis across multiple turns.

### What to extract from the user's message:
- Product/project name
- What it does
- Demo URL, video, or visual hook (if mentioned)
- Any draft tweet text they've already written
- Traction metrics (if mentioned)

If the user provides a draft tweet, score THAT draft and generate improved variants.

## Step 2: Musk Repost Pattern Analysis

### Core Repost Triggers (Score each 0-10)

Evaluate the user's content against these proven patterns:

| Pattern | Weight | Description |
|---------|--------|-------------|
| **AI Visual Demo** | 10 | Visually stunning AI-generated output (images, video, 3D, games) |
| **AI Agent** | 9 | Autonomous AI that completes complex tasks end-to-end |
| **"Wow Factor"** | 9 | Instantly impressive, no explanation needed |
| **Robotics / Physical AI** | 9 | Humanoid robots, embodied AI, real-world autonomous systems |
| **Video / Multimodal Generation** | 8 | AI-generated video, voice, music, or cross-modal output |
| **Playable/Interactive** | 8 | Users can try it immediately (game, tool, demo) |
| **Grok/xAI Adjacent** | 8 | Content that relates to or complements Grok capabilities |
| **Open-Source AI** | 7 | Open-weight models, open-source tools (Musk pushed Grok open-source) |
| **Underdog / Unexpected Origin** | 7 | Surprising team origin — small team, non-obvious country, solo dev |
| **Creator Tool** | 7 | Empowers individuals to create professional-grade output |
| **Speed/Scale** | 6 | "X million users in Y hours" type virality metrics |
| **Government Efficiency / DOGE** | 6 | Tools that cut bureaucratic waste or align with efficiency themes |
| **Meme Potential** | 6 | Content that can be remixed into memes |
| **Anti-Establishment** | 5 | Challenges incumbents (Adobe, Google, OpenAI, etc.) |
| **Space / Mars** | 5 | Space exploration, Mars colonization, rocket tech |

### Scoring Formula

```
For each pattern the content matches:
  match_score(i) = relevance(0-10) × weight(i)

Repost Score = Σ match_score(i) / Σ weight(i) for ALL patterns × 100
```

- `relevance` = how strongly the content matches that pattern (0 = no match, 10 = perfect match)
- `weight` = the number in the table above
- Denominator uses ALL 15 patterns (sum of all weights = 108), so a perfect score requires hitting every pattern at 10/10.
- In practice, 70+ is strong; 85+ is exceptional.

### Reference Scores (for calibration)

| Product | Score | Key Patterns Hit |
|---------|-------|-----------------|
| Lovart (AI Design Agent) | 81 | AI Visual Demo, AI Agent, Underdog, Creator Tool, Speed/Scale, Wow, Anti-Establishment |
| Loopit (AI Game Gen) | 79 | Playable, AI Visual Demo, Underdog, Creator Tool, Wow, Grok Adjacent |
| Midjourney | 78 | AI Visual Demo, Wow, Creator Tool, Anti-Establishment, Speed/Scale, Meme |
| Suno (AI Music) | 76 | AI Visual Demo, Wow, Multimodal, Creator Tool, Playable, Meme |
| Manus (AI Agent) | 74 | AI Agent, Underdog, Wow, Speed/Scale |
| DeepSeek | 73 | Open-Source, Underdog, Anti-Establishment, Wow, Speed/Scale |
| Cursor (AI Code Editor) | 72 | AI Agent, Wow, Creator Tool, Anti-Establishment, Speed/Scale, Grok Adjacent |

Products scoring 70+ all share: strong visual demo OR autonomous agent + wow factor. Products below 50 typically lack visual impact.

### What Musk Ignores (Anti-Patterns)

Avoid these — they virtually guarantee being ignored:

- 🚫 **Beg-tagging**: "@elonmusk PLEASE see this!! 🙏🙏🙏"
- 🚫 **Hashtag spam**: #AI #MachineLearning #Startup #Tech #Innovation
- 🚫 **Wall of text with no visual**: Long explanations, no demo
- 🚫 **Obvious paid promotion / shill tone**: "This amazing product will change everything!!!"
- 🚫 **Political hot-takes unrelated to tech**: Partisan rants with no tech substance
- 🚫 **Copycat / derivative products**: "Like ChatGPT but…" with no unique angle
- 🚫 **Excessive self-promotion**: Multiple @elonmusk tags in the same thread
- 🚫 **Low-effort screenshots**: Static UI screenshots with no motion or interaction

## Step 3: Generate Optimized Tweets

### Tweet Formula

Based on analysis of content Musk engages with, use this structure:

```
[Hook - 1 line, max impact] + [Visual media] + [Optional: metric/claim]
```

### Rules for Musk-Optimized Tweets

1. **Lead with the demo, not the pitch** - Show, don't tell
2. **Keep text under 50 words** - Musk engages with brief, punchy content
3. **Attach video/GIF** - Visual content gets 10x more engagement
4. **Use superlatives carefully** - "World's first X" works if defensible
5. **Tag @elonmusk only if organic** - Don't beg; make content worth sharing
6. **Post timing** - See timing windows below
7. **Thread format** - First tweet = hook + demo, reply with details
8. **No hashtags** - Musk never engages with hashtag-heavy posts
9. **Mention Grok/xAI angle if relevant** - "Built with Grok" or "Works with Grok" increases odds
10. **Include virality metric if available** - "1M users in 24 hours" type stats

### Posting Timing Windows (US Pacific)

| Window | Time (PT) | Notes |
|--------|-----------|-------|
| **Prime** | 10 PM – 2 AM | Musk's late-night scroll; highest engagement probability |
| **Secondary** | 6 PM – 10 PM | Evening wind-down; decent reach |
| **Weekend** | Sunday 8 PM – 1 AM | Variable but Sunday evening is consistently strong |
| **Avoid** | 6 AM – 12 PM | Low engagement; posts get buried before Musk is active |

### Tweet Templates

**Template A: Product Launch**
```
[Product Name] — [bold claim in ≤8 words]

[1-2 sentence description of what it does]

[Attach: 30-60s demo video or GIF]
```

Example:
```
Lovart — the world's first AI design agent.

Give it a brief. It delivers agency-grade creative in minutes.
20,000 people queued on launch day.

[45s demo video attached]
```

**Template B: Milestone/Traction**
```
[Metric] in [timeframe].

[Product Name] lets you [core value prop].

[Attach: demo video showing the "wow" moment]
```

Example:
```
1M songs created in 72 hours.

Suno turns a one-line prompt into a full, radio-quality track.

[30s audio/video demo attached]
```

**Template C: Challenge the Status Quo**
```
[Incumbent] charges $X/mo for [thing].

[Product Name] does it with AI for [fraction of price / free].

[Attach: side-by-side comparison video]
```

Example:
```
Adobe charges $55/mo for design tools most people never learn.

Lovart does it with one sentence for $9/mo.

[side-by-side comparison: 2 hours in Photoshop vs 30 seconds in Lovart]
```

**Template D: Pure Demo (Highest Conversion)**
```
[No text or minimal text — just the demo video/GIF]

[Reply to own tweet with product name + link]
```

Example:
```
[60s screen recording: type a prompt → watch a playable 3D game appear in real-time]

↳ Reply: "This is Loopit. Try it → loopit.ai"
```

**Template E: Reply to Musk's Tweet**
```
[Monitor Musk's tweets on a relevant topic]
[Reply with your demo + one punchy line — no @tag needed, you're already in his thread]
```

Example:
```
Musk tweets: "AI is getting insane"
↳ You reply: "Made a game in 10 seconds with pure AI. No code." + [15s GIF of Loopit generating a game]
```

This is often the **highest-conversion path** — you're already in his notification stream.

### Output Format

Produce ALL of this in a **single response** — no follow-up turns:

1. **Repost Score**: X/100 with a compact table (pattern | relevance | score). Only show patterns scoring >0.
2. **3 Tweet Variants**: Using different templates. Keep each tweet under 50 words.
3. **Media + Timing**: What to attach and when to post (2-3 lines max).
4. **How to Increase Score**: Top 3 actionable changes, with estimated score impact.

## Musk Engagement Style Reference

When Musk reposts or engages, his style is:
- Single word: "Wow", "Interesting", "True", "Cool"
- Single emoji: 🔥, 👀, 🤯
- Brief comment: "This is the future", "AI is moving fast"
- Quote tweet with minimal addition

Content that elicits these minimal-effort responses has the highest repost probability.

## Post-Publish Playbook (include as a brief checklist)

- **0–5 min**: Self-reply with link + one extra detail
- **5–30 min**: Engage with early replies
- **30–60 min**: DM 3–5 mutual followers for amplification
- **1–4 hours**: If no traction, reply to a relevant Musk tweet with the demo (Template E)
- **Next window**: Repost with a different template at the next Prime time (10 PM–2 AM PT)

Don't: beg-tag Musk, delete/repost repeatedly, or spam across accounts.

## Important Notes

- This skill analyzes public patterns; no guarantee of actual repost
- Musk's interests shift — AI/tech/robotics/efficiency is the current focus (2025-2026)
- Quality of the actual product matters more than tweet optimization
- Organic virality > manufactured virality
- The best strategy: build something genuinely impressive, then present it well
