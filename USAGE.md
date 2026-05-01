# Usage Guide

## When to Use Its Wrap

Its Wrap is designed for researchers who need to transition their work into product-ready decision materials. Use it when:

- You have a working prototype, demo, or experiment
- You need to communicate value to product managers or leadership
- Your research is "done" but needs framing for business decisions
- You want to identify gaps before pitching your work

## Quick Examples

### Example 1: LLM Research Demo

**Input:**
```
We built an LLM that automatically categorizes support tickets.
It works on 200 historical tickets but we haven't measured accuracy.
We think it could save time for the support team.
```

**What Its Wrap does:**
- Identifies missing metrics (accuracy, baseline time savings)
- Frames the user problem (support team manual work)
- Structures the evidence gap
- Proposes proxy metrics
- Suggests validation next steps

### Example 2: Vibe-Coded Prototype

**Input:**
```
I made a React app with a Python backend that visualizes
user behavior patterns. It's deployed on Vercel.
```

**What Its Wrap does:**
- Maps frontend/backend to product features
- Identifies what's demoable vs production-ready
- Flags missing: auth, scalability, data pipeline
- Suggests which parts can be shown to PMs now

### Example 3: Algorithm Research

**Input:**
```
We developed a new recommendation algorithm.
Offline evaluation shows 15% better precision.
```

**What Its Wrap does:**
- Questions: online validation, latency, A/B test plan
- Identifies missing: user impact metrics, integration cost
- Structures the offline→online validation gap

## Workflow

### Step 1: Prepare Your Input

Gather whatever you have:
- Demo links or screenshots
- Code repositories
- Experiment results
- Notes or documents
- User feedback (even informal)

### Step 2: Engage Claude with Its Wrap

Simply describe your research and ask for a product decision handoff:

```
"I have this demo [describe or share]. Can you help me turn this
into something my PM can use to decide next steps?"
```

Claude will automatically invoke the Its Wrap skill.

### Step 3: Respond to Clarifying Questions

Its Wrap may ask follow-up questions if critical information is missing:

- "Who is the target user?"
- "What problem does this solve?"
- "Do you have any usage metrics?"

These questions help produce a more useful output.

### Step 4: Review the Output

The skill produces a structured handoff package with:

1. **Executive Summary** - Quick decision recommendation
2. **Problem & User Scenario** - Why this matters
3. **Research Asset Reconstruction** - What exists now
4. **Productized Solution** - What it could become
5. **Decision Evidence** - What's proven vs assumed
6. **Non-Quantitative Value** - Strategic/experience value
7. **Alternatives** - Simpler options considered
8. **Execution Path** - How to get from here to shipped
9. **Cost Model** - Development and operational costs
10. **Risks & Boundaries** - What could go wrong
11. **Data Loop** - How to measure and improve
12. **Missing Information** - Known gaps to fill
13. **Next Actions** - Concrete recommended steps

### Step 5: Iterate or Share

- Use the output to guide further research
- Share the package with your PM
- Fill in missing items marked as `TBD`

## Tips for Best Results

### Do:
- Share working demos when possible
- Be honest about what's unverified
- Think about users before technology
- Consider simpler alternatives

### Don't:
- Hide missing information
- Overstate evidence
- Skip the user problem
- Force a decision before validation

## Common Patterns

### Pattern: Research → Pilot

Use when you have promising results but need validation:

1. Its Wrap identifies evidence gaps
2. Structures pilot requirements
3. Defines success metrics
4. Proposes phased rollout

### Pattern: Demo → Product

Use when you have a working prototype:

1. Its Wrap maps demo features to product value
2. Identifies productionization gaps
3. Suggests MVP scope
4. Flags technical debt

### Pattern: Algorithm → Feature

Use when you have technical improvements:

1. Its Wrap translates technical gains to user value
2. Structures A/B test plan
3. Identifies integration requirements
4. Proposes rollout strategy

## Advanced Usage

### Customizing the Output

You can ask for specific adaptations:

- "Focus on the cost model for leadership"
- "Emphasize the technical risks for engineering review"
- "Make this concise for a quick pitch"

The skill will adapt depth and emphasis while maintaining coverage of required areas.

### Handling Multiple Stakeholders

If you need versions for different audiences:

```
"Create a version for my PM focused on execution,
and a version for leadership focused on ROI."
```

Its Wrap can produce adapted outputs for different decision-makers.

## Troubleshooting

### Output is too long

Ask for a condensed version:
```
"Give me an executive summary only"
```

### Missing critical section

Point it out:
```
"I need more detail on the risk assessment"
```

### Unclear terminology

Ask for clarification:
```
"What do you mean by 'proxy metrics'?"
```

## Integration with Other Skills

Its Wrap works well with:

- **brainstorming** - For exploring product possibilities
- **writing-plans** - For turning the execution path into a project plan
- **test-driven-development** - For building validated research

## See Also

- [README.md](README.md) - Overview and introduction
- [INSTALL.md](INSTALL.md) - Installation instructions
- `.skill/SKILL.md` - Full skill specification
