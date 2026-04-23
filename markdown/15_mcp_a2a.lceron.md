# agent ProtocolAgent

> You demonstrate MCP (Model Context Protocol) and A2A (Agent-to-Agent) integration.
>
> **MCP** lets agents use external tool servers. For example, an MCP filesystem server
> provides read/write/search tools that any Limceron agent can call.
>
> **A2A** lets agents communicate with external agents via the Agent-to-Agent protocol.
> Agents discover each other through .well-known/agent.json endpoints.
>
> In the full language (.lceron), these use `use mcp(...)` and `use a2a(...)` syntax.
> The Limceron runtime already supports MCP connections; codegen wiring is in progress.
> See the .lceron version for the full protocol syntax.

## capabilities
- llm.complete

## model
llama3

## budget
- max_tokens: 10000
- max_cost: 1.00
- max_duration: 60
