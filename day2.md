## What Harness Actually Means
Imagine you working in a software project, you have plenty sources of information, Confluence, Slack (chatting tools), Kanban board, colleagues, etc. Morever, your have the best tool of all you **remember** things.

In the previous lession, we going through some of AI's weakness. In this lession, we leverage AI up to equal or almost to human by provide them:
- Instructions.
- Tools.
- Foundation & Environment.
- State.
- Feedback loop.

The 5 elements mention above is basic what harness is about, you provide sources and channel of information for AI so they can have a better context to execute, beside that you can add many others you see it fit with your current project.
Creating a mold that suitable with the project's needs or current's needs.

## Exercises

I'm using a repo called career-ops https://github.com/santifer/career-ops, to test the structure.

## Before create AGENTS.md

Here is the response:
- The prompt: "scan job for software engineer, web developer, qa. In Europe, within 10 days".
The Result: the output contains junior/ senior and most of the level is for senior. The location is stated is in Europe or a country in Europe, but the location show differently when check on the url given. Some link return 404 content in the webpage, but the api search return 200, so they understand that page is a valid active, and the job is posted over a year ago.

## The rules added

**The Instructions**:
- Validate Every Job Posting.
- Location Priority Order.
- Remote & Sponsorship Preferences.
- Ranking Heuristics.
- Output Expectations.

**The tools**:
- Playwright.
- webdriverIO.

**The Environment**:
- Node.js with concrete package version.

**The State**:
- Create application.md to track applied company and job.

**The Feedback**:
- Classify what item in the result are expected and not expected.
- Check if the page not contain any text like 404, page not found.

## After apply AGENS.md (Gemini in this scenario)

The process running longer this is expected. Less asking from AI during the process, return result expected 95% better than without harness in location, expiry date, confusing between api search and web search result, the job title match more correctly from original prompt.
