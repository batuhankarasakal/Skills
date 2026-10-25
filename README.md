# Batu's skills

My agent skills for design and building software.

## Skills

No skills published yet. This repository is ready for the first one.

## Add a skill

1. Create `skills/your-skill-name/` using lowercase letters and hyphens.
2. Copy [the skill template](templates/SKILL.md.example) into that folder as `SKILL.md`.
3. Replace every placeholder with your own instructions.
4. Optionally copy [the Codex metadata template](templates/openai.yaml.example) to `agents/openai.yaml` inside the skill folder.
5. Add a link and short description to the Skills section above.

```text
skills/
  your-skill-name/
    SKILL.md
    agents/
      openai.yaml       Optional Codex display metadata
    references/        Optional detailed guidance
    scripts/           Optional executable helpers
    assets/            Optional output resources
```

Start with `SKILL.md` alone. Add supporting files only when the skill needs them, and link to them from its instructions.

Read [AGENTS.md](AGENTS.md) for authoring conventions. Templates live outside `skills/` so they are not offered as installable skills.

## Install

Once the first skill is published:

```bash
npx skills add batuhankarasakal/Skills
```

To install a particular skill:

```bash
npx skills add batuhankarasakal/Skills --skill your-skill-name
```

For Codex, invoke an installed skill with `$your-skill-name`. For Claude Code, use `/your-skill-name`.

### Claude Code plugin

The plugin manifest is prepared. Once skills are published:

```text
/plugin marketplace add batuhankarasakal/Skills
/plugin install batu-skills@batu-skills
```

## Inspiration

The repository organization is inspired by [Jakub Krehel's skills](https://github.com/jakubkrehel/skills). His skill content is not included here. The skills published here will be my own.

## License

[MIT](LICENSE).
