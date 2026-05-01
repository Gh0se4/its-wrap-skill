# Contributing to Its Wrap

Thank you for your interest in improving Its Wrap! This document provides guidelines for contributing.

## Ways to Contribute

### 1. Report Issues

Found a bug or have a suggestion? Open an issue on GitHub:

- Describe the problem or suggestion clearly
- Include examples of input/output where relevant
- Suggest expected behavior if applicable

### 2. Submit Pull Requests

Want to improve the skill directly? Here's how:

#### Setup

```bash
# Fork the repository on GitHub
# Clone your fork
git clone https://github.com/YOUR_USERNAME/its-wrap-skill.git
cd its-wrap-skill

# Create a branch for your changes
git checkout -b feature/your-improvement
```

#### Making Changes

Focus on `.skill/SKILL.md` for core skill changes:

```bash
# Edit the skill file
vim .skill/SKILL.md

# Test your changes in Claude Code
cp -r .skill ~/.claude/skills/its-wrap-test
# Test with various research inputs
```

#### Guidelines

- **Preserve the structure**: Keep YAML frontmatter intact
- **Maintain clarity**: Skill outputs should be clear and actionable
- **Test with real inputs**: Verify changes work with actual research scenarios
- **Update documentation**: If behavior changes, update USAGE.md

#### Submit

```bash
# Commit with clear message
git add .
git commit -m "Improve: clarify proxy metrics section"
git push origin feature/your-improvement

# Open Pull Request on GitHub
```

### 3. Share Examples

Real-world usage examples help others learn:

- Open an issue with "Example: " prefix
- Describe your research context
- Share (sanitized) input and output
- Explain what worked or what could improve

### 4. Improve Documentation

Documentation improvements are always welcome:

- Fix typos or unclear explanations
- Add more usage examples
- Improve installation instructions
- Translate to other languages

## Design Principles

When contributing, keep these principles in mind:

### 1. Researcher-First

The skill serves researchers who need to communicate with PMs. Keep language accessible while maintaining rigor.

### 2. Decision-Support, Not Decision-Making

Its Wrap prepares materials for decisions, but doesn't make them. Preserve the PM's agency.

### 3. Honest About Gaps

The skill should always surface missing information, never hide it.

### 4. Flexible Structure

Required thinking areas are fixed, but output format should adapt to input complexity.

## Testing Changes

Before submitting PRs, test your changes:

### Manual Testing Checklist

- [ ] Test with simple research description
- [ ] Test with complex multi-part research
- [ ] Test with vibe-coding project input
- [ ] Test with AI/LLM research
- [ ] Verify all required sections appear
- [ ] Verify missing information is flagged
- [ ] Check that output helps a real PM decision

### Example Test Inputs

```
# Simple
"Built a script that summarizes meeting transcripts"

# Complex
"We have a 3-month research project with a working prototype,
user interviews, and preliminary metrics. Need to decide
whether to spin up a product team."

# Vibe-coded
"Made a full-stack app in a weekend that does X. Deployed
to Vercel, uses Supabase, OpenAI API."
```

## Code of Conduct

- Be respectful and constructive
- Focus on improving the skill for researchers
- Share credit where due
- Respect user privacy in examples

## Questions?

Open an issue with "Question: " prefix.

## License

By contributing, you agree that your contributions will be licensed under the MIT License.
