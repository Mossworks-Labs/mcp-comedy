# mcp-comedy

MCP server for comedy writing — humor theory, techniques, and comedian knowledge.

Part of the [CRAFT](https://github.com/Mossworks-Labs/craft) content studio.

## Tools

| Tool | Description |
|------|-------------|
| `comedy_theory` | Humor psychology and why things are funny |
| `comedy_history` | Historical evolution of comedy genres |
| `famous_comedians` | Styles and techniques of notable comedians |
| `comedy_techniques` | Practical comedy writing methods |

## Usage

### Stdio (Claude Code / local)

```json
{
  "mcpServers": {
    "comedy": {
      "command": "node",
      "args": ["dist/index.js"]
    }
  }
}
```

### HTTP (Docker / Kubernetes)

```bash
docker build -t mcp-comedy .
docker run -p 8080:8080 -e MCP_TRANSPORT=http mcp-comedy
```

## Development

```bash
npm install
npm run build
node dist/index.js
```

Requires Node.js 22+.
