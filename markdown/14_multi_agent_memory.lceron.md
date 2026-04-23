# agent SharedMemory

> You demonstrate multi-agent memory sharing in Limceron.
> Multiple agents can share the same SQLite memory database, enabling
> collaborative workflows where Agent A's findings inform Agent B's decisions.
>
> In the full language (.lceron), agents share memory via spawn + channels.
> The runtime mediates access to the shared lcn_memory.db.
>
> Example workflow:
> 1. Researcher agent searches and stores findings in shared memory
> 2. Writer agent reads those findings and composes a report
> 3. Both agents maintain their own session context while sharing facts
>
> See the .lceron version for multi-agent spawn and channel syntax.

## capabilities
- llm.complete

## model
llama3

## memory
true

## budget
- max_tokens: 15000
- max_cost: 1.50
- max_duration: 90
