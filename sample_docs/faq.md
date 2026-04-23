# Frequently Asked Questions

**Q: What LLM providers does Limceron support?**
A: Limceron connects to any OpenAI-compatible API. Use Ollama for local models or point to cloud providers.

**Q: Can an agent exceed its budget?**
A: No. The runtime enforces budgets at the system level. An agent physically cannot make an LLM call that would exceed its limits.

**Q: What is the difference between .lceron and .lceron.md?**
A: They compile to the same binary. The .lceron.md format uses Markdown syntax for zero learning curve. The .lceron format adds guards, taints, supervisors, and other advanced features.

**Q: How does memory work?**
A: When `memory: true`, the runtime stores every interaction in a local SQLite database (lcn_memory.db). The agent can recall context from previous sessions automatically.

**Q: What is taint tracking?**
A: Taint types mark data provenance (user_input, llm_output, sanitized). The compiler ensures tainted data flows through guards before reaching sensitive operations, preventing prompt injection at the type-system level.
