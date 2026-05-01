# Installation Guide

## Quick Start

### Option 1: Clone and Install (Recommended)

```bash
# Clone the repository
git clone https://github.com/Gh0se4/its-wrap-skill.git

# Navigate to the skill directory
cd its-wrap-skill

# Install for Claude Code
# Copy the .skill folder to your Claude Code skills directory
cp -r .skill ~/.claude/skills/its-wrap

# Or for Codex (if using)
cp -r .skill ~/.agents/skills/its-wrap
```

### Option 2: Direct Download

```bash
# Download the skill file directly
curl -o ~/.claude/skills/its-wrap/SKILL.md \
  https://raw.githubusercontent.com/Gh0se4/its-wrap-skill/main/.skill/SKILL.md
```

## Claude Code Installation

### Method 1: Automatic Discovery (Recommended)

Claude Code will automatically discover skills in `~/.claude/skills/`:

```bash
# Create the skills directory if it doesn't exist
mkdir -p ~/.claude/skills

# Clone or copy the skill
git clone https://github.com/Gh0se4/its-wrap-skill.git /tmp/its-wrap
cp -r /tmp/its-wrap/.skill ~/.claude/skills/its-wrap
```

Restart Claude Code and the skill will be available.

### Method 2: Project-Level Installation

For project-specific use:

```bash
# In your project root
mkdir -p .claude/skills
cp -r /path/to/its-wrap-skill/.skill .claude/skills/its-wrap
```

## Verification

After installation, verify the skill is available:

```bash
# List available skills
ls ~/.claude/skills/

# Should show: its-wrap/
```

## Usage

Once installed, the skill is automatically available. When you have research content to convert to product decision material, Claude will use this skill to guide the process.

Example trigger phrases:
- "I have a research demo that needs to become a product decision doc"
- "Turn this prototype into something my PM can review"
- "Help me hand off this research to product management"
- "Convert this vibe-coding project into a decision package"

## Uninstallation

```bash
# Remove the skill
rm -rf ~/.claude/skills/its-wrap
```

## Troubleshooting

### Skill not appearing

1. Check the directory structure:
   ```bash
   ls -la ~/.claude/skills/its-wrap/
   # Should contain: SKILL.md
   ```

2. Restart Claude Code to refresh skill discovery

3. Verify the skill file is valid YAML at the top of SKILL.md

### Permission issues

```bash
# Fix permissions
chmod 644 ~/.claude/skills/its-wrap/SKILL.md
```

## Platform-Specific Notes

### macOS

Default skills directory: `~/.claude/skills/`

### Linux

Default skills directory: `~/.claude/skills/`

### Windows (WSL)

Default skills directory: `~/.claude/skills/`

## Next Steps

See [USAGE.md](USAGE.md) for detailed usage examples and workflows.
