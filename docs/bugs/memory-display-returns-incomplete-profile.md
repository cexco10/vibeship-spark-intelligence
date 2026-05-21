# Bug: Memory display returns only one fact despite having more saved

## Summary
When asked "Show me my memory. What do you know about me?"
Spark replies with only one fact despite having multiple
saved memories about the user.

## Steps to Reproduce
1. Save multiple facts using /remember:
   - /remember My name is Celestine
   - /remember I prefer dark mode
   - /remember My favorite color is Yellow
2. Send: "Show me my memory. What do you know about me?"
3. Spark replies: "You're Celestine."

## Expected Behavior
Spark should display all saved memories in a clear list:
- Name: Celestine
- Preference: dark mode
- Favorite color: Yellow
- Current task: Spark Compete bug hunt

## Actual Behavior
Spark returned only one fact: "You're Celestine."
All other saved memories were ignored.

## Impact
Users cannot verify what Spark has saved about them.
This breaks trust in the memory system.

## Fix
Memory display should query and return all saved
profile facts, not just the most recent or most
prominent one.

## Team
Team name: Celestine Team
Discovered via: Spark Compete Bugs & Goblins Hunt — Mission #28
LLM used: Minimax
