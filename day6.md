# Make the Agent Initialize Before Every Work Session

You start coding with agent as usual, new project is initialized, the agent do what they are alway best to implement things immediately. It work in the first try, then add something new everything breakdown, agent given the same solution over and over again, but it doesn't work and turn out, because the project is not yet config properly.

## Core Concepts
- Initialization Phase: Establishes the prerequisites for subsequent implementation.
- Startup Readiness Checklist: operated by a fresh agent session: can start, can test, can see progress, can pick up next steps. Four conditions, all required.
- Always Ready to Hand Off: The project is in a state at any given moment where a fresh agent can take over
- Time from Start to First Passing Test: The time from project start until the first feature point passes verification.
- Success Rate of Subsequent Sessions: The proportion of subsequent sessions that can successfully execute tasks without relying on implicit knowledge.

## Best practice.

- Verifiable environment, framework environment.
- Provide test sample.
- Startup readiness checklist document.
- Git checkpoint.