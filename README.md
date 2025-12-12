# toMCP

**Turn any website into an MCP server.**

Convert any website URL into an MCP (Model Context Protocol) server config for your AI tools.

## Usage

Simply add `tomcp.org/` before any URL:

```
tomcp.org/docs.stripe.com
tomcp.org/react.dev
tomcp.org/your-docs.com/api
```

## Supported AI Tools

- **Cursor** - `~/.cursor/mcp.json`
- **Claude Desktop** - `~/.claude/claude_desktop_config.json`
- **Windsurf** - `~/.codeium/windsurf/mcp_config.json`
- **VS Code** - `.vscode/mcp.json`
- **Cline** - `~/.cline/mcp_settings.json`

## How It Works

1. Visit [tomcp.org](https://tomcp.org)
2. Enter any website URL
3. Select your AI tool
4. Copy the generated MCP config
5. Add it to your tool's config file
6. Restart your AI tool

## Example Config

```json
{
  "mcpServers": {
    "docs-stripe-com": {
      "url": "https://tomcp.org/docs.stripe.com"
    }
  }
}
```

## Tech Stack

- **Frontend**: Vanilla HTML/CSS/JS with Tailwind CSS
- **Backend**: Cloudflare Workers
- **AI**: Cloudflare Workers AI (Llama 3.1)

## Features

- Works with any public URL
- No setup required - just paste the config
- Free forever - powered by Cloudflare Workers
- Chat with any website using AI

## License

MIT
