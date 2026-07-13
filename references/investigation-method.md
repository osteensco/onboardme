# Investigation method

Use this method to build the map and guide behavior tracing without turning the session into a file tour.

## Repository reconnaissance

1. Read repository instructions before running commands or changing files.
2. Establish the product purpose, system boundary, users, and expected learner work.
3. Locate manifests, build entry points, runtime entry points, tests, configuration, schemas, migrations, CI, deployment definitions, and operational documentation.
4. Separate active source from generated, vendored, archived, experimental, and legacy code.
5. Identify the repository's own setup, test, lint, debug, and observability paths.
6. Inspect recent history and high-change areas only after establishing the current structure.
7. Record uncertainties and contradictions explicitly.

Avoid exhaustive inventories. Map components at the level needed to explain responsibilities and dependency direction.

## Vertical trace

For a representative behavior, determine:

- external trigger and observable result;
- runtime entry point;
- authentication, authorization, and validation boundaries;
- orchestration and domain rules;
- state reads and writes;
- transaction or consistency boundary;
- external calls and emitted messages;
- errors, retries, idempotency, and partial failures;
- logs, metrics, and traces;
- focused tests;
- historical rationale where the implementation is surprising.

Ask the learner to predict each major transition before following it. Confirm static conclusions dynamically when safe and proportionate through a focused test, breakpoint, local trace, structured log, query observation, or temporary instrumentation.

## Search strategy to teach

1. Start from an externally observable identifier: route, command, message, error text, event, table, or configuration key.
2. Find its boundary and definition.
3. Follow symbol references and dependency direction.
4. Inspect focused tests for behavior and vocabulary.
5. Run the smallest safe experiment that distinguishes competing explanations.
6. Consult Git history for rationale, not as a substitute for current behavior.
7. Summarize supported conclusions and remaining uncertainty.

## Claim discipline

Tag important claims:

- `verified`: directly supported by sufficient current evidence;
- `documented`: stated by project documentation but not independently confirmed;
- `inferred`: best explanation from indirect evidence;
- `contradicted`: credible evidence disagrees;
- `unknown`: evidence is insufficient.

Include evidence next to the claim. A useful entry contains the statement, status, file or symbol references, runtime or test observation, last-checked commit when helpful, and an explicit verification step for anything unresolved.

## Counterfactual prompts

Choose counterfactuals that expose the learner's causal model:

- What if persistence succeeds but the response is lost?
- What if the same event arrives twice?
- What if two actors update this state concurrently?
- What if validation passes but the external dependency fails?
- What if old and new application versions run together?
- What observable signal would distinguish this failure from a nearby one?
