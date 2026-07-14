# AGU Space Physics Writing Skill

`agu-writing` is an Agent Skill for drafting, translating, restructuring, and auditing AGU-style space-physics manuscripts. It supports the Sun, heliosphere, solar wind, magnetosphere, radiation belts, ionosphere, thermosphere, radio science, and space weather.

Its central rule is simple: write from the author's evidence. The skill preserves numbers, units, notation, physical meaning, uncertainty, and claim strength; it never invents observations, mechanisms, references, or repository details.

## 功能

- 中译英与 AGU 风格科学改写
- 标题、摘要、Key Points 和 Plain Language Summary
- Introduction、Data、Methods、Results、Discussion 和 Conclusions
- 图注、Open Research 声明与投稿合规检查
- 论点—证据、因果关系、竞争性解释和术语审查
- AGU Advances、GRL、JGR: Space Physics、Space Weather、Earth and Space Science、Radio Science 与通用 AGU 写作

## 仓库结构

```text
AGU-Writing-Skill/
├── README.md
├── CHANGELOG.md
├── LICENSE
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── agu-compliance.md
    ├── claim-evidence-review.md
    ├── examples-front-matter.md
    ├── examples-study-design.md
    ├── examples-main-text.md
    ├── examples-figures-open-research.md
    ├── journal-modes.md
    ├── section-templates.md
    └── space-physics-style.md
```

## 安装

安装第三方 skill 前，请先查看 `SKILL.md` 和配套文件。本仓库不包含可执行脚本，也不需要 API key。

### 直接下载（ZIP）

从 [v1.0.1 发布页](https://github.com/luckidd/AGU-Writing-Skill/releases/tag/v1.0.1) 下载 `agu-writing-v1.0.1.zip`，解压后将其中的 `agu-writing` 文件夹整体放入所用工具的 skills 目录。不要把 ZIP 解压后自动生成的外层目录直接作为 skill 目录；目标目录必须是 `agu-writing`，其中应直接包含 `SKILL.md`、`references/` 和 `agents/`。

### Codex

Codex 推荐使用共享 Agent Skills 路径 `~/.agents/skills/`。在 Codex 对话中也可以调用内置安装器：

```text
Use $skill-installer to install https://github.com/luckidd/AGU-Writing-Skill/tree/v1.0.1
```

用户级手动安装：

```bash
mkdir -p ~/.agents/skills
git clone --depth 1 --branch v1.0.1 https://github.com/luckidd/AGU-Writing-Skill.git ~/.agents/skills/agu-writing
```

Windows PowerShell：

```powershell
New-Item -ItemType Directory -Force "$HOME\.agents\skills" | Out-Null
git clone --depth 1 --branch v1.0.1 https://github.com/luckidd/AGU-Writing-Skill.git "$HOME\.agents\skills\agu-writing"
```

项目级安装：

```bash
mkdir -p .agents/skills
git clone --depth 1 --branch v1.0.1 https://github.com/luckidd/AGU-Writing-Skill.git .agents/skills/agu-writing
```

新建会话后输入 `$agu-writing`，或使用 `/skills` 确认是否已发现。

### Claude Code

用户级安装：

```bash
mkdir -p ~/.claude/skills
git clone --depth 1 --branch v1.0.1 https://github.com/luckidd/AGU-Writing-Skill.git ~/.claude/skills/agu-writing
```

项目级安装：

```bash
mkdir -p .claude/skills
git clone --depth 1 --branch v1.0.1 https://github.com/luckidd/AGU-Writing-Skill.git .claude/skills/agu-writing
```

Windows PowerShell 中可将目标目录改为 `$HOME\.claude\skills\agu-writing` 或 `.claude\skills\agu-writing`。安装后输入 `/agu-writing` 显式调用，或让 Claude Code 根据任务自动加载。

### Gemini CLI

使用 Gemini CLI 自带的安装命令：

```bash
gemini skills install https://github.com/luckidd/AGU-Writing-Skill
gemini skills list
```

仅安装到当前工作区：

```bash
gemini skills install https://github.com/luckidd/AGU-Writing-Skill --scope workspace
```

如需固定为 `v1.0.1`，使用 `git clone --branch v1.0.1`，并将目标目录设为 `~/.gemini/skills/agu-writing` 或 `.gemini/skills/agu-writing`。

### OpenCode

OpenCode 支持共享 `.agents/skills` 路径，因此可复用 Codex 的用户级或项目级安装方式。也可以使用 OpenCode 专用用户目录：

```bash
mkdir -p ~/.config/opencode/skills
git clone --depth 1 --branch v1.0.1 https://github.com/luckidd/AGU-Writing-Skill.git ~/.config/opencode/skills/agu-writing
```

项目级目录为 `.opencode/skills/agu-writing` 或 `.agents/skills/agu-writing`。

## 使用示例

Codex：

```text
$agu-writing 将下面的中文摘要改写为 JGR: Space Physics 风格英文。保留全部数值、单位和结论强度，并指出影响科学结论的信息缺口。
```

Claude Code：

```text
/agu-writing Audit this Discussion section for unsupported causality, competing explanations, and overgeneralization from a single event.
```

自动触发式提示：

```text
Please revise these three Key Points for a GRL submission. Do not introduce claims that are absent from the Results.
```

## 兼容性说明

核心 `SKILL.md` 使用开放的 Agent Skills 结构。`agents/openai.yaml` 为 Codex/ChatGPT 桌面端提供界面元数据；其他工具会忽略该文件，不影响 skill 的核心功能。

安装路径依据各工具的当前官方文档：

- [Codex skills](https://developers.openai.com/codex/skills/)
- [Claude Code skills](https://code.claude.com/docs/en/skills)
- [Gemini CLI Agent Skills](https://geminicli.com/docs/cli/using-agent-skills/)
- [OpenCode Agent Skills](https://opencode.ai/docs/skills/)

## 版本

当前稳定版本：`v1.0.1`。变更见 [CHANGELOG.md](CHANGELOG.md)。

## License

MIT License. See [LICENSE](LICENSE).
