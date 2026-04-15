# Chromara Content Skill Graph

Central knowledge base for all Chromara content production. Queried by content agents to maintain brand consistency across platforms.

---

## Brand Identity

**Company:** Chromara
**Founders:** Faith Binkholder (Co-Founder & COO), Lydia Steevens (Co-Founder & CTO)
**Origin:** Both former Sephora retail floor employees
**Category:** Beauty tech infrastructure (not a makeup brand)
**Product:** NovaMirror (consumer-facing name)
**Mission:** Make shade matching failure feel like a named personal injury with a solution

---

## Current Campaign

"Donate $1 to End Shade Matching Forever"
30-day crowdfunding-style awareness and conversion campaign across Brand TikTok, Personal TikTok, YouTube, and Pinterest.

---

## Core Stats (Verified, Never Exceed)

| Stat | Value | Source |
|------|-------|--------|
| Shade match failure rate | 67% | Revieve 2024 |
| Foundation return rate | 40% | Industry data |
| Annual industry waste | $2B+ | Ceiling figure |
| Shade combinations | 4.5 million | From 9 pods |
| Single-use packaging waste | 120 billion units/year | BeautyMatter/Pact Collective 2024 |

---

## Hard Rules (Apply at Execution Level)

### Never Use
- Em dashes (anywhere, ever)
- Antithetical parallelism ("this isn't X, it's Y" / "not X, but Y")
- Rhetorical fragments for effect
- Oxidation/pH references
- Charity or civic framing
- Investor/VC language in consumer content

### Banned Words
revolutionizing, redefining, seamless, celestial, shade equity, pumps, dispensing mechanism, stepper motor, microdosing, patented, portal, align/alignment, collective, breach

### Naming
- Consumer content: "NovaMirror" only
- Never use "ChromaCore" in consumer-facing materials
- Never disclose proprietary mechanism details (describe outputs only)

---

## File Structure

```
/content-skill-graph/
├── INDEX.md                    ← You are here
├── platform/
│   ├── tiktok.md
│   ├── instagram.md
│   ├── facebook.md
│   ├── newsletter.md
│   ├── youtube.md
│   ├── x.md
│   └── pinterest.md
├── voice/
│   ├── brand-voice.md
│   └── platform-tone.md
├── engine/
│   ├── hooks.md
│   ├── repurpose.md
│   ├── content-types.md
│   └── scheduling.md
├── audience/
│   ├── consumers.md
│   └── b2b.md
└── evolution/
    ├── changelog.md
    ├── winners.md
    └── losers.md
```

---

## Agent Access Pattern

When an agent needs to create content:

1. Read [[brand-voice]] for core constraints
2. Read [[platform-tone]] for platform-specific adaptation
3. Read relevant platform file (e.g., [[tiktok]])
4. Read [[hooks]] for opening formulas
5. Read [[content-types]] for format specs
6. Check [[winners]] for what's working
7. Check [[losers]] for what to avoid
8. Log updates to [[changelog]] when patterns change

---

## Learning Protocol

Performance Analyst agent reviews content at 48-72 hours post-publish:
- Update [[winners]] with high-performing patterns
- Update [[losers]] with underperforming patterns
- Update [[hooks]] based on what's working per platform
- Update platform files if platform-specific learnings emerge
- Log all changes to [[changelog]]

---

## Links

- [[brand-voice]] — Core voice rules and constraints
- [[platform-tone]] — How voice adapts per platform
- [[hooks]] — Hook formulas by type
- [[repurpose]] — Content chain from one idea to seven platforms
- [[content-types]] — Format specifications
- [[scheduling]] — Posting frequency and timing
- [[consumers]] — Consumer audience segments
- [[b2b]] — B2B audience segments
- [[winners]] — Patterns that work
- [[losers]] — Patterns to avoid
- [[changelog]] — All updates to this system
