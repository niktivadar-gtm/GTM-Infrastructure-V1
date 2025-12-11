# First Principles Thinking

## What is it?

First principles thinking is the practice of breaking down a complex problem into its most basic, fundamental elements and then reassembling them from the ground up. Instead of relying on assumptions, analogies, or "how it's always been done," you strip everything away until you reach fundamental truths, then build your solution from there.

**Core Principle:** "Don't reason by analogy. Reason from first principles."

In GTM, we're surrounded by inherited assumptions: "SaaS needs a 30-day free trial," "Enterprise sales takes 6 months," "You have to be on LinkedIn," "Pricing should be per-user." First principles thinking allows you to question everything and rebuild GTM systems from fundamental truths about human behavior, economics, and value creation. This is how you build breakthrough strategies while competitors copy each other into mediocrity.

---

## GTM Use Cases

### Use Case 1: Deconstructing the Sales Funnel

A SaaS company has the "standard" funnel: Awareness → Lead → MQL → SQL → Opportunity → Closed Won. The sales cycle is 90 days, MQL→SQL conversion is 10%, and the team is trying to "optimize" each stage with more touchpoints, better lead scoring, and nurture campaigns.

**The Problem:** They're optimizing a fundamentally flawed system. Marginal improvements on a broken process.

**First Principles Approach:**

**Step 1: Identify the Assumptions**
- Assumption: Leads need to be "nurtured" over time
- Assumption: Everyone goes through all stages
- Assumption: More email touches = more conversions
- Assumption: 90-day sales cycles are "normal for enterprise"

**Step 2: Break Down to Fundamental Truths**
- Truth: A customer buys when (Pain > Price + Switching Cost)
- Truth: Trust comes from value demonstration, not email frequency
- Truth: Decision-makers want to buy, not be sold to
- Truth: Time kills deals (the longer it takes, the lower close rates)

**Step 3: Reason Up from First Principles**
- What if we only targeted prospects with acute pain *right now*?
- What if we demonstrated value *before* asking for a meeting?
- What if qualified buyers could skip stages entirely?
- What if we designed for a 7-day sales cycle instead of 90?

**The Rebuilt Solution: "Pain-First Prospecting"**
- Only target companies showing acute pain signals (hiring SDRs, job postings, tech stack changes)
- First touch includes free value delivery (audit, competitive analysis) not a pitch
- Qualified buyers go straight from first meeting → demo → contract
- Sales cycle: 7-14 days for high-pain prospects

**The Outcome:** 30% close rate (vs 2% before), 10x faster sales cycle.

**The Insight:** The "funnel" is a framework, not a law of nature. When you rebuild from customer psychology instead of inherited process, you create breakthrough efficiency.

---

### Use Case 2: Building a System - Goal First, Tool Last

A GTM engineer is asked to "build a lead enrichment system." Their first instinct is to open Clay or Apollo and start building workflows based on what those tools can do.

**The Problem:** Starting with the tool means the tool defines your system. You're constrained by the tool's capabilities before you've even defined what you need.

**First Principles Approach:**

**Identify Assumptions:**
- We need to use Clay/Apollo/ZoomInfo
- The tool determines what data we can enrich
- "Lead enrichment" means getting company + contact data
- More data = better

**Fundamental Truths:**
- The goal is to identify *which* leads are worth pursuing
- Data only matters if it informs decisions
- Systems should achieve outcomes, not just collect data
- Tools should serve the system design, not define it

**Reason from First Principles:**
- What is the actual goal? (Not "enrich leads" → "Identify which leads match our ICP and have buying intent")
- What data points would actually tell us that?
- What's the minimum data needed to make this decision?
- What's the simplest system that achieves this goal?

**The Rebuilt Solution: Goal → System → Tool**

1. **Define the Goal:** Identify leads that are: Series B+ tech companies, using Salesforce, recently hired an SDR (buying intent signal)

2. **Design the System:**
   - Input: List of company domains
   - Required data: Funding stage, tech stack, recent hires
   - Decision logic: IF (funding > Series B) AND (uses Salesforce) AND (hired SDR in last 60 days) → High Priority
   - Output: Scored leads in CRM

3. **Choose Tools Based on System Needs:**
   - Funding data: Crunchbase API
   - Tech stack: BuiltWith
   - Hiring signals: LinkedIn scraper or People Data Labs
   - Orchestration: n8n (not Clay, because we need custom logic)

**The Outcome:** A purpose-built system that does exactly what's needed, nothing more. Total cost: $200/month instead of $800/month for Clay.

**The Insight:** First principles for GTM engineers means: Goal → System Design → Tool Selection. Never start with the tool.

---

### Use Case 3: Pricing Strategy - Value, Not Competitors

A B2B SaaS company is setting pricing. They look at competitors: Company A = $99/user/month, Company B = $149/user/month. Their thinking: "We should price at $129 to be competitive."

**The Problem:** Copycat pricing without strategic thought. Following competitors into commoditization.

**First Principles Approach:**

**Identify Assumptions:**
- We should price based on competitors
- Per-user pricing is the right model
- Cheaper = more customers
- Monthly and annual plans are required

**Fundamental Truths:**
- Price should reflect value delivered, not competitor pricing
- Different customers get different amounts of value
- Pricing model influences customer behavior and your revenue
- Revenue = Price × Volume; optimize both, not just volume

**Reason from First Principles:**
- What value does our product actually create? (Quantify it)
- Who gets the most value? (Segment by value, not demographic)
- What metric best aligns our revenue with customer value?
- How can we charge for outcomes, not inputs?

**The Rebuilt Solution:**
Analysis shows the product saves customers 20 hours/week (value = $2,000/week at $100/hour).

New pricing:
- Charge 10% of value delivered = $800/month per team (not per user)
- High-value segment (agencies managing multiple clients): $2,500/month
- Low-value segment (solopreneurs): $99/month
- No per-user pricing — charge for value, not seats

**The Outcome:** Average ACV 3x higher than competitor-based pricing would have been. Higher perceived value (customers see ROI clearly).

**The Insight:** Pricing derived from customer value > pricing derived from competitor positioning. First principles says: understand the value you create, then capture a fair percentage of it.

---

### Use Case 4: Lead Scoring System - Logic First, Not Formula

A GTM engineer is asked to "build a lead scoring system." They look at HubSpot's default lead scoring template: +10 points for email open, +20 for page visit, +50 for demo request. They start configuring those rules.

**The Problem:** Using someone else's scoring logic without questioning if it makes sense for your business.

**First Principles Approach:**

**Identify Assumptions:**
- Lead scoring should use engagement metrics (opens, clicks, visits)
- More engagement = higher score = better lead
- We need a 0-100 point scale
- The HubSpot/Salesforce template is a good starting point

**Fundamental Truths:**
- A "good lead" is one that's likely to buy and be a good customer
- Engagement ≠ buying intent (people browse without buying all the time)
- The best predictor of future behavior is past behavior (look at closed deals)
- Scores exist to prioritize sales effort, not to look sophisticated

**Reason from First Principles:**
- What actually predicts if someone will buy? (Analyze your closed deals)
- What do our best customers have in common *before* they bought?
- What's the simplest scoring system that achieves the goal (prioritize sales effort)?
- Do we even need a 0-100 scale, or just High/Medium/Low?

**The Rebuilt Solution: Analyze First, Score Second**

1. **Analyze closed deals:** Discover that 90% of closed deals had:
   - Company size: 50-500 employees
   - Used Salesforce
   - Visited pricing page 2+ times
   - Came from cold outreach or referral (not ads)

2. **Design scoring from truths:**
   - High Priority: Meets all 4 criteria
   - Medium: Meets 2-3 criteria
   - Low: Meets 0-1 criteria
   - Ignore engagement metrics (opens, clicks) entirely

3. **Implement the simple system:**
   - Use enrichment to get company size + tech stack
   - Track pricing page visits (behavioral signal)
   - Tag source
   - Auto-score in CRM

**The Outcome:** Sales focuses on High Priority leads. Close rate goes from 12% → 28% because they're working actual good-fit prospects.

**The Insight:** First principles for lead scoring means: analyze what actually predicts success, then build the simplest system that captures it. Don't use someone else's formula.

---

### Use Case 5: Automation Design - Eliminate Before You Automate

A sales team wants to "automate their workflow." They start comparing Zapier, Make, and n8n. The question is: "Which automation tool should we use?"

**The Problem:** They're jumping to tool selection before understanding what should actually be automated.

**First Principles Approach:**

**Identify Assumptions:**
- We need an automation tool
- More automation = better
- The tool determines what we can automate
- Automation = efficiency

**Fundamental Truths:**
- Automation is: moving data from System A → System B based on a trigger
- Only repetitive, rules-based tasks should be automated
- Automating a bad process = bad process at scale
- The best automation is the one the user never sees

**Reason from First Principles:**
- What tasks are actually repetitive? (Not "could be" automated)
- What workflows have clear, unambiguous rules?
- Should we automate this, or eliminate it entirely?
- What's the simplest way to connect these systems?

**The Rebuilt Solution: "Process First, Automate Second"**
1. Map the current manual process completely
2. Eliminate unnecessary steps (essentialism)
3. Simplify what remains
4. THEN automate what's left
5. Choose tool based on simplicity, not features

Result: 50% of "automation ideas" get eliminated entirely. The remaining automation is simple, robust, and maintainable.

**The Outcome:** Fewer automations, but the ones that exist actually work and save time.

**The Insight:** First principles asks: "Should this step exist at all?" before asking "How do we automate it?" Many workflows are automated solutions to problems that shouldn't exist.

---

## Correct vs False Thinking

### ❌ False Ways of Thinking (Missing First Principles)

- **"Let's do what [successful company] does."** → This is reasoning by analogy, not first principles. What works for them might not work for you. Context matters.

- **"Industry best practice is X, so we should do X."** → "Best practice" often means "what everyone copies from everyone else." First principles questions whether the practice is actually best.

- **"We need to use [tool] because everyone in our industry uses it."** → Cargo-culting. First principles asks: what problem are we solving, and is this the simplest solution?

- **"That's just how SaaS/sales/marketing works."** → This is inherited wisdom, not truth. First principles challenges assumptions about "how things work."

- **"We should price like our competitors."** → You're letting competitors determine your revenue. First principles derives pricing from value, not competition.

- **"If it ain't broke, don't fix it."** → Just because something "works" doesn't mean it's optimal. First principles asks: if we rebuilt this today, would we do it the same way?

- **"We tried that before and it didn't work."** → Past context ≠ current context. First principles evaluates decisions based on current truths, not past failures.

### ✅ Correct Ways of Thinking (Applying First Principles)

- **"Everyone does X, but what if we questioned that assumption? What's actually true here?"** → This is first principles in action. Identifying assumptions, stripping to truth.

- **"If we had to build this from scratch today, would we build it this way?"** → The ultimate first principles question for existing systems.

- **"What problem are we actually solving, stripped of all methodology?"** → This gets to the fundamental goal, separate from how others approach it.

- **"Let's map out what we assume to be true, then test each assumption."** → Systematic first principles thinking. Explicit assumptions → explicit testing.

- **"Competitors charge per-user, but our value isn't user-based. What metric actually aligns with the value we create?"** → First principles pricing. Derive from value, not convention.

- **"The 'standard funnel' isn't working. What are the fundamental truths about how our customers actually buy?"** → Rebuilding from customer behavior, not inherited frameworks.

- **"Before we automate this, should this step exist at all?"** → First principles for process design. Question existence before optimizing efficiency.

- **"What would this look like if we ignored all constraints except laws of physics, economics, and human psychology?"** → True first principles. Most "constraints" are self-imposed.

---

## Quick Reference

**The First Principles 3-Step Process:**
1. **Identify assumptions** - What am I assuming to be true?
2. **Break down to truths** - What is objectively, fundamentally true?
3. **Reason upward** - Build the solution from those truths

**The Ultimate Test:** "If I had to rebuild this from scratch today with everything I now know, would I build it the same way?"

If the answer is no, you've found an opportunity for first principles redesign.

**When to Use First Principles:**
- ✅ High-stakes decisions (pricing, positioning, channel strategy)
- ✅ Systems that aren't working despite "best practices"
- ✅ When you want 10x improvement, not 10%
- ❌ Low-stakes decisions (button colors, minor copy tweaks)

**Warning:** First principles thinking is mentally demanding. Use it for decisions that matter. Don't waste cognitive energy on trivial choices.