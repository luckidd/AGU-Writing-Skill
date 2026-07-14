# AGU-Writing-Skill

AGU-Writing-Skill is an Agent Skill for drafting, translating, restructuring, and auditing AGU-style space-physics manuscripts. It supports work on the Sun, heliosphere, solar wind, magnetosphere, radiation belts, ionosphere, thermosphere, radio science, and space weather.

The skill writes from the author's evidence. It preserves numerical values, units, notation, physical meaning, uncertainty, and claim strength. It does not invent observations, mechanisms, references, or repository details.

## Features

- AGU-style scientific drafting and Chinese-to-English rewriting
- Titles, abstracts, Key Points, and Plain Language Summaries
- Introductions, Data, Methods, Results, Discussions, and Conclusions
- Figure captions, Open Research statements, and submission-compliance checks
- Claim-evidence, causality, alternative-explanation, and terminology review
- Support for AGU Advances, GRL, JGR: Space Physics, Space Weather, Earth and Space Science, Radio Science, and general AGU writing

## Download

Download the ready-to-install package from the [v1.0.2 release](https://github.com/luckidd/AGU-Writing-Skill/releases/tag/v1.0.2):

- [agu-writing-skill-v1.0.2.zip](https://github.com/luckidd/AGU-Writing-Skill/releases/download/v1.0.2/agu-writing-skill-v1.0.2.zip)

After extraction, place the included `agu-writing-skill` folder in the appropriate skills directory. The target folder must directly contain `SKILL.md`, `references/`, and `agents/`; do not use an automatically created outer ZIP folder as the skill root.

This repository contains no executable code and requires no API key.

## Install

### Codex

Ask Codex to install the released skill:

```text
Use $skill-installer to install https://github.com/luckidd/AGU-Writing-Skill/tree/v1.0.2
```

Or install it manually for all of your local Agent Skills tools:

```bash
mkdir -p ~/.agents/skills
git clone --depth 1 --branch v1.0.2 https://github.com/luckidd/AGU-Writing-Skill.git ~/.agents/skills/agu-writing-skill
```

For a single project:

```bash
mkdir -p .agents/skills
git clone --depth 1 --branch v1.0.2 https://github.com/luckidd/AGU-Writing-Skill.git .agents/skills/agu-writing-skill
```

Windows PowerShell:

```powershell
New-Item -ItemType Directory -Force "$HOME\.agents\skills" | Out-Null
git clone --depth 1 --branch v1.0.2 https://github.com/luckidd/AGU-Writing-Skill.git "$HOME\.agents\skills\agu-writing-skill"
```

### Claude Code

Install for your user account:

```bash
mkdir -p ~/.claude/skills
git clone --depth 1 --branch v1.0.2 https://github.com/luckidd/AGU-Writing-Skill.git ~/.claude/skills/agu-writing-skill
```

Or install for the current project:

```bash
mkdir -p .claude/skills
git clone --depth 1 --branch v1.0.2 https://github.com/luckidd/AGU-Writing-Skill.git .claude/skills/agu-writing-skill
```

### Gemini CLI

Use Gemini CLI's installer:

```bash
gemini skills install https://github.com/luckidd/AGU-Writing-Skill
gemini skills list
```

For a fixed version or a manual installation, clone the repository into `~/.gemini/skills/agu-writing-skill` or `.gemini/skills/agu-writing-skill`.

### OpenCode

OpenCode supports the shared `.agents/skills` directory, so the Codex manual installation works unchanged. Its dedicated user-level location is also supported:

```bash
mkdir -p ~/.config/opencode/skills
git clone --depth 1 --branch v1.0.2 https://github.com/luckidd/AGU-Writing-Skill.git ~/.config/opencode/skills/agu-writing-skill
```

## Use

Start a new session after installation and invoke the skill as `AGU-Writing-Skill` (technical identifier: `$agu-writing-skill`). For example:

```text
$agu-writing-skill Rewrite the following Chinese abstract in JGR: Space Physics style. Preserve all numerical values, units, and claim strength, and identify any evidence gaps that could affect the scientific conclusion.
```

```text
$agu-writing-skill Audit this Discussion section for unsupported causality, competing explanations, and overgeneralization from a single event.
```

The skill can also activate automatically when the request clearly concerns AGU-style space-physics writing.

## Compatibility

The core `SKILL.md` follows the open Agent Skills format. `agents/openai.yaml` supplies optional UI metadata for Codex and ChatGPT Desktop; other compatible tools may ignore that file without affecting the skill.

- [Codex skills](https://developers.openai.com/codex/skills/)
- [Claude Code skills](https://code.claude.com/docs/en/skills)
- [Gemini CLI Agent Skills](https://geminicli.com/docs/cli/using-agent-skills/)
- [OpenCode Agent Skills](https://opencode.ai/docs/skills/)

## License

MIT License. See [LICENSE](LICENSE).
