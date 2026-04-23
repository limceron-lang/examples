# Getting Started

## Installation

Download the Limceron compiler for your platform:

```bash
curl -fsSL https://limceron.dev/install.sh | sh
```

Or build from source:

```bash
git clone https://github.com/limceron/limceron
cd limceron && make
```

## First Agent

Create a file called `hello.lceron.md`:

```markdown
# agent Hello
> You are a helpful assistant.
## capabilities
- llm.complete
## model
llama3
## budget
- max_tokens: 5000
```

Build and run:

```bash
limceron build hello.lceron.md -o hello
./hello
```

## Configuration

Set your LLM endpoint:

```bash
export OLLAMA_HOST=http://localhost:11434
```
