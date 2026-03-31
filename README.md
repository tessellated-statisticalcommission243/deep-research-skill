# Deep Research — Claude Skill

A Claude skill that delivers 10-15x the depth of surface-level research on any topic — markets, products, features, competitors, regulations, or opportunities.

## What This Skill Does

Most AI research outputs are shallow — they cover what's easily Googlable and present generic overviews. This skill forces Claude to go far beyond that by executing a structured 5-layer research methodology with analytical frameworks, synthesis techniques, and built-in quality gates.

**The 5 Research Layers:**

1. **Surface Scan** — The basics (table stakes, done fast)
2. **Structure & Landscape** — How the space is organized, with decision logic and tradeoffs
3. **Depth Dive** — Hidden insights, failure stories, implementation gotchas, practitioner reality (where most research stops, this skill keeps going)
4. **Adjacent Opportunities** — Things you didn't ask about but should know exist
5. **Horizon Pointers** — Brief flags for further exploration

**Includes:**

- **12 analytical frameworks** with full application instructions (PESTEL, Porter's Five Forces, JTBD, Competitive Positioning Map, SWOT, and more)
- **Synthesis engine** with triangulation, pattern recognition, confidence calibration, and a mandatory red-team protocol
- **6 topic-specific playbooks** (Market Entry, Product Research, Competitive Analysis, Regulatory, Problem-Solving, Service Expansion)
- **Good vs. bad output examples** with commentary
- **Dynamic source selection** with weighting by topic type

## Installation

### Claude Desktop / Claude.ai

1. Download the `deep-research.skill` file from [Releases](../../releases)
2. Drag and drop the `.skill` file into your Claude conversation
3. The skill is now active for that project

### Manual Installation

1. Clone this repo or download the `deep-research/` folder
2. Place the entire `deep-research/` folder in your Claude skills directory
3. The skill triggers automatically on research-intent prompts

## File Structure

```
deep-research/
├── SKILL.md                          # Core engine (mode detection, execution flow, output template)
└── references/
    ├── frameworks.md                 # 12 analytical frameworks with application guides
    ├── synthesis-engine.md           # Synthesis, red-team, confidence calibration
    ├── playbooks.md                  # 6 step-by-step research playbooks
    ├── examples.md                   # Good vs bad output comparisons
    └── source-selection.md           # Source categories, weighting, red flags
```

## Usage

The skill triggers automatically when you use research-intent language:

```
"Research the utility discount market for disability placard holders"
"Dig into how referral features work in patient portals"
"What does the competitive landscape look like for telehealth GLP-1 services?"
"Explore whether we should expand into FMLA certifications"
"Help me understand the regulatory requirements for medical window tint exemptions"
```

### Two Modes

**Guided Mode** — If your prompt is broad or ambiguous, Claude asks 3-5 targeted questions before executing.

**Autonomous Mode** — If your prompt is specific and detailed, Claude executes immediately.

You can also force a mode:
- "Ask me questions first, then research X" → Guided
- "Just go — research X" → Autonomous

## What Makes This Different

| Typical AI Research | This Skill |
|---|---|
| Generic overview | Structured 5-layer methodology |
| Surface-level facts | Hidden insights, failure cases, practitioner reality |
| No analytical framework | 12 frameworks applied based on topic type |
| Single narrative | Red-team counter-arguments built in |
| "Here are some facts" | Facts elevated to insights with "so what" |
| Stops at what was asked | Delivers 10-15x with adjacent opportunities |

## Customization

The skill is designed to be modified. Common customizations:

- **Add industry-specific playbooks** — Copy the playbook template in `references/playbooks.md` and add steps specific to your industry
- **Adjust framework selection** — Modify the framework selection table in `SKILL.md` to match your most common research scenarios
- **Add source categories** — Add industry-specific sources to `references/source-selection.md`
- **Tune depth** — Adjust quality gates in each layer to match your depth requirements

## License

MIT License — see [LICENSE](LICENSE) for details.
