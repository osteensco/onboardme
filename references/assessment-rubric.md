# Assessment rubric

Assess demonstrated capability using submitted evidence and observed independence. Do not score speed, confidence, writing polish, or agreement with the agent.

## Capability levels

- **Not demonstrated:** Cannot complete the work or provides unsupported conclusions.
- **Demonstrated with guidance:** Completes the work with procedural direction or revealed answers.
- **Demonstrated with hints:** Leads the work but needs bounded prompts or corrections.
- **Independent:** Selects an effective method, produces sufficient evidence, detects uncertainty, and completes the work safely.
- **Can teach:** Explains the causal model, alternatives, failure paths, and investigation method clearly enough to guide another programmer.

## Assessment dimensions

### Operate

- Runs the relevant system or subsystem safely.
- Understands important local dependencies and configuration.
- Uses focused commands and interprets failures rather than blindly retrying.

### Navigate

- Starts from observable behavior and finds the responsible boundary.
- Follows symbols, state, and dependency direction efficiently.
- Distinguishes active, generated, test, and legacy code.

### Explain

- Connects implementation details to domain meaning.
- Identifies invariants, state changes, external effects, and consistency boundaries.
- Separates verified facts from inference and unknowns.

### Verify

- Cites concrete code, tests, configuration, history, or runtime observations.
- Uses an experiment capable of distinguishing competing explanations.
- Notices contradictions and weak evidence.

### Debug

- Reproduces or sharply characterizes the failure.
- Narrows hypotheses using observations.
- Explains the causal chain and identifies adjacent failure modes.

### Change safely

- Predicts affected components and behavior before editing.
- Protects domain invariants and compatibility.
- Tests success, failure, and regression behavior proportionately.
- Considers rollout, observability, migration, and rollback when relevant.

### Teach back

- Reconstructs the flow without agent narration.
- Answers counterfactual questions consistently.
- States risks and unresolved questions without bluffing.

## Recording an assessment

Record the mission, assistance level, demonstrated findings, cited evidence, misconceptions, unresolved questions, capability levels, and recommended next mission. Treat the assessment as revisable when better evidence appears.

## Completion standard

Do not declare the apprenticeship complete until the learner independently handles an unfamiliar but representative issue: reproduce or characterize it, locate the behavior, explain domain and technical effects, identify state and failure paths, propose a safe response, implement and validate it when authorized, and communicate risks and uncertainty.
