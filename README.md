# JieBang Tools - MCP Server

A Model Context Protocol (MCP) Server providing 20+ online developer utilities, accessible via Streamable HTTP transport.

## What is MCP?

The [Model Context Protocol (MCP)](https://modelcontextprotocol.io/) is an open standard that enables AI models to securely interact with external tools and data sources. This project implements an MCP Server that exposes JieBang's developer tools as MCP tools, allowing any MCP-compatible AI client (Claude, Cursor, Windsurf, etc.) to directly use these utilities.

## MCP Server Info

| Field | Value |
|-------|-------|
| **Server Name** | JieBang Tools |
| **Version** | 1.7.0 |
| **Transport** | Streamable HTTP |
| **Endpoint** | `https://www.jiebang.site/mcp` |
| **Authentication** | API Key (Bearer token) |

## Available MCP Tools

### Data Format
| Tool | Description |
|------|-------------|
| `json-yaml` | Convert between JSON and YAML formats |
| `sql-format` | Format and beautify SQL queries |
| `base-convert` | Convert numbers between different bases (binary, octal, decimal, hex) |
| `html-entity` | Encode/decode HTML entities |
| `cron-parse` | Parse and explain cron expressions |

### SEO & Web
| Tool | Description |
|------|-------------|
| `seo-check` | Analyze webpage SEO health and meta tags |
| `meta-extract` | Extract metadata (title, description, OG tags) from any URL |

### Image & File
| Tool | Description |
|------|-------------|
| `qrcode` | Generate QR codes from text or URLs |
| `image-convert` | Convert images between formats (PNG, JPG, WebP, BMP, GIF) |
| `file-process` | Calculate file hashes (MD5, SHA1, SHA256) and encode/decode Base64 |

### Time & Timezone
| Tool | Description |
|------|-------------|
| `timezone-convert` | Convert time between any world timezones |

### Task Automation
| Tool | Description |
|------|-------------|
| `cron-task` | Create and manage scheduled/cron tasks |

## Quick Start

### 1. Register for an API Key

```bash
curl -X POST https://www.jiebang.site/api/auth/register \
  -H "Content-Type: application/json" \
  -d '{"email": "your@email.com", "password": "your-password"}'
```

Response:
```json
{
  "api_key": "jb_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
}
```

### 2. Configure Your MCP Client

Add to your MCP client configuration (e.g., Claude Desktop, Cursor, Windsurf):

```json
{
  "mcpServers": {
    "jiebang-tools": {
      "url": "https://www.jiebang.site/mcp",
      "headers": {
        "Authorization": "Bearer jb_your_api_key_here"
      }
    }
  }
}
```

### 3. Use the Tools

Once configured, your AI assistant can directly call any of the 20+ tools. For example:

- "Convert this JSON to YAML" → calls `json-yaml`
- "Generate a QR code for https://example.com" → calls `qrcode`
- "Check the SEO of example.com" → calls `seo-check`
- "What does the cron expression `0 9 * * 1-5` mean?" → calls `cron-parse`

## API Endpoints

All tools are also available as REST API endpoints:

```
POST /api/json-yaml
POST /api/sql-format
POST /api/base-convert
POST /api/html-entity
POST /api/cron-parse
POST /api/seo-check
POST /api/meta-extract
POST /api/qrcode
POST /api/image-convert
POST /api/file-process
POST /api/timezone-convert
POST /api/cron-task
```

Authentication: Include `Authorization: Bearer <your-api-key>` in request headers.

## Free Tier

- **100 API calls/day** — No credit card required
- Register at [jiebang.site](https://www.jiebang.site) to get started

## Web Interface

Prefer a browser? All tools are also available at [www.jiebang.site](https://www.jiebang.site) with a user-friendly web interface — no coding required.

## Tech Stack

- Pure JavaScript, zero dependencies
- Cloudflare Pages + Functions (edge computing)
- Cloudflare KV for API key storage

## License

[MIT](LICENSE)

## Links

- 🌐 Website: [https://www.jiebang.site](https://www.jiebang.site)
- 📦 MCP Registry: [site.jiebang.www/tools](https://www.jiebang.site/mcp)
- 📖 Smithery: [JieBang Tools on Smithery](https://smithery.ai/server/https://www.jiebang.site/mcp)
