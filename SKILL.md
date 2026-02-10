---
name: elonmusk-repost
description: Analyze Elon Musk's repost patterns on X and generate tweets optimized for getting reposted by @elonmusk. Use when users want to craft viral AI/tech product launches targeting Musk's attention.
category: technique
triggers: [musk, repost, retweet, viral tweet, x post, twitter, elonmusk]
version: "1.1"
author: mingyouagi
last_updated: 2026-02-10
---

# Elon Musk Repost Skill

Analyze what Elon Musk reposts on X and generate tweets optimized for his engagement.

## How to Use

When invoked, follow this workflow:

1. **Check prerequisites** - Verify account readiness
2. **Gather context** - Ask the user about their product/content
3. **Analyze fit** - Score how well it matches Musk's repost patterns
4. **Generate tweets** - Create optimized tweet drafts
5. **Plan post-publish** - Give a follow-up playbook

## Prerequisites (Account-Level)

Before optimizing tweet content, confirm the basics:

- Profile looks credible (real bio, avatar, some post history)
- At least a few hundred organic followers
- Account is not brand new (>30 days old)
- No recent spam/suspension flags

A zero-follower egg-avatar account will be ignored regardless of content quality.

## Step 1: Gather Product/Content Info

Ask the user:
- What is the product/project name?
- What does it do? (one sentence)
- Is there a demo URL or video?
- What's the visual hook? (screenshot, GIF, video)

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

### Successful Case Studies

**Lovart (AI Design Agent)** — Score: 81/100
- AI Agent: 9/10 × 9 = 81 — End-to-end design agent
- AI Visual Demo: 10/10 × 10 = 100 — Stunning design outputs
- Underdog Origin: 8/10 × 7 = 56 — LiblibAI (China), unexpected entrant
- Creator Tool: 8/10 × 7 = 56 — Agency-grade design for $90/mo
- Speed/Scale: 7/10 × 6 = 42 — 20,000 queued on day 1, 800K users in 2 months
- Wow Factor: 9/10 × 9 = 81 — "World's first Design Agent"
- Anti-Establishment: 6/10 × 5 = 30 — Challenges Adobe/Canva
- **Total: 446 / (7 matched patterns' max = 756) → normalized across all 15 → ~81/100**

**Midjourney** — Score: 78/100
- AI Visual Demo: 10/10 × 10 = 100 — Iconic AI image generation
- Wow Factor: 9/10 × 9 = 81 — Jaw-dropping visuals from text
- Creator Tool: 9/10 × 7 = 63 — Anyone can create stunning art
- Anti-Establishment: 7/10 × 5 = 35 — Challenges Adobe/stock photography
- Speed/Scale: 8/10 × 6 = 48 — 16M+ users, organic growth
- Meme Potential: 8/10 × 6 = 48 — Endless remixable output

**Cursor (AI Code Editor)** — Score: 72/100
- AI Agent: 8/10 × 9 = 72 — AI writes and edits code autonomously
- Wow Factor: 8/10 × 9 = 72 — "It just wrote the whole feature"
- Creator Tool: 9/10 × 7 = 63 — Turns anyone into a 10x developer
- Anti-Establishment: 8/10 × 5 = 40 — Challenges VS Code / JetBrains
- Speed/Scale: 7/10 × 6 = 42 — Explosive developer adoption
- Grok/xAI Adjacent: 5/10 × 8 = 40 — Coding + AI intersection

**Suno (AI Music)** — Score: 76/100
- AI Visual Demo: 8/10 × 10 = 80 — Audio is the "visual"; instantly shareable
- Wow Factor: 9/10 × 9 = 81 — Full songs from a text prompt
- Video/Multimodal: 9/10 × 8 = 72 — Audio generation, cross-modal AI
- Creator Tool: 9/10 × 7 = 63 — Anyone can make radio-quality music
- Playable/Interactive: 8/10 × 8 = 64 — Try it instantly, share results
- Meme Potential: 8/10 × 6 = 48 — Meme songs go viral

**Loopit (AI Game Generator)** — Score: 79/100
- Playable/Interactive: 9/10 × 8 = 72 — "Make everything playable"
- AI Visual Demo: 9/10 × 10 = 90 — AI-generated mini-games
- Underdog Origin: 8/10 × 7 = 56 — SeedLeap (China)
- Creator Tool: 8/10 × 7 = 56 — Anyone can create games
- Wow Factor: 9/10 × 9 = 81 — Instant game generation
- Grok/xAI Adjacent: 6/10 × 8 = 48 — Aligns with Musk's AI gaming interest

**DeepSeek** — Score: 73/100
- Open-Source AI: 10/10 × 7 = 70 — Fully open-weight LLM
- Underdog Origin: 9/10 × 7 = 63 — Chinese hedge fund → top-tier LLM
- Anti-Establishment: 8/10 × 5 = 40 — Challenges OpenAI
- Wow Factor: 9/10 × 9 = 81 — GPT-4 performance at a fraction of cost
- Speed/Scale: 7/10 × 6 = 42 — Viral global adoption

**Manus (AI Agent)** — Score: 74/100
- AI Agent: 9/10 × 9 = 81 — General-purpose autonomous agent
- Underdog Origin: 8/10 × 7 = 56 — Chinese team
- Wow Factor: 9/10 × 9 = 81 — End-to-end autonomous task completion
- Speed/Scale: 7/10 × 6 = 42 — Viral launch, invite-only hype

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

For each generation, provide:

1. **Repost Score**: X/100 with per-pattern breakdown (show the math)
2. **3 Tweet Variants**: Using different templates above
3. **Recommended Media**: What visual to attach (format, length, content)
4. **Posting Strategy**: Best time window, thread structure, follow-up plan
5. **Risk Assessment**: What could prevent a repost
6. **Improvement Suggestions**: How to increase the score

## Musk Engagement Style Reference

When Musk reposts or engages, his style is:
- Single word: "Wow", "Interesting", "True", "Cool"
- Single emoji: 🔥, 👀, 🤯
- Brief comment: "This is the future", "AI is moving fast"
- Quote tweet with minimal addition

Content that elicits these minimal-effort responses has the highest repost probability.

## Step 4: Post-Publish Playbook

After posting, follow this sequence:

1. **0–5 min**: Reply to your own tweet with link + one extra detail or metric
2. **5–30 min**: Engage with early replies; like/retweet anyone who shares it
3. **30–60 min**: DM or tag 3–5 relevant mutual followers to start organic amplification
4. **1–4 hours**: If no traction, reply to a relevant Musk tweet with the same demo (Template E)
5. **4–12 hours**: If still no traction, consider reposting at the next Prime timing window with a different template
6. **Next day**: Analyze impressions; iterate on the hook or media if engagement was low

**Do not**:
- Delete and repost the same tweet repeatedly
- Tag Musk in follow-up tweets if the first one didn't land
- Spam the same content across multiple accounts

## Important Notes

- This skill analyzes public patterns; no guarantee of actual repost
- Musk's interests shift — AI/tech/robotics/efficiency is the current focus (2025-2026)
- Quality of the actual product matters more than tweet optimization
- Organic virality > manufactured virality
- The best strategy: build something genuinely impressive, then present it well
