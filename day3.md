# Make the Repository Your Single Source of Truth
Unlike human, AI has only a single source (when you given to them) and barely can figure it out outside of it. They (AI Agent) can't asking from another agent because they don't the same source.

## The concept.
- Knowledge Visibility Gap: The proportion of total project knowledge that's NOT in the repository. Depend on person/team knowledge.
- System of Record: The code repository as the authoritative source for project decisions, architecture constraints, execution state, and verification standards
- Cold-Start Test: The five questions above. How many it can answer is how complete your map is.
- Discovery Cost: How much context budget the agent burns to find a key piece of information in the repo
- Knowledge Decay Rate: Document must be sync with the code.

## Map structure.
- Going from the top should be the general rule: project overview, command line, hard constraint.
- For details and microservices will be next: back-end, api layers, database, etc.
- For progress: draft, in-progress, done.
- Standardized commands: setup, test, lint, checktandardlize.

## Excercise
Cold-start test: testing career-ops with questions below and how it response.

- What is this system?
- How is it organized?
- How do I verify it?
- What's the current progress?

Tried with one first question What is this system?, and giving a comprehensive guidance with many other questions as well. A short and concise describe about teh system, what is core abilities, how to use it and how the work process occur and how to getting started. So basically, the author did really good job at this. 

ACID assessment: well-implemented as well, all the scanned job will be store in a md file, as well as applied, evaluated cv with job description.
