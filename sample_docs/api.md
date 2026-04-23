# API Reference

## Authentication
All API requests require a Bearer token in the Authorization header.

```
Authorization: Bearer <your-token>
```

## Endpoints

### POST /v1/chat
Send a message to an agent.

**Request body:**
- `agent_id` (string, required) — The agent to message
- `message` (string, required) — The user message
- `session_id` (string, optional) — Resume a previous session

**Response:**
- `response` (string) — The agent's reply
- `tokens_used` (integer) — Tokens consumed
- `session_id` (string) — Session identifier for continuity

### GET /v1/agents
List all available agents.

### GET /v1/agents/{id}/status
Get an agent's current status and budget usage.

## Rate Limits
- 100 requests per minute per API key
- 10,000 tokens per request maximum
- Budget limits are enforced server-side
