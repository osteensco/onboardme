# Onboard Me

An agent skill for learning an unfamiliar codebase through evidence-backed
investigation, runtime tracing, graduated implementation missions, and
teach-back.

## Install

Install the skill from GitHub with the [Skills CLI](https://skills.sh):

```sh
npx skills add osteensco/onboardme
```

To install it non-interactively for a specific agent, pass the agent name and
accept the defaults:

```sh
npx skills add osteensco/onboardme --agent codex --yes
```

You can inspect the skill before installing it:

```sh
npx skills add osteensco/onboardme --list
```

For local development, run the same discovery check against this checkout:

```sh
npx skills add . --list
```

## What's included

- `SKILL.md` contains the main onboarding workflow.
- `references/` contains the investigation method, mission catalog, and
  assessment rubric loaded by the skill when needed.
- `assets/templates/` contains reusable apprenticeship artifacts.
- `agents/openai.yaml` contains the OpenAI agent interface metadata.

The repository intentionally keeps `SKILL.md` at its root. This is a standard
Skills CLI discovery location, and the referenced files are installed with it.
