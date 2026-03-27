---
name: research-to-convert
description: >
  Builds conversion-optimized landing pages, marketing sites, and
  waitlist pages through deep market research — not generic AI templates.
  Researches competitors, applies Eugene Schwartz awareness levels and
  Alex Hormozi value equation, analyzes competitor fonts/colors/design,
  then builds and self-critiques the result. Use when building a landing
  page, marketing page, product page, waitlist, launch page, or when
  the user says "build me a page that converts", "I need a landing page",
  "create a waitlist", "help me with marketing copy", or "I have an idea
  and need a page for it". Also use when the user wants to improve an
  existing landing page or optimize copy for conversion.
---

# Research-to-Convert

Research-driven process for building marketing pages that actually convert.
The difference: every other AI tool goes prompt → page. This skill goes
prompt → research → frameworks → design analysis → build → self-critique → page.

**Rule: Never build before completing Steps 1-5. The research IS the skill.**

## Before Starting — Get Context From the User

Ask these in a single message. Only ask what the user knows that you can't research:

1. Describe your product/idea in 2-3 sentences — what does it do and why does it matter?
2. Who specifically is this for? (e.g. "food reviewers who write Google Maps reviews for free")
3. What's the goal of this page? (waitlist signups, sales, app downloads, etc.)
4. Any existing brand decisions? (name, colors, fonts — or should we figure this out?)
5. Anything you've already tried or any competitors you're aware of?

Do NOT ask about competitors, market size, design direction, copy approach, or
technical stack — research those yourself in the following steps.
Once you have answers, proceed to Step 1 immediately without further questions.

## Step 1: Market & Competitor Research

Before writing any copy or code, run deep research.

**Search patterns (adapt keywords to the user's product/market):**

| What you need | Search query pattern |
|---|---|
| Competitor landscape | `[product category] app startup 2025 2026` |
| Revenue/traction data | `[competitor name] revenue funding users` |
| Visual identity | `[competitor] brand colors hex font typography` |
| Market validation | `[product category] startups funded YC 2025` |
| Legal constraints | `[platform] API terms of service commercial use` |
| User pain points | `[competitor] app store reviews complaints` |
| Category design norms | `[competitor] website landing page design` |

**Document before proceeding:**
- Top 3-5 direct competitors: what they look like, how they position, real numbers
- What's been tried before and why it failed or succeeded
- Legal or technical constraints that could kill the idea
- The gap nobody is filling — this becomes the core positioning

## Step 2: Pressure-Test Assumptions

List every assumption in the user's idea. For each:
- Find evidence that supports or contradicts it
- If a core assumption is dead, say so immediately and suggest pivots
- Be honest — the user hired you for truth, not comfort

Rate the idea 1-10 with specific reasoning. Share this with the user.

## Step 3: Identify Audience Awareness Stage

Reference: [references/SCHWARTZ.md](references/SCHWARTZ.md) — read this file now.

For EACH audience segment, determine their Schwartz awareness stage:

| Stage | They already know... | Your headline must... |
|---|---|---|
| **Unaware** | Nothing about the problem | Lead with curiosity or desire |
| **Problem-Aware** | They have a pain | Name and agitate the pain, reveal solution |
| **Solution-Aware** | Solutions exist, not yours | Differentiate your new mechanism |
| **Product-Aware** | Your product, not convinced | Prove with testimonials and results |
| **Most Aware** | Everything, ready to act | Price, offer, urgency — close the deal |

Write the hero headline ONLY after identifying the stage. The stage determines
everything: headline approach, copy length, proof requirements, and CTA style.

## Step 4: Structure the Offer

Reference: [references/HORMOZI.md](references/HORMOZI.md) — read this file now.

Apply to every section of the page:

```
Value = (Dream Outcome × Perceived Likelihood) / (Time Delay × Effort)
```

**Maximize the top:**
- Dream Outcome → specific numbers, not vague promises ("$247.80/month" not "earn money")
- Perceived Likelihood → comparison tables, testimonials with real stats, proof of mechanism

**Minimize the bottom:**
- Time Delay → "earn from day one", "results this week", "paid monthly"
- Effort → "same thing you already do", "no behavior change", "3 steps"

## Step 5: Research Competitor Visual Design

**This step is critical. Never skip it. Never guess.**

The page must look like it belongs in the product's CATEGORY, not in the builder's personal aesthetic preferences.

**Process:**
1. Search for 4-5 competitor websites and adjacent products
2. Research their actual fonts: search `"[competitor] font typeface what font"`
3. Research their actual colors: search `"[competitor] brand color hex code"`
4. Identify the visual PATTERN across all competitors
5. Design within that pattern with a distinctive accent

**Category patterns (starting point — always verify with research):**

| Category | Background | Accent colors | Font style |
|---|---|---|---|
| Food / lifestyle | White, warm cream | Coral, warm red, orange | Rounded sans-serif |
| SaaS / B2B | White, light gray | Blue, indigo | Clean geometric sans-serif |
| Finance / fintech | Dark navy, white | Green, gold | Professional, clean |
| Creative tools | Dark or bold | Vibrant, multi-color | Experimental display fonts |
| Health / wellness | Soft white, pastels | Teal, green, sage | Rounded, friendly |
| E-commerce | White, minimal | Brand-specific | Clean, readable |

**Never use:** Inter, Roboto, Arial, or default system fonts. These create zero
brand recognition and signal "this was built by AI without thinking."

**Good distinctive pairings (examples, always research category first):**
- Plus Jakarta Sans + Bricolage Grotesque (warm, modern — food/lifestyle)
- Cabinet Grotesk + Satoshi (clean, distinctive — SaaS)
- General Sans + Clash Display (bold, contemporary — creative)
- Nunito + Poppins (friendly, accessible — wellness/education)

## Step 6: Build the Page

**Conversion-optimized section order:**

1. **Hero** — Problem/desire headline + social proof badge + email CTA (above fold)
2. **Comparison** — Side-by-side crystallizing the value gap (old way vs. new way)
3. **Differentiators** — 3-4 cards explaining why the mechanism works (builds trust)
4. **How it works** — 3 steps with SPECIFIC titles ("$47 hits your account" not "Get paid")
5. **Testimonial** — One person with name, photo, real stats, real city
6. **Stats bar** — Hard numbers sourced from Step 1 research
7. **Final CTA** — Specific offer with genuine urgency + legal disclaimer
8. **Secondary audience** — B2B or alternate audience sections (below main CTA)
9. **Footer** — Three-column nav with platform, business, and legal links

**Copy principles:**
- Specificity > abstraction: "$47 hits your account" beats "Get paid monthly"
- Visual proof > description: show a mock earnings dashboard, don't describe the feature
- Cut ruthlessly: if a section doesn't build trust or drive toward CTA, kill it
- Negative proof builds trust: showing honest/negative outcomes being rewarded
- Movement language: "Join 2,847 people who..." not "Sign up for our beta"
- One accent color for ALL CTAs and interactive elements — consistency signals quality

**Waitlist/signup flow:**
- Email-only first capture (lowest friction possible)
- Post-signup modal for segmentation (role, city, referral source)
- Frame extra questions as "skip the line" incentive, not a gate
- Include referral/affiliate hook in post-signup when applicable

**Technical output:**
- React (JSX) or HTML — deployable to Vercel/Netlify immediately
- Mobile-responsive — non-negotiable
- Google Fonts loaded via import — never rely on system fonts
- All colors defined as constants at the top of the file for easy theming

## Step 7: Self-Critique in Character

After building, review the ENTIRE page as the target user.

**Process:**
1. Define persona: age, current tools they use, how they'd discover this page
2. Scroll top to bottom, narrating internal reactions at each section
3. Check these specific conversion killers:

| Check | Fix if failing |
|---|---|
| Value prop clear in 5 seconds? | Simplify hero headline |
| Comparison crystallizes the gap? | Add side-by-side table |
| Social proof from a real-seeming person? | Add testimonial with stats |
| How-it-works steps are specific? | Replace generic titles with concrete outcomes |
| CTA offer is specific (exact amount/benefit)? | State the exact number or benefit |
| Anything feels like pitch deck instead of product? | Rewrite for the user, not investors |
| What's missing that would make YOU sign up? | Add it |

4. Implement ALL improvements
5. Present the final version with a summary of what changed and why

## Anti-Patterns

These kill conversion. Avoid them:

- **Building before researching** — the #1 mistake, produces generic output
- **Dark mode for consumer/lifestyle products** — category mismatch signals "not for me"
- **Generic copy** — "Review honestly" instead of "Write what you actually think"
- **Invisible fonts** — Inter/Roboto/Arial create zero brand recognition
- **Skipping competitor design research** — your page should feel like it belongs in the category
- **Multi-audience sections before primary CTA** — don't slow momentum for secondary audiences
- **Vague offers** — "guaranteed minimum" instead of "$5 per review, guaranteed"
- **Fake urgency** — countdown timers that reset destroy trust instantly
- **Skipping self-critique** — the step that caught 8 improvements in the original build
