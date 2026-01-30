# X Writer Skill

Felix's dedicated X (Twitter) writing assistant - generates tweets in authentic voice for AI practitioners, product builders, and entrepreneurs.

## Quick Start

**Activate the skill:**
```
/x-writer
```

**Or simply tell Claude:**
```
"I want to write a tweet about [topic]"
```

---

## What This Skill Does

1. **Interviews you** to extract core claim, proof, and CTA
2. **Selects best formula** from 5 proven tweet structures
3. **Generates 3 versions**:
   - Version A: Zinger (50-150 chars) - viral potential
   - Version B: Thread Opener (180-250 chars) - persuasive depth
   - Version C: Playbook (200-280 chars) - authority building
4. **Runs quality checks** before delivery
5. **Saves approved version** to your writing drafts

---

## Input Formats Supported

**Minimal:**
```
"Write about Claude Code enabling solo founders"
```

**With context (Chinese OK):**
```
"写一条推文：以前需要10人团队，现在1人+AI就够了。我就是例子。"
```

**Full brief:**
```
"Tweet about how 2026 is the year for solo founders. Claim: AI made 1 person = 10 person team. Proof: I've shipped 7 apps solo. CTA: Stop looking for co-founder, start building."
```

---

## The 5 Formulas

| Formula | Use When | Example |
|---------|----------|---------|
| **Generational Shift** | Time-based change | "2020 vs 2026: The math changed" |
| **Counterintuitive Truth** | Challenge consensus | "Everyone thinks X. Wrong." |
| **Data Bomb** | Surprising number/pattern | "Just saw: 90% of..." |
| **Step-by-Step Playbook** | How-to advice | "My 3-step framework:" |
| **Identity Filter** | Mindset/values | "Some people... Other people..." |

---

## Example Session

**You:**
```
想写一条关于AI工具让solo founder更强的推文
```

**AI:**
```
Got it - tweet about AI empowering solo founders.

Quick questions:
1. What's the specific change? (e.g., speed, capability, cost)
2. Do you have proof? (personal experience, data, or example?)
3. What should readers DO?
```

**You:**
```
1. 以前要10人团队，现在1人+Claude Code就够
2. 我自己就是证明，今年一个人发了7个app
3. 让大家停止找co-founder，直接build
```

**AI:**
```
Perfect. Using **Formula 1: Generational Shift**.

**Version A: Maximum Impact (98 chars)**
2020: need 10 people to build an app
2026: 1 person + Claude Code

The math changed. The game changed.

*Use for: Standalone tweet, max virality*

---

**Version B: Balanced Thread Opener (234 chars)**
Everyone says "find a co-founder first."

Wrong.

2020 you needed a team. 2026 you need Claude Code.

I shipped 7 apps solo this year that would've taken 10 people in 2020.

Stop looking for a co-founder. Start building. Hire when you hit revenue.

*Use for: Thread starter, persuasive argument*

---

**Version C: The Playbook (267 chars)**
Solo founders ask: "Should I find a co-founder or stay solo?"

My playbook:
1. Stay solo for 90 days
2. Ship 3 MVPs using Claude Code
3. If one hits → hire. If not → you saved 50% equity

Most co-founder problems = "I'm afraid to build alone."
AI fixed that.

*Use for: Authority building, actionable advice*

---

Which version fits your goal?
```

---

## Output Location

Approved tweets save to:
```
00_Inbox/writing draft/YYYY-MM-DD-X-[topic].md
```

Example:
```
00_Inbox/writing draft/2026-01-13-X-solo-founder-claude.md
```

---

## Key Features

✅ **Bilingual input** - Give context in Chinese or English
✅ **Smart interviewing** - Extracts what's missing from your input
✅ **Formula-driven** - Uses proven structures, not guesswork
✅ **3 versions always** - Different lengths for different contexts
✅ **Quality-checked** - Runs 6-point checklist before delivery
✅ **Fast** - 5 minutes from idea to 3 polished tweets

---

## Voice Characteristics

This skill writes in **Felix's authentic X voice**:
- Direct, no fluff ("Wrong." not "I respectfully disagree")
- Proof-driven (specific numbers, names, examples)
- Builder-focused (for people who ship, not theorists)
- Urgent ("right now matters", "window is closing")
- Authority from experience ("I've sold 3 startups...")

**Signature elements:**
- "lock in", "ship", "taste freedom", "vibe coding"
- ALL CAPS for quotable phrases
- Short punchy sentences
- No hedge words ("maybe", "I think")

---

## Tips for Best Results

**DO:**
- ✅ Give specific claims, not vague themes
- ✅ Include personal experience or data
- ✅ Know your CTA (what should readers do?)
- ✅ Iterate - pick a version, then tweak if needed

**DON'T:**
- ❌ Say "write about AI in general"
- ❌ Skip the interview questions
- ❌ Ask for generic motivational content
- ❌ Expect LinkedIn-style corporate voice

---

## Comparison: X vs 小红书

| Feature | X Writer | XHS Writer |
|---------|----------|------------|
| **Language** | English | Chinese |
| **Length** | 50-280 chars | 800-1500 chars |
| **Output** | 3 tweet versions | 1 article + 3 titles |
| **Style** | Direct, urgent | Deep analysis |
| **Format** | Short zingers | Long-form narrative |
| **Audience** | Solo builders, AI practitioners | Chinese entrepreneurs, B2B |

---

## Related Files

- **Formula library:** `[[01_Projects/X_skill/02_核心配方生成/X爆款结构.md]]`
- **Detailed workflow:** `[[01_Projects/X_skill/X_writer.md]]`
- **Tweet samples:** `[[00_Inbox/X_Samples/X.md]]`

---

**Ready to ship some tweets?**

Just say: *"I want to write about [your topic]"*
