# Chromara Content Skill Graph

Central knowledge base for Chromara's AI content production system. Designed to be queried by Claude Managed Agents for consistent, brand-aligned content generation across all platforms.

## What This Is

A structured knowledge graph that enables AI agents to:
- Maintain brand voice consistency across 7 platforms
- Adapt tone appropriately per platform while keeping core voice intact
- Use proven hook formulas and content structures
- Avoid known failure patterns
- Learn from performance data over time

## Structure

```
/content-skill-graph/
├── INDEX.md                    # Central hub, quick reference
├── platform/
│   ├── tiktok.md               # TikTok-specific rules
│   ├── instagram.md            # Instagram-specific rules
│   ├── facebook.md             # Facebook-specific rules
│   ├── newsletter.md           # Email newsletter rules (Brevo)
│   ├── youtube.md              # YouTube-specific rules
│   ├── x.md                    # X/Twitter-specific rules
│   └── pinterest.md            # Pinterest-specific rules
├── voice/
│   ├── brand-voice.md          # Core voice, constraints, banned patterns
│   └── platform-tone.md        # How voice adapts per platform
├── engine/
│   ├── hooks.md                # Hook formulas by type
│   ├── repurpose.md            # Content chain (1 idea → 7 platforms)
│   ├── content-types.md        # Format specifications
│   └── scheduling.md           # Posting frequency and timing
├── audience/
│   ├── consumers.md            # Consumer audience segments
│   └── b2b.md                  # B2B audience segments
└── evolution/
    ├── changelog.md            # All updates to the system
    ├── winners.md              # Patterns that work
    └── losers.md               # Patterns to avoid
```

## How Agents Use This

1. **Script Writer Agent** reads `brand-voice.md` → `platform-tone.md` → relevant platform file → `hooks.md` → `content-types.md`
2. **QA Reviewer Agent** checks output against `brand-voice.md` constraints and `losers.md` patterns
3. **Performance Analyst Agent** updates `winners.md` and `losers.md` based on PostHog data
4. **Trend Scout Agent** may update platform files or `hooks.md` based on emerging patterns

## Key Constraints

These rules are enforced across ALL content:

- No em dashes (anywhere, ever)
- No antithetical parallelism ("this isn't X, it's Y")
- No rhetorical fragments for effect
- Stats ceiling: 67%, 40%, $2B+, 4.5M, 120B
- Consumer content uses "NovaMirror" only (never "ChromaCore")
- See `brand-voice.md` for full constraint list

## Brand Quick Reference

| Element | Value |
|---------|-------|
| Company | Chromara |
| Founders | Faith Binkholder (COO), Lydia Steevens (CTO) |
| Product | NovaMirror (consumer) / ChromaCore (B2B only) |
| Category | Beauty tech infrastructure |
| Core stat | 4.5 million shades from 9 refillable pods |

## Evolution

This is a living system. As content performs (or doesn't), the skill graph updates:

- `winners.md` grows with proven patterns
- `losers.md` grows with failed patterns
- `changelog.md` tracks all modifications
- Platform files get refined based on learnings

## License

Internal use only. Chromara proprietary.
