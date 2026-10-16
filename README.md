<p align="center"><img src="assets/logo.svg" width="72" alt="ToDo List MCP logo"></p>

# ToDo List MCP — Cursor plugin

[ToDo List MCP](https://todolistmcp.com) is an AI-forward list and notes service built for agents and the humans they look after. Your agent can create lists, add and complete items, set due dates and tags, and share lists — and you see the same lists in the web app.

This plugin connects Cursor to the hosted server. It contains no server code and no API keys: it points at `https://todolistmcp.com/mcp` and authentication is handled with OAuth.

## Install

**From the Cursor Marketplace:** search for **ToDo List MCP** and click install.

**Locally (for testing):**

```bash
git clone https://github.com/torrancemiller/todolistmcp-plugin ~/.cursor/plugins/local/todolist-mcp
```

Restart Cursor (or reload the window); the `todolist` MCP server appears under MCP settings.

## Sign in

The first time an agent calls a ToDo List MCP tool, Cursor opens todolistmcp.com in your browser. Sign in with **Google** or with a **one-time email code**, approve access, and you're done. Tokens are scoped (`lists:read`, `lists:write`, `lists:share`) and can be revoked from your account on todolistmcp.com.

## Configuration

None. There are no variables or keys to set.

## Example prompts

- "Make a packing list for a 5-day beach trip and add it to ToDo List MCP."
- "What's overdue on my lists this week?"
- "Mark 'book flights' done on my Jamaica list and add 'renew passport' due Friday."
- "Turn the TODOs in this file into items on a new list called 'Refactor'."
- "Share my grocery list with sam@example.com."

## Support

- Issues and feature requests: https://github.com/torrancemiller/todolistmcp-plugin/issues
- Email: [apps@clordo.com](mailto:apps@clordo.com)

## Links

- Website: https://todolistmcp.com
- MCP endpoint: https://todolistmcp.com/mcp
- OAuth metadata: https://todolistmcp.com/.well-known/oauth-protected-resource
- Privacy: your lists are private to your account unless you share them. See https://todolistmcp.com for the privacy policy.

## Publisher

Published by **CLORDO LLC**.

## License

[MIT](LICENSE) © 2026 CLORDO LLC
