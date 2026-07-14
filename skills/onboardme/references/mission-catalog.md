# Mission catalog

Select missions that match the learner's role and the repository's real behavior. Each mission must state its objective, constraints, starting information, required findings, required evidence, counterfactual, assistance level, and completion standard.

## Orientation

- Set up and run the system from documented instructions.
- Explain each local dependency and configuration source.
- Trigger one successful workflow and identify its observable effects.
- Cause one safe failure and locate the diagnostic signal.

## Navigation and archaeology

- Find where a user-visible message originates and under which conditions.
- Trace a route, command, job, or event to the responsible domain behavior.
- Identify every enforcement point for an invariant or permission.
- Find all writers of a state field and distinguish authoritative from derived state.
- Explain a surprising implementation using code, tests, and Git history.
- Determine whether apparently legacy code is still reachable.

## Vertical tracing

- Trace the simplest successful workflow end to end.
- Trace a core business workflow across persistence and integrations.
- Trace an asynchronous producer through every active consumer.
- Compare success with timeout, retry, duplicate, or partial-failure behavior.
- Identify transaction boundaries and consistency assumptions.

## Domain understanding

- Build a glossary from code and tests, noting ambiguous terms.
- Reconstruct an entity lifecycle and verify allowed transitions.
- Explain an invariant, where it is enforced, and how it can fail.
- Distinguish source-of-truth, derived, cached, and historical data.
- Translate a product request into domain concepts and likely code locations.

## Graduated changes

1. Correct a discovered documentation error.
2. Add a focused test for existing behavior.
3. Improve diagnostics or handle a narrow edge case.
4. Make a small behavior change within one component.
5. Make a vertical change across boundary, domain, persistence, and tests.
6. Improve retry, idempotency, concurrency, or partial-failure handling.
7. Propose a cross-cutting change with migration, rollout, observability, rollback, and risk analysis.

## Debugging and review

- Diagnose a seeded or naturally occurring local failure.
- Compare an expected trace with observed behavior.
- Review a change for violated invariants, missing failure paths, or incomplete tests.
- Reconstruct an incident from logs, code, tests, and history.
- Predict the blast radius of a schema, event, configuration, or API change.

## Final challenge

Choose an unfamiliar, representative, safe issue. Provide symptoms and reproduction context, not file locations or the answer. Require independent investigation, evidence, impact analysis, an authorized implementation when appropriate, validation, and teach-back.

## Sequencing rules

- Begin with work close to the learner's expected responsibilities.
- Alternate tracing, runtime observation, domain reasoning, and changes.
- Revisit a capability in a different context before considering it durable.
- Increase ambiguity and breadth gradually.
- Reduce assistance before increasing difficulty.
- When a misconception appears, create a targeted mission rather than adding more explanation.
