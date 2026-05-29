# Preventing Agents from Declaring Victory Too Early
To clarify more clearly, from previous lecture I learn to handle list of features for agents (**The scheduler**, **verifier**, and **handoff**), and expected them to follow it.
But here any issues that could be a problem, you given the agents an list of **verifier**, agents response with all passed announce everything is "Done". When you verify yourself, there are multiple task not working properly. Then you realized it not actually done, they just **done** all the tasks you gave.

## Core Concepts
- **Premature Completion Declaration**: The agent asserts the task is complete, but unmet correctness specifications remain.
- **Confidence Calibration Bias**: A systematic gap between the agent's self-reported completion confidence and the actual completion quality.
- **Termination Criteria**: The agent must satisfy all conditions before declaring completion.
- **Verification-Validation Dual Gate**: The first layer (verification) checks whether the code correctly implements the specified behavior; the second layer (validation) checks whether system-level behavior meets end-to-end requirements.
- **Runtime Feedback Signals**: Logs, process states, and health checks from program execution—these form the objective basis for the harness to judge completion quality.
- **Completion Priority Constraint**: First verify functional correctness, then address performance, and finally handle style. No refactoring is allowed until core functionality has been verified.

# Most important: Passing Unit Tests ≠ Task Complete.

## Passing Unit Tests ≠ Task Complete

Example given by https://walkinglabs.github.io/learn-harness-engineering/en/lectures/lecture-09-why-agents-declare-victory-too-early/

## Definition of Done
- Feature complete = end-to-end verification passed, not "code is written"
- Required verification levels:
  1. Unit tests pass
  2. Integration tests pass
  3. End-to-end flow verification passes
- Do not proceed to level 2 if level 1 fails
- Do not proceed to level 3 if level 2 fails

## Exercises

## Termination Validation Function Design:
I'mn using the same project career-ops, when return the scanned result, it keep given the wrong url link to the job, most of the link are 404 meanwhile the api return status "200" which is tell it a valid link (the agent misundertand it) or general career page of the company, when you actually searching for the job, it's doesn't existed or inactive.

Solution: the content of the web page do not contain "404" or "page not found" accordingly languages.

The purporse is detect "page not found" in different languages.
