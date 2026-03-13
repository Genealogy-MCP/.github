# Genealogy MCP

A growing collection of [Model Context Protocol](https://modelcontextprotocol.io/) servers that bring genealogy platforms into AI assistants.

## Servers

| Server | Platform | Tools | Auth | Writes | Transport |
|---|---|---|---|---|---|
| [gramps-mcp](https://github.com/Genealogy-MCP/gramps-mcp) | Gramps Web API | 19 | JWT Bearer | Yes | stdio, HTTP |
| [familysearch-mcp](https://github.com/Genealogy-MCP/familysearch-mcp) | FamilySearch API | 9 | Browser | No | stdio, HTTP |
| [wikitree-mcp](https://github.com/Genealogy-MCP/wikitree-mcp) | WikiTree API | 10 | None | No | stdio, HTTP |

## Quick Start

Add any server to your MCP client configuration:

```json
{
  "mcpServers": {
    "gramps": {
      "command": "docker",
      "args": [
        "run", "-i", "--rm",
        "-e", "GRAMPS_API_URL=http://localhost:5555/api",
        "-e", "GRAMPS_TOKEN=your-jwt-token",
        "ghcr.io/genealogy-mcp/gramps-mcp:latest"
      ]
    }
  }
}
```

Each server also supports streamable HTTP transport on port 8000 — see individual repo READMEs for full configuration options.

## Shared Stack

All servers are built with Python, [FastMCP](https://github.com/jlowin/fastmcp), and `httpx`. Package management via `uv`. Docker images published to [GitHub Container Registry](https://github.com/orgs/Genealogy-MCP/packages).

## License

All servers are licensed under [AGPL-3.0-only](https://www.gnu.org/licenses/agpl-3.0.html).
