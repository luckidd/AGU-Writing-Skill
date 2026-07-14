# AGU Space Physics Writing Skill

`agu-writing` is an Agent Skill for drafting, translating, restructuring, and reviewing AGU-style manuscripts in space physics. It supports research on the Sun, heliosphere, solar wind, magnetosphere, radiation belts, ionosphere, thermosphere, radio science, and space weather.

Its core principle is simple: **write from the author’s evidence**. The skill preserves numerical values, units, notation, physical meaning, uncertainty, and the strength of scientific claims. It does not invent observations, mechanisms, references, or repository information.

## Features

* Translation and AGU-style scientific editing
* Titles, abstracts, Key Points, and Plain Language Summaries
* Introduction, Data, Methods, Results, Discussion, and Conclusions sections
* Figure captions, Open Research statements, and submission-compliance checks
* Review of claim–evidence alignment, causal reasoning, interpretation, and terminology
* Support for AGU Advances, Geophysical Research Letters, JGR: Space Physics, Space Weather, Earth and Space Science, Radio Science, and general AGU writing

## Installation

Before installing any third-party skill, review its `SKILL.md` file and accompanying resources.

This repository contains no executable scripts and does not require an API key.

### Codex

For Codex, the recommended shared Agent Skills directory is `~/.agents/skills/`.

You can also use the built-in installer from a Codex conversation:

```text
Use $skill-installer to install https://github.com/luckidd/agu-writing/tree/v1.0.0
```

User-level installation:

```bash
mkdir -p ~/.agents/skills
git clone --depth 1 --branch v1.0.0 https://github.com/luckidd/agu-writing.git ~/.agents/skills/agu-writing
```

Project-level installation:

```bash
mkdir -p .agents/skills
git clone --depth 1 --branch v1.0.0 https://github.com/luckidd/agu-writing.git .agents/skills/agu-writing
```

After starting a new session, enter `$agu-writing` to invoke the skill, or use `/skills` to confirm that it has been discovered.

### Claude Code

User-level installation:

```bash
mkdir -p ~/.claude/skills
git clone --depth 1 --branch v1.0.0 https://github.com/luckidd/agu-writing.git ~/.claude/skills/agu-writing
```

Project-level installation:

```bash
mkdir -p .claude/skills
git clone --depth 1 --branch v1.0.0 https://github.com/luckidd/agu-writing.git .claude/skills/agu-writing
```

On Windows PowerShell, use `$HOME\.claude\skills\agu-writing` for a user-level installation or `.claude\skills\agu-writing` for a project-level installation.

After installation, enter `/agu-writing` to invoke the skill explicitly, or allow Claude Code to load it automatically when relevant to the task.

### Gemini CLI

Use the installation command provided by Gemini CLI:

```bash
gemini skills install https://github.com/luckidd/agu-writing
gemini skills list
```

To install the skill only in the current workspace:

```bash
gemini skills install https://github.com/luckidd/agu-writing --scope workspace
```

To pin the installation to `v1.0.0`, use `git clone --branch v1.0.0` and set the destination directory to either `~/.gemini/skills/agu-writing` or `.gemini/skills/agu-writing`.

### OpenCode

OpenCode supports the shared `.agents/skills` directory, so you can reuse the Codex user-level or project-level installation instructions.

Alternatively, install the skill in OpenCode’s dedicated user directory:

```bash
mkdir -p ~/.config/opencode/skills
git clone --depth 1 --branch v1.0.0 https://github.com/luckidd/agu-writing.git ~/.config/opencode/skills/agu-writing
```

## Compatibility

The core `SKILL.md` file follows the open Agent Skills structure.

The `agents/openai.yaml` file provides interface metadata for Codex and the ChatGPT desktop app. Other tools can safely ignore this file without affecting the skill’s core functionality.

Installation paths are based on the current official documentation for each tool:

* [Codex Skills](https://developers.openai.com/codex/skills/)
* [Claude Code Skills](https://code.claude.com/docs/en/skills)
* [Gemini CLI Agent Skills](https://geminicli.com/docs/cli/using-agent-skills/)
* [OpenCode Agent Skills](https://opencode.ai/docs/skills/)

## Version

Current stable release: `v1.0.0`.

See [CHANGELOG.md](CHANGELOG.md) for release notes and version history.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
