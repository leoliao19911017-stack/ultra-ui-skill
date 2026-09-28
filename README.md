# Ultra UI Skill

A practical workflow for steering generic, template-like AI interface output toward a distinctive, observable, and production-aware design direction.

## What it covers

- Explore directions that differ in structure, typography, color logic, material, and interaction—not just surface styling.
- Translate subjective taste into an observable brief with concrete decisions and explicit avoidances.
- Review screenshots or prototypes with an isolated visual critic that separates visible gaps from unverified risks.
- Bound revision loops with a maximum number of rounds, stop conditions, and explicit authorization for further iteration.
- Remove common AI tells, then check real content, states, accessibility, responsive behavior, performance, and polish.

The skill is framework-, model-, and vendor-agnostic. It guides design judgment; it does not replace user research, accessibility testing, or production validation.

## Repository structure

```text
ultra-ui-skill/
|-- SKILL.md                  Skill entrypoint and workflow router
|-- agents/openai.yaml        Codex UI metadata
|-- references/               Creative direction, critic, and anti-AI guidance
|-- evals/                    Baseline, with-skill results, and a visual fixture
|-- README.md
`-- LICENSE
```

## Install for Codex

PowerShell:

```powershell
$skillsRoot = if ($env:CODEX_HOME) { Join-Path $env:CODEX_HOME "skills" } else { Join-Path $HOME ".codex\skills" }
New-Item -ItemType Directory -Force -Path $skillsRoot | Out-Null
git clone https://github.com/leoliao19911017-stack/ultra-ui-skill.git (Join-Path $skillsRoot "ultra-ui-skill")
```

POSIX shell (optional):

```sh
skills_root="${CODEX_HOME:-$HOME/.codex}/skills"
mkdir -p "$skills_root"
git clone https://github.com/leoliao19911017-stack/ultra-ui-skill.git "$skills_root/ultra-ui-skill"
```

Both commands install to `~/.codex/skills/ultra-ui-skill` when `CODEX_HOME` is not set. Restart Codex or begin a new session if the skill is not discovered immediately.

## Use

Invoke it explicitly in a prompt:

```text
Use $ultra-ui-skill to turn this product brief into three genuinely different UI directions, recommend one, and define the observable design brief.
```

It may also be selected automatically when an interface risks feeling generic, template-driven, overdecorated, or recognizably AI-generated.

## Validate locally

PowerShell:

```powershell
$codexHome = if ($env:CODEX_HOME) { $env:CODEX_HOME } else { Join-Path $HOME '.codex' }
$validator = Join-Path $codexHome 'skills\.system\skill-creator\scripts\quick_validate.py'
$skill = Join-Path $codexHome 'skills\ultra-ui-skill'
python $validator $skill
```

POSIX shell:

```sh
codex_home="${CODEX_HOME:-$HOME/.codex}"
validator="$codex_home/skills/.system/skill-creator/scripts/quick_validate.py"
skill="$codex_home/skills/ultra-ui-skill"
python "$validator" "$skill"
```

The validator comes from Codex's locally installed `skill-creator` system skill. It checks skill packaging and frontmatter only; it does not prove design quality.

## Evidence and limits

The repository includes the [unassisted baseline](evals/baseline.md) and [with-skill evaluation](evals/with-skill.md). The recorded evaluations cover divergent direction exploration, subtraction before decoration, and a bounded screenshot critique. They are a small set of single-run behavioral observations, not proof of repeatable visual quality, production readiness, or superiority across models and projects.

## Source and independence

This is an independent distillation of publicly readable methods from [“How to turn your AI into a world-class designer”](https://www.lennysnewsletter.com/p/how-to-turn-your-ai-into-a-world), supplemented with clearly labeled production heuristics. It does not reproduce the article.

The public article is paywalled after the heading for Technique 7. This skill does not present unread paid material as sourced from the article.

Ultra UI Skill is not affiliated with, sponsored by, or endorsed by Lenny's Newsletter or Anshu Chimala.

## License

[MIT](LICENSE)
