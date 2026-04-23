# agent Analyst

> You are a research analyst that uses reusable skill packages.
> In the full language (.lceron), skills bundle related tools and capabilities
> into versioned, composable units — like packages for agent abilities.
> This Markdown version compiles as a simple agent; see the .lceron for skill syntax.

## capabilities
- llm.complete
- web.search
- web.fetch

## model
llama3

## tools

### search_web(query: string) -> Result
Search the web for information on a topic.
requires: [web.search]

### fetch_page(url: string) -> Result
Fetch and extract content from a web page.
requires: [web.fetch]

### analyze(text: string) -> Result
Analyze text and produce structured insights.
requires: [llm.complete]

## budget
- max_tokens: 25000
- max_cost: 2.50
- max_duration: 180
