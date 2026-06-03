# Day 3 — Role-Based Prompting
**ABTalks 60-Day Claude AI Mastery Challenge**

---

## What is Role-Based Prompting?

Role-Based Prompting means assigning Claude a specific expert persona *before* asking your question. Instead of a generic answer, you get a response shaped by the mental model, priorities, and vocabulary of that expert.

**Syntax:**
```
You are a [Role]. [Context about their experience].
Now answer: [Your question]
```

---

## The Experiment

**Question used across all three tests:**
> *"How should I build a product that people actually want to use?"*

---

### Response 1 — No Role Assigned (Generic)

**Prompt:**
```
How should I build a product that people actually want to use?
```

**Output:**
Focus on user needs. Build an MVP, gather feedback, and iterate. Research your target audience, solve a real problem, and keep the interface simple. Test early and often. Prioritize features based on user demand.

**Observation:** Broad, textbook advice. Covers everything, specializes in nothing.

---

### Response 2 — Founder Persona

**Prompt:**
```
You are a successful startup Founder who has built and scaled multiple products from 0 to 1.
How should I build a product that people actually want to use?
```

**Output:**
Start with pain, not features. Talk to 50 potential customers before writing a single line of code. Your job isn't to build — it's to find a problem so painful people will pay to solve it. Launch ugly and fast, then let *retention data* tell you what to build next. Most products fail not from bad engineering, but from building something nobody needed. Revenue is the only real validation.

**Observation:** Focused on customers, market validation, and business survival. Urgency-driven. Talks about *retention* and *revenue* as north-star metrics.

---

### Response 3 — Developer Persona

**Prompt:**
```
You are a senior software developer with 10+ years of experience shipping production products used by millions.
How should I build a product that people actually want to use?
```

**Output:**
Ship a working prototype in week one. Instrument everything with analytics from day zero — you can't improve what you don't measure. Keep the tech stack boring and proven so you spend cycles on product, not infra. Build feature flags so you can A/B test without redeployments. The best code is code you don't have to write yet — defer complexity until users prove they need it. Error tracking and logging from day one — you'll thank yourself later.

**Observation:** Focused on shipping speed, observability, and technical decisions that enable iteration. Talks about *feature flags*, *error tracking*, and *proven stacks* — things a founder might never mention.

---

## Comparison Table

| Dimension | No Role | Founder | Developer |
|-----------|---------|---------|-----------|
| **Focus** | General UX principles | Customer pain & revenue | Shipping speed & instrumentation |
| **First step** | Research users | Talk to 50 customers | Ship a prototype |
| **Key metric** | User satisfaction | Retention & revenue | Analytics & error rates |
| **Vocabulary** | "MVP", "feedback" | "pain", "validation", "revenue" | "feature flags", "observability", "stack" |
| **Tone** | Academic | Urgent, survival-minded | Pragmatic, technical |
| **Depth** | Surface-level | Business-strategic | Technically specific |

---

## Key Learnings

1. **Same question, completely different answers.** The role shapes not just the *tone* but the entire *mental model* and *priorities* of the response.

2. **Role prompting = unlocking expertise.** The Founder thinks about survival and customers. The Developer thinks about shipping and measuring. Both are right — but for different contexts.

3. **Use multiple personas for important decisions.** Before building anything significant, ask the Founder version, the Developer version, and even a User Research version. You'll get a 360° view you'd never get from a single prompt.

4. **The more specific the role, the better.** "You are a developer" is weak. "You are a senior developer with 10+ years shipping products used by millions" is strong — it sets context, experience level, and implied priorities.

---

## Practical Benefits of Role-Based Prompting

- **Persona-driven depth:** You get answers from the lens of someone who has *lived* the problem, not just read about it.
- **Better decisions:** Viewing one problem from multiple professional angles reveals blind spots.
- **Real-world simulation:** You can consult a Founder, PM, HR Manager, Marketer, and Developer in the same afternoon — for free.

---

## Tool of the Day — Claude Usage Counter

**What it is:** A Chrome extension that tracks your Claude message consumption, estimated limits, and real-time usage statistics.

**Setup:**
1. Open Chrome Web Store → search "Claude Usage Counter"
2. Click "Add to Chrome"
3. Pin to toolbar
4. Open claude.ai and observe stats

**Why it matters:** Helps you stay within plan limits and understand how intensively you're using Claude across sessions.

---

## LinkedIn Post

*Day 3 of #60DayClaudeChallenge — Role-Based Prompting blew my mind today.*

I asked Claude the same question three times:
- Once with no role → generic advice
- Once as a Founder → "talk to 50 customers before writing code"
- Once as a Developer → "ship in week one, instrument everything"

Same question. Completely different mental models. This is the real power of prompt engineering.

@Anthropic @ABTalksOnAI @AnilBajpai
#60DayClaudeChallenge #PromptEngineering #AITools #Claude
