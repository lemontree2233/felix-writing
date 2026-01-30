# X Writing Samples - Index & Loading Strategy

⚠️ **CRITICAL: DO NOT read X.md automatically. It's 412KB and will blow up context.**

---

## 📋 Sample Loading Strategy

### Default Behavior (90% of cases)
**DO NOT load any samples.**

Just use the formulas and templates from `X爆款结构.md`. That file already contains:
- 5 formula templates
- Real tweet examples in each formula section
- Quality checklist
- Voice elements

**This is sufficient for most tweet generation tasks.**

---

## 🎯 When to Load Samples (10% of cases)

Only load samples if:

1. **User explicitly requests**: "Show me examples of my past tweets about X"
2. **User asks for specific style**: "Write like that tweet I did about solo founders"
3. **You need clarification**: After generating, if user says "not like this, more like my usual style"

---

## 📁 Sample Categories (Reference Only - Don't Load)

The full `X.md` file contains ~74 tweets organized by these themes:

| Theme | Tweet Count | Topics |
|-------|-------------|--------|
| **AI Tools as Leverage** | ~20 | Claude Code, vibe coding, AI agents |
| **Solo Founder Path** | ~15 | 1-person businesses, anti-co-founder, freedom |
| **Speed to Market** | ~12 | Ship fast, weekend builds, MVP mindset |
| **Breaking Systems** | ~10 | Skip college, avoid VC, challenge norms |
| **Distribution = Product** | ~8 | Content creation, organic growth, build in public |
| **Industry Observations** | ~9 | SF trends, funding, AI company metrics |

---

## 🔄 How to Use Samples (If Needed)

**Step 1: Ask user for specifics**
```
"Which past tweet style do you want to reference? Can you describe it or give me a topic?"
```

**Step 2: Use Grep to find relevant tweets**
Instead of reading all of X.md, search for specific keywords:

```bash
# Example: Find tweets about "Claude Code"
grep -i "claude code" 00_Inbox/X_Samples/X.md
```

**Step 3: Read only the relevant section**
If you find a match, read X.md with offset/limit to get ONLY that section:
- Use Read tool with offset and limit parameters
- Never read the entire file

---

## 🎓 Formula → Sample Mapping

If user asks for examples of a specific formula:

| Formula Type | Keyword Search | Sample Topics |
|--------------|---------------|---------------|
| **Generational Shift** | "2020", "2026", "used to" | Hiring changes, tool evolution, cost shifts |
| **Counterintuitive Truth** | "wrong", "everyone thinks" | Co-founder myth, VC path, general-purpose AI |
| **Data Bomb** | "saw", "stat", "%" | App metrics, churn rates, pricing patterns |
| **Playbook** | "my playbook", "answer:" | Co-founder decision, validation process, building solo |
| **Identity Filter** | "some people", "other people" | AI threat vs lever, building vs waiting |

---

## ⚡ Quick Reference Tweets (Pre-extracted)

These are SHORT examples you CAN include in responses without loading X.md:

### Generational Shift
```
2020: hire 10 interns to test ideas
2026: 1 person + Claude Code ships 7 apps/year

Not because interns got worse.
Because AI made the cost of trying ideas go from $100k → $100.
```

### Counterintuitive Truth
```
Most founders think "general-purpose AI agent" is the future.

Wrong.

Real B2B = 90% workflow (deterministic steps), not open-ended chat.
Customers don't want "does everything poorly."
They want "does THIS thing 10x faster."
```

### Data Bomb
```
Just saw: 90% of new apps use AI but charge same $9.99/month as 2019.

Translation: you're competing on legacy pricing with 100x better product.

Charge more. If your app saves 10 hours/week, it's worth $99/month not $9.99.
```

### Playbook
```
Solo founders ask: "Should I find a co-founder or stay solo?"

My playbook:
1. Stay solo for 90 days
2. Ship 3 MVPs using Claude Code
3. If one hits → hire. If not → you saved 50% equity

Most co-founder problems = "I'm afraid to build alone."
AI fixed that.
```

### Identity Filter
```
Some people are debating "will AI take my job?"

Other people are using AI to do 10 people's jobs and earning 10x.

The gap isn't technical skill.
It's whether you see AI as a threat or a lever.

2026 feels like a generational lock-in moment. Choose now.
```

---

## 🚨 Critical Rules

### ✅ DO:
- Use the templates in `X爆款结构.md` (already loaded)
- Use the 5 pre-extracted examples above (lightweight)
- Search X.md with grep if user asks for specific topic
- Read X.md with offset/limit if you find a specific tweet to reference

### ❌ NEVER:
- Read the entire X.md file (412KB)
- Load X.md "just in case"
- Read X.md without user requesting a specific past example
- Use Read tool on X.md without offset/limit parameters

---

## 📊 Token Economics

| Approach | Token Cost | When to Use |
|----------|-----------|-------------|
| Use X爆款结构.md only | ~2,000 tokens | 90% of cases (default) |
| Use pre-extracted examples | ~500 tokens | Need quick reference |
| Grep search X.md | ~100 tokens | Find specific topic |
| Read X.md section (offset/limit) | ~500-1,000 tokens | User wants specific past tweet |
| Read entire X.md | ~30,000 tokens | ❌ NEVER DO THIS |

---

## 🎯 Revised Workflow

**Phase 0: Check if samples needed**
```
IF user says "write a tweet about X":
  → Skip samples, use X爆款结构.md formulas

IF user says "write like that tweet I did about Y":
  → Grep X.md for keyword "Y"
  → If found, read that section only

IF user says "show me my past tweets about Z":
  → Grep X.md for keyword "Z"
  → Return matches without reading full file
```

---

## 📝 Update Log

- 2026-01-13: Created index with "lazy loading" strategy
- 2026-01-13: Added pre-extracted examples for each formula
- 2026-01-13: Defined grep-first, read-section approach

---

**The Golden Rule:**

X爆款结构.md has everything you need.

Only touch X.md if user explicitly asks for past examples.

**Treat X.md like a database, not a context file.**
