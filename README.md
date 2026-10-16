<p align="center"><img src="assets/logo.svg" width="72" alt="ToDo List MCP logo"></p>

# ToDo List MCP

[ToDo List MCP](https://todolistmcp.com) is an AI-forward list and notes service built for agents and the humans they look after. Any MCP-capable agent or chat app (Grok, Grok Bot, Cursor, Claude, ChatGPT, VS Code, and others) can create lists, add and complete items, set due dates and tags, and share lists, and you see the same lists in the web app.

This repo is the public connector config. It contains no server code and no API keys: it points at the hosted server `https://todolistmcp.com/mcp`, and sign-in is handled with OAuth.

## Connect

**Any MCP client:** add a remote (Streamable HTTP) MCP server with this URL:

```
https://todolistmcp.com/mcp
```

Most clients accept a config like this:

```json
{
  "mcpServers": {
    "todolist": { "type": "http", "url": "https://todolistmcp.com/mcp" }
  }
}
```

**Grok and Grok Bot:** install **ToDo List MCP** from the marketplace.

**Cursor:** install **ToDo List MCP** from the Cursor Marketplace, or test locally:

```bash
git clone https://github.com/clordo/todolistmcp-plugin ~/.cursor/plugins/local/todolist-mcp
```

## Sign in

The first time your agent calls a ToDo List MCP tool, your client opens todolistmcp.com in your browser. Sign in with **Google** or with a **one-time email code**, approve access, and you're done. Tokens are scoped (`lists:read`, `lists:write`, `lists:share`) and can be revoked from your account on todolistmcp.com.

## Configuration

None. There are no variables or keys to set.

## Example prompts

- "Make a packing list for a 5-day beach trip and add it to ToDo List MCP."
- "What's overdue on my lists this week?"
- "Mark 'book flights' done on my Jamaica list and add 'renew passport' due Friday."
- "Turn the TODOs in this file into items on a new list called 'Refactor'."
- "Share my grocery list with sam@example.com."

## Support

- Issues and feature requests: https://github.com/clordo/todolistmcp-plugin/issues
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
