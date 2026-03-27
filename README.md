# research-to-convert

A Claude Code skill that builds landing pages that actually convert — by researching your market before writing a single line of code.

## The problem with AI landing pages

Every AI page builder does the same thing: you describe your product, it generates a page. The result looks polished but converts like garbage because it skipped the only step that matters — understanding who you're talking to and what they already believe.

**Generic AI output:** "We help you do X. Sign up today!" → 2% conversion

**Research-to-convert output:** "Your reviews make platforms billions. You make $0." → built from competitive analysis of Yelp ($1.41B revenue), Beli (75M reviews), and Google Maps ($3.5B ad revenue), targeting Problem-Aware reviewers using Schwartz Stage 4 agitation with Hormozi specificity ($247.80/month, not "earn money")

The difference is the research.

## What this skill does

A 7-step process that turns Claude into a conversion copywriter who does their homework:

1. **Research** — searches competitors, finds real revenue numbers, checks legal feasibility
2. **Pressure-test** — challenges every assumption, rates the idea honestly 1-10
3. **Schwartz** — identifies audience awareness stage, matches all copy to that stage
4. **Hormozi** — structures the offer to maximize value perception
5. **Design research** — finds competitors' actual fonts, colors, patterns before designing
6. **Build** — creates a deployable page with conversion-optimized section order
7. **Self-critique** — reviews the page in character as the target user, implements fixes

Every step exists because skipping it produced a measurably worse result during real testing.

## Install

### Claude Code (recommended)
```bash
git clone https://github.com/solzange/research-to-convert.git
cp -r research-to-convert ~/.claude/skills/research-to-convert
```

### Other AI coding agents
This skill follows the [Agent Skills open standard](https://agentskills.io) and works with Claude Code, Cursor, Gemini CLI, and other compatible tools. Copy the skill directory to your agent's skill location.

## Usage

The skill auto-triggers when you ask Claude to build a landing page, marketing site, or waitlist page. Invoke directly with:

```
/research-to-convert
```

### Prompts that trigger this skill

- "I have an idea for [X]. Build me a landing page."
- "Create a waitlist page for my startup"
- "I need a page that actually converts"
- "Build me marketing for this product"
- "Help me with conversion-optimized copy"
- "Improve my existing landing page"

### What happens (and why it's different)

Claude will NOT immediately start building. It will:

1. Ask about your product and audience
2. Research your competitors (real searches, real data)
3. Tell you what's strong and what's weak about your positioning
4. Identify whether your audience is Unaware, Problem-Aware, Solution-Aware, or Product-Aware — and explain why it matters
5. Research what competing products' websites actually look like (fonts, colors, layout patterns)
6. Build the page using the right framework for your audience's awareness stage
7. Review the entire page pretending to be your target user, narrating what works and what doesn't
8. Fix everything the self-critique caught

Output: a deployable React/Next.js page with conversion-optimized copy, category-appropriate design, and proper waitlist/signup flow.

## File structure

```
research-to-convert/
├── SKILL.md                    # Core instructions (the 7-step process)
├── README.md                   # This file
└── references/
    ├── SCHWARTZ.md             # Eugene Schwartz awareness framework
    └── HORMOZI.md              # Alex Hormozi value equation framework
```

Claude loads SKILL.md when triggered. Reference files load only when Claude reaches the relevant step — keeping context usage efficient.

## The frameworks

### Eugene Schwartz (Breakthrough Advertising, 1966)
The 5 stages of customer awareness determine how you write every headline. Most landing pages target Problem-Aware or Solution-Aware audiences, but getting the stage wrong means your copy talks past the reader entirely.

### Alex Hormozi ($100M Offers)
The Value Equation structures every offer: maximize dream outcome and perceived likelihood, minimize time delay and effort. Applied to landing pages, this means specific numbers ($247.80/month), visual proof (mock dashboards), zero-friction signup (email only), and legitimate urgency (real founding member benefits).

## Origin

This skill was extracted from a real session building a startup landing page from scratch. The process involved:
- 15+ market research searches across competitor data, legal terms, revenue figures, and design systems
- Competitive analysis of Yelp, Google Maps, Beli, YouTube, Lemon8, The Infatuation, and Atmosfy
- Three design iterations (dark developer theme → light theme → category-researched warm theme)
- In-character self-critique as a 24-year-old target user that identified 8 specific improvements
- Font and color research on every major competitor before choosing the visual identity

The playbook was documented, then converted into this reusable skill.

## Live example

**[revu-app-psi.vercel.app](https://revu-app-psi.vercel.app/)** — a waitlist landing page for a review platform startup, built entirely using this skill's process in a single session.

The page went through the full 7-step cycle: competitive research (Yelp, Beli, Google Maps, YouTube), Schwartz Stage 4 copy for Problem-Aware reviewers, Hormozi value equation applied to the offer, competitor visual research that caught a wrong design direction (dark developer theme → warm food-platform theme after researching what Yelp, Beli, and Google Maps actually look like), and an in-character self-critique as a 24-year-old Google Maps power reviewer that led to adding the comparison table, removing audience tabs that slowed conversion, and specifying "$5 per review" instead of a vague "guaranteed minimum."

## Origin story

This skill started with a real conversation. Someone noticed their mum was always excited about how many views her Google Maps reviews got, and their girlfriend was frustrated that she didn't earn anything from hers despite having even more reviews.

That frustration became a startup idea: what if reviewers got paid like YouTube creators? The idea went through hours of deep market research, brutal honest feedback, financial modeling, competitive analysis, and three rounds of design iteration — all in one session. 

The landing page that came out of it was genuinely good. Not because of any single clever trick, but because every decision was driven by research: the headline came from Schwartz's awareness framework, the offer structure came from Hormozi's value equation, the design came from studying what Yelp, Beli, and YouTube actually look like, and the final optimizations came from pretending to be the target user and being honest about what wasn't working.

Afterward, the question was: "Can we make this process repeatable?" This skill is the answer.

## What this skill is NOT

- Not a generic AI page builder (those skip research and produce AI slop)
- Not a design system or component library
- Not a replacement for real user testing (this gets you to a strong v1, then you test with humans)
- Not a prompt template (it's a multi-step process with research, frameworks, and self-correction)

## Contributing

The most valuable contributions:
- Additional copywriting frameworks with practical, step-by-step application instructions
- Category-specific design pattern documentation (what do fintech landing pages look like vs. food apps vs. SaaS?)
- Before/after examples of pages built with this skill (especially the self-critique step improvements)
- Bug reports: did the skill trigger when it shouldn't have, or fail to trigger when it should?

## License

MIT
