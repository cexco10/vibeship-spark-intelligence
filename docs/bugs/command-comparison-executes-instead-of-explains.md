# Bug: Command comparison request executes instead of explaining

## Summary
When asked to compare /run /board and /mission status,
Spark executes /board and shows current state instead
of explaining what each command does and how they differ.

## Steps to Reproduce
1. Send: "Compare /run /board and /mission status for me. What is the difference?"
2. Spark shows current mission board state
3. No explanation of what each command does is given

## Expected Behavior
Spark should explain:
- /run: starts a new mission
- /board: shows current mission state
- /mission status: checks a specific mission
And how they differ in purpose and usage.

## Actual Behavior
Spark ran /board and dumped current mission state
with no explanation of command differences.

## Team
Team name: Celestine Team
Discovered via: Spark Compete Bugs & Goblins Hunt — Mission #22
LLM used: Minimax 2.7
