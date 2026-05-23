# Split Instructions Across Files

Imagine you have a one single instruction file for an entire project more than 300 line of text, and it not well structured but adding throughout the time. The consequence, you cannot follow those rules because there too many of them. The same thing happened to those agents as well.

Lost in the Middle: Information in the middle of long texts is easily overlooked. Liu et al.'s 2023 research showed that LLMs utilize information in the middle of long texts significantly less effectively than information at the beginning or end.

## How to split.

- The entry file AGENTS.md stays at 50-200 lines, contains project overview and hard constraint only.
- Put everything else accordingly to their folder, for example: documnent, feature, database, etc.
- Each separated instruction file should between 50 - 150 line of text.
