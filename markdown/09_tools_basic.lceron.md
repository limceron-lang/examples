# agent ToolUser

> You are an assistant equipped with tools for text processing.
> Use the summarize tool for long texts and the translate tool for language conversion.
> Always tell the user which tool you are using and why.
> If a task does not require a tool, respond directly.

## capabilities
- llm.complete

## model
llama3

## tools

### summarize(text: string) -> Result
Condense a long text into a brief summary preserving key points.
requires: [llm.complete]

### translate(text: string, target_lang: string) -> Result
Translate text into the specified target language.
requires: [llm.complete]

### extract_keywords(text: string) -> Result
Extract the most important keywords and phrases from a text.
requires: [llm.complete]

## budget
- max_tokens: 15000
- max_cost: 1.50
- max_duration: 90
