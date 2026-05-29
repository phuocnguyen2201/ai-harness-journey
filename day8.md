# Use Feature Lists to Constrain What the Agent Does
Everything is before it was built always have a feature lists, where is listed core functions and features must have before deliver.
Consequences, after every features are done and passed the verification then the work is done. On the other hands, agents don't understand the meaning of "done", they just fullfill the prompt you given them, and you'll have to decided is it done or not.

## Core 
 - Feature lists are harness primitives: **The scheduler**, **verifier**, and **handoff** reporter all need to read the feature list to function.
    - **Scheduler**: Reads states, picks the next not_started feature.
    - **Verifier**: Executes verification commands, decides whether to allow state transitions.
    - **Handoff reporter**: Automatically generates session handoff summaries from the feature list.
    - **Progress tracker**: Tallies state distribution, provides project health metrics.
 - Triple structure: Each feature item contains three elements: (**behavior description**, **verification command**, **current state**).
 - State machine model: Each feature item has four states — **not_started**, **active**, **blocked**, **passing**.
 - Pass-state gating: The only way a feature moves from **"active"** to **"passing"** is by the verification command executing successfully.
 - Single source of truth: All information about "what needs to be done" must derive from one feature list.
 - Back-pressure: The number of features that haven't passed yet is the pressure the harness exerts on the agent.