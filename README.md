# Limceron Examples

Example programs demonstrating Limceron language features.

## Structure

- `language/` — `.lceron` source files (compilable)
- `markdown/` — `.lceron.md` files (Markdown-as-source, also compilable)

## Highlights

| Example | Features |
|---------|----------|
| `01_hello_agent.lceron` | Basic agent with ask() |
| `11_supervisor.lceron` | Supervisor with restart strategies |
| `16_inference_router.lceron` | Model routing |
| `20_medical_categorizer.lceron` | Production: MySQL + LLM |
| `25_exit_case_patana.lceron` | Production: ONNX BERT + entropy circuit breaker |

## Markdown-as-source

Every `.lceron.md` file is simultaneously a readable document and a compilable program:

```bash
limceron build examples/markdown/25_exit_case_patana.lceron.md -o categorizer
```

## Quick links

- [Main repository](https://github.com/limceron/limceron)
- [Language specification](https://github.com/limceron/spec)
