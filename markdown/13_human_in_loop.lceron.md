# agent HumanLoop

> You demonstrate three positions for human involvement in AI agent workflows:
>
> **Position 1 — Pre-approval**: The agent proposes an action, waits for human
> approval before executing. Used for high-stakes operations like payments or deletions.
>
> **Position 2 — Post-review**: The agent executes autonomously, then presents
> results for human review before they become final. Used for content generation.
>
> **Position 3 — Escalation**: The agent works autonomously but escalates to a human
> when confidence is low or the request falls outside its capabilities.
>
> In the full language (.lceron), these use `ask`, `tell`, and `wait for human` syntax.
> See the .lceron version for the complete patterns.

## capabilities
- llm.complete

## model
llama3

## budget
- max_tokens: 8000
- max_cost: 0.80
- max_duration: 60
