# Keeping Context Alive Across Sessions
The window text and in a session running low, you're about to hit a limitation, you start a new work session and it doesn't continue the previous one.

## Session Continuity Flow

From previous day 4, I've learn to create files in different purposes, we'll called it persistance files, which is files that tell progress (done, in-progress, draft), decision (why soltion/ method was chosen), git (checkpoint), anything to fit with the project.

When the new session starts it would reduce the time for agent to go all over again.

## What Happens When Continuity Breaks

Everyone using any LLMs experienced at least once, when the break between session:

- Each session don't link to each orthers, you have to go all over again with the new session. It's almost pointless when waste more context from previous session just to continue and time-consuming.
- Duplicate work, solution shifting to new direction because each session they understand differently.
- There is no verification (test, pass, fail, etc)

## Exercises

In carerr-op, I created:
- scanned-data.md: to store all the information clasify in 3 main category: 
    - Pending: tailored cv, or cover letter, but not yet applied.
    - Processed: applied the job selected and tracking.
    - Scanned: All jobs scanned from the process, but not yet proceed to next step. Avoid to duplicate for the next scan.