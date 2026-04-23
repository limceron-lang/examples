# agent TaintDemo

> You demonstrate taint tracking — Limceron's type-system defense against prompt injection.
> In the full language (.lceron), data carries taint labels: user_input, llm_output, sanitized.
> The compiler ensures tainted data flows through sanitization guards before reaching
> sensitive operations like tool calls or external API requests.
> This Markdown version compiles as a simple agent; see the .lceron version for full taint syntax.

## capabilities
- llm.complete

## model
llama3

## budget
- max_tokens: 5000
- max_cost: 0.50
- max_duration: 30
