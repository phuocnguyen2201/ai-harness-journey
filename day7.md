# Draw Clear Task Boundaries for Agents

Agents are alway with "do a little extra", they provide more than project's needs, if they see things related to the project. So, set clear boundaries for agents is an essential, avoid prompts that too broad for agents.

## Core Concepts
- Overreach or under-finish: these are two side of one coin, agent provide so much context you asking for or the work done below expectation, result none of them giving the best result.
- WIP Limit (Work-in-Progress Limit): limit tasks all-in-one go, finish one then move to a new one.
- Completion Evidence: verify the task as "done" and then allow agent to move to next task.
- Scope Surface: A DAG structure where each node is a work unit and edges are dependencies.
- Completion Pressure: The constraining force the harness exerts through WIP limits and completion evidence requirements, forcing the agent to finish the current task before starting a new one.

## Exercises

- Task Atomization: Career-op contain many many job seeking website from across the globle, if the prompt to tell agent to search job from all of those website would be time-consuming.
    - Narrow down the group of website: proritize my current location, group website as location or continent narrow number down to 5 countries, 3 job each website, languages: English, hybrid or remote, etc.
    - Verify the job post still valid as the return code is 200, posted date is still valid, location is solid display.
    - If everything above is valid and pass, put the found job advertise in category accordingly their location.

- Comparison Experiment & Completion Evidence Audit:
    - Without constraints: the quote spent 30% for one scan, due to high number in job seeking website, the location is unclear, the date and the job advertise is expired (some job was 2 years ago), link are no longer valid, 404 or other error code, etc.
    - With constraints: the return result better with category in countries, location, job title, company name, how long the job was posted, link to the job post. The quote spent less, just 7% - 15% per scan but with many valid job advertises. The link to job ad is valid.

-