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

- `skills/onboardme/SKILL.md` contains the main onboarding workflow.
- `skills/onboardme/references/` contains the investigation method, mission catalog, and
  assessment rubric loaded by the skill when needed.
- `skills/onboardme/assets/templates/` contains reusable apprenticeship artifacts.
- `skills/onboardme/agents/openai.yaml` contains the OpenAI agent interface metadata.

When asked to persist an apprenticeship, the skill stores all generated
artifacts under the target repository's `.onboardme/` directory and adds
`/.onboardme/` to that repository's root `.gitignore`.

The complete skill bundle lives under `skills/onboardme/` so Skills CLI installs
its referenced files together with `SKILL.md`.
