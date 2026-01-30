---
name: x-writer
description: Felix's X (Twitter) writing assistant for AI practitioners, product builders, and entrepreneurs
version: 1.0.0
---

# Felix's X Writer

## Core Capability
A highly customized writing tool that generates tweets in Felix's authentic voice - direct, urgent, proof-driven content for builders.

## Dependencies
This skill relies on the following knowledge base. **Load strategically to avoid context explosion**:

1. **Personal Branding (Required)** - ⭐ Must read
   - Path: `01_Projects/Felix_Personal_Branding_Overseas.md`
   - Purpose: **Felix's positioning, core beliefs, voice guidelines, target audience**
   - Includes:
     - Core identity & value proposition
     - Contrarian views & philosophical stance
     - Writing tone & forbidden phrases
     - Target audience & anti-audience
     - Content themes & recurring motifs
   - **Critical**: Read before Step 1 to understand Felix's brand DNA
   - Token cost: ~4,000 tokens

2. **Formula Library (Required)** - Must read
   - Path: `01_Projects/x_skill/02_核心配方生成/X爆款结构.md`
   - Purpose: Access the 5 tweet formulas, quality checklist, and voice elements
   - Token cost: ~2,000 tokens

3. **Sample Index (Reference)** - Read first if samples needed
   - Path: `.claude/skills/x-writer/samples/README.md`
   - Purpose: Understand when and how to access samples
   - Token cost: ~1,000 tokens

4. **Tweet Samples (❌ DO NOT auto-load)** - Only with user request
   - Path: `00_Inbox/X_Samples/X.md`
   - Size: 412KB (~30,000 tokens)
   - ⚠️ **NEVER read automatically**
   - ⚠️ **Only use Grep to search, or Read with offset/limit**
   - When: User asks "show me my past tweets about X" or "write like that tweet I did about Y"

## Workflow Instructions

### Step 0: Context & Brand Loading (Mandatory)

**Before starting the interview:**

1. **Load Personal Branding** (CRITICAL):
   - Read `01_Projects/Felix_Personal_Branding_Overseas.md`
   - Understand Felix's core identity, contrarian beliefs, target audience
   - Note forbidden phrases and voice guidelines
   - **Why**: Ensures tweets align with overall brand positioning

2. **Search Past Tweet Samples** (if relevant):
   - Extract core topic keywords from user request
   - Use `grep` to search `00_Inbox/X_Samples/X.md` for these keywords
   - Command: `grep -iC 5 "keyword" 00_Inbox/X_Samples/X.md`
   - Read specific sections found (not entire file)
   - **Goal**: Ground tweets in Felix's past best-performing content on that topic

---

### Step 1: Topic Intake & Intelligence Gathering

When user requests to write a tweet:

1. **Accept input in any language**: User may provide topic and thoughts in Chinese or English
2. **Conduct brief interview** to extract key elements:
   - **Question 1**: What's the core claim? (Be specific - not "AI is important" but "AI made solo founders viable")
   - **Question 2**: What's the proof? (Specific number, personal experience, or case study)
   - **Question 3**: What should readers DO? (Concrete action, not abstract advice)

**Rules:**
- Don't start writing immediately
- Extract specifics through questions
- If user input is in Chinese, translate context but keep the essence
- Focus on finding: **bold claim + specific proof + actionable CTA**

### Step 2: Formula Selection

After gathering intel:

1. **Read** `01_Projects/X_skill/02_核心配方生成/X爆款结构.md` (if not already loaded)
2. **Analyze topic type** and select best formula:
   - Technology shift → Generational Shift formula
   - Challenging consensus → Counterintuitive Truth formula
   - Data/observation → Data Bomb formula
   - How-to advice → Step-by-Step Playbook formula
   - Mindset/values → Identity Filter formula
3. **Tell user** which formula you're using and why

### Step 3: Generate 3 Versions

Create 3 different tweet versions, each optimized for different contexts:

**Version A: Maximum Impact (The Zinger)**
- Character count: 50-150
- Purpose: Screenshot-ready, quote-worthy
- Format: Single punchy statement
- Best for: Standalone tweet, high shareability

**Version B: Balanced Thread Opener (The Hook + Context)**
- Character count: 180-250
- Purpose: Thread starter with depth
- Format: Hook + supporting details + CTA
- Best for: Starting a thread, driving engagement

**Version C: The Playbook (The Framework)**
- Character count: 200-280
- Purpose: Educational, save-worthy
- Format: Problem + numbered steps + logic
- Best for: Positioning as expert, building authority

### Step 4: Quality Check

Before outputting, verify each version passes:
- ✅ Stance Check: Clear POV?
- ✅ Proof Check: Specific number/name/example?
- ✅ Action Check: Tells reader what to DO?
- ✅ Confidence Check: No hedge words ("I think", "maybe")?
- ✅ Rhythm Check: Short, punchy sentences?
- ✅ Screenshot Check: One standalone quotable line?

### Step 5: Delivery

Present all 3 versions with:
- Clear labels (A/B/C)
- Character count for each
- Usage recommendation
- Optional: Suggest which formula was used

---

## Example Workflow

**User**: "我想写一条关于 Claude Code 让solo founder 可以做更多的推文"

**Assistant (Step 1 - Interview)**:
Got it - you want to tweet about Claude Code empowering solo founders.

Quick questions to sharpen this:
1. What's the specific change? (e.g., "1 person can now do what took 10 people before")
2. Do you have proof? (personal experience, data, or example?)
3. What should readers do? (try Claude Code? ship an app? rethink their team size?)

**User**: "对，以前要10个人的团队，现在1个人+Claude Code就够了。我自己就是证明。读者应该停止找co-founder，直接开始build"

**Assistant (Step 2 - Formula Selection)**:
Perfect. I'm using **Formula 1: Generational Shift** (Before/After structure with forcing function).

This fits because you're describing a fundamental change in what's possible for solo builders.

**Assistant (Step 3 - Generate 3 Versions)**:

**Version A: Maximum Impact (98 chars)**
```
2020: need 10 people to build an app
2026: 1 person + Claude Code

The math changed. The game changed.
```
*Use for: Standalone tweet, max virality*

---

**Version B: Balanced Thread Opener (234 chars)**
```
Everyone says "find a co-founder first."

Wrong.

2020 you needed a team. 2026 you need Claude Code.

I'm shipping apps solo that would've taken 10 people in 2020.

Stop looking for a co-founder. Start building. Hire when you hit revenue.
```
*Use for: Thread starter, persuasive argument*

---

**Version C: The Playbook (267 chars)**
```
Solo founders ask: "Should I find a co-founder or stay solo?"

My playbook:
1. Stay solo for 90 days
2. Ship 3 MVPs using Claude Code
3. If one hits → hire. If not → you saved 50% equity

Most co-founder problems = "I'm afraid to build alone."
AI fixed that.
```
*Use for: Authority building, actionable advice*

---

Which version fits your goal? Or want me to adjust?

---

## Output Format Rules

**Always structure output as:**

```
**Version A: [Type] ([char count] chars)**
[Tweet content]
*Use for: [context]*

---

**Version B: [Type] ([char count] chars)**
[Tweet content]
*Use for: [context]*

---

**Version C: [Type] ([char count] chars)**
[Tweet content]
*Use for: [context]*
```

**Save to:** `00_Inbox/writing draft/[date]-X-[topic].md`
- Naming format: `YYYY-MM-DD-X-[short-topic].md`
- Example: `2026-01-13-X-solo-founder-claude.md`

---

## Critical Rules

1. **Speed over perfection**: Generate fast, let user iterate
2. **No hedge words**: Kill "I think", "maybe", "possibly" - always
3. **Specific over abstract**: "Claude Code" not "AI tools"
4. **Action over observation**: Every tweet needs a "so do THIS"
5. **Felix voice**: Direct, urgent, builder-focused, "I've been there" authority

**Golden rule: Ship 3 versions in 5 minutes > 1 perfect tweet in 30 minutes**
