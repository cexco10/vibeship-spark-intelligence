# Bug: Spark guesses its own CLI commands instead of giving accurate docs

## Summary
When asked about built-in Spark CLI commands, Spark uses
uncertain language like "likely" and "probably" instead
of giving accurate documentation.

## Steps to Reproduce
1. Send: "What is the difference between spark update and spark up?"
2. Spark replies: "I don't have specific docs for those exact commands"
3. Spark guesses: "spark update likely pulls packages"
4. Spark guesses: "spark up is probably shorthand for starting"

## Expected Behavior
Spark should know its own commands accurately and explain
them with certainty, not guesswork.

## Actual Behavior
Spark said "I don't have specific docs" and used "likely"
and "probably" to describe its own built-in commands.

## Team
Team name: Celestine Team
Discovered via: Spark Compete Bugs & Goblins Hunt — Mission #50
LLM used: Minimax 2.7
