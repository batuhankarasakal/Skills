# Authoring skills

This repository holds Batuhan Karasakal's original agent skills. Do not import another author's skill content unless explicitly requested and appropriately attributed.

## Structure

- Give each skill its own `skills/<name>/SKILL.md`.
- Match the folder name and frontmatter `name`. Use lowercase letters, digits and hyphens.
- Write a concise frontmatter `description` explaining what the skill does and when to use it.
- Keep templates in `templates/`. Do not publish unfinished examples as skills.
- Keep the README skill list in sync with published skills.

## Instructions

- State the intended result and the scope the skill owns.
- Prefer specific, useful decisions over generic advice the agent already knows.
- Keep the entry point focused. Move substantial conditional detail into linked references.
- Give each rule one home. Do not duplicate the same instructions across files.
- Use the target project's existing conventions and tools.
- Preserve the user's requested scope and permission boundaries. A skill does not grant approval to publish, send messages or perform destructive actions.
- Add verification that demonstrates the intended result. State what remains unverified.
- Add scripts or assets only when they solve an actual repeated need.

## Metadata and invocation

`agents/openai.yaml` is optional and can provide a display name and short description for Codex. Automatic selection is the default.

If a skill is deliberately explicit-only, set `disable-model-invocation: true` in its frontmatter for Claude Code and `policy.allow_implicit_invocation: false` in `agents/openai.yaml` for Codex.

## Before publishing

Check the frontmatter, relative links and README entry. Remove template placeholders, run any included scripts and try the skill on a representative request. Keep any validation focused on that skill's actual behavior.
