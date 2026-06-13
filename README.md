<div align="center">

# 🔧 JieBang Tools

**Free online tools that respect your privacy.**

150+ utilities for developers, designers, and everyday users.

[🌐 Live Site](https://www.jiebang.site) · [📖 API Docs](https://www.jiebang.site/api-docs) · [🐛 Report Bug](https://github.com/jiebang-tools/tools/issues) · [✨ Request Feature](https://github.com/jiebang-tools/tools/issues)

</div>

---

## Why JieBang?

Most online tools require sign-up, upload your files to servers, or bombard you with ads. JieBang is different:

- **100% Client-Side** — Your files never leave your browser. Period.
- **No Sign-Up** — Open and use. No accounts, no cookies, no tracking.
- **No Server Processing** — Everything runs in your browser using JavaScript.
- **Free & Open Source** — MIT licensed. Fork it, self-host it, modify it.
- **Dark Mode** — Easy on the eyes, always.
- **Mobile Friendly** — Works on any device with a modern browser.

## Featured Tools

### Developer Tools
| Tool | Description |
|------|-------------|
| [JSON Formatter](https://www.jiebang.site/tools/json-formatter) | Format, validate, and minify JSON with syntax highlighting |
| [Base64 Encoder](https://www.jiebang.site/tools/base64) | Encode/decode Base64 for text and files |
| [URL Encoder](https://www.jiebang.site/tools/url-encoder) | Encode/decode URLs and query parameters |
| [JWT Decoder](https://www.jiebang.site/tools/jwt-decoder) | Decode and inspect JWT tokens instantly |
| [Cron Expression Generator](https://www.jiebang.site/tools/cron-generator) | Build and understand cron expressions visually |
| [Regex Tester](https://www.jiebang.site/tools/regex-tester) | Test regular expressions with real-time matching |
| [Hash Generator](https://www.jiebang.site/tools/hash-generator) | Generate MD5, SHA-1, SHA-256, SHA-512 hashes |
| [Markdown Preview](https://www.jiebang.site/tools/markdown-preview) | Write and preview Markdown with live rendering |

### Image Tools
| Tool | Description |
|------|-------------|
| [Image Converter](https://www.jiebang.site/tools/image-convert) | Convert between HEIC, PNG, JPG, WebP, BMP, GIF — no upload needed |
| [Image Compressor](https://www.jiebang.site/tools/image-compress) | Compress images with adjustable quality, batch support |
| [QR Code Generator](https://www.jiebang.site/tools/qrcode-generator) | Generate QR codes with logos, WiFi, vCard, SVG export |
| [Color Picker](https://www.jiebang.site/tools/color-picker) | Pick colors from screen, WCAG contrast checker, palette export |
| [Watermark Remover](https://www.jiebang.site/tools/watermark-remover) | Remove image/video watermarks with preset positions |

### Document Tools
| Tool | Description |
|------|-------------|
| [PDF Toolkit](https://www.jiebang.site/tools/pdf-toolkit) | Merge, split, rotate, add watermark — all in browser |
| [YAML/JSON Converter](https://www.jiebang.site/tools/yaml-json) | Convert between YAML and JSON formats |

### SEO & Web Tools
| Tool | Description |
|------|-------------|
| [SEO Analyzer](https://www.jiebang.site/tools/seo-analyzer) | Check meta tags, headings, and SEO health |
| [Sitemap Generator](https://www.jiebang.site/tools/sitemap-generator) | Generate XML sitemaps from URLs |

**[View all 150+ tools →](https://www.jiebang.site)**

## Tech Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (no framework bloat)
- **Styling**: Custom CSS with dark mode support
- **Hosting**: Cloudflare Pages (global CDN, edge caching)
- **API**: RESTful API with free tier (100 requests/day)
- **MCP**: Model Context Protocol server for AI assistant integration

## Quick Start

### Use Online
Visit [www.jiebang.site](https://www.jiebang.site) — no installation needed.

### Self-Host
```bash
# Clone the repository
git clone https://github.com/jiebang-tools/tools.git
cd tools

# Serve locally (any static file server works)
python3 -m http.server 8080
# Or use Node.js
npx serve .
```

Open `http://localhost:8080` in your browser.

### API Access
```bash
# Free tier: 100 requests/day
curl "https://www.jiebang.site/api/qrcode?text=Hello&size=200"

# Pro tier: 5,000 requests/day for $1.99/month
curl -H "Authorization: Bearer YOUR_API_KEY" \
     "https://www.jiebang.site/api/qrcode?text=Hello&size=200"
```

See [API Documentation](https://www.jiebang.site/api-docs) for all endpoints.

### MCP Integration
JieBang provides an MCP server for AI assistants:

```bash
# Add to your MCP client config
{
  "mcpServers": {
    "jiebang": {
      "url": "https://www.jiebang.site/mcp"
    }
  }
}
```

## Project Structure

```
├── index.html              # Homepage (Chinese)
├── en/                     # English version
├── tools/                  # Chinese tool pages
│   ├── json-formatter.html
│   ├── image-convert.html
│   ├── pdf-toolkit.html
│   └── ...
├── en/tools/               # English tool pages
├── css/
│   └── style.css           # Global styles
├── js/
│   └── common.js           # Shared utilities
├── api/                    # API serverless functions
├── functions/              # Cloudflare Pages Functions
├── _headers                # CDN cache rules
├── _redirects              # URL redirects
└── sitemap.xml             # SEO sitemap
```

## Contributing

Contributions are welcome! Here's how you can help:

1. **Report bugs** — [Open an issue](https://github.com/jiebang-tools/tools/issues)
2. **Suggest tools** — [Request a feature](https://github.com/jiebang-tools/tools/issues)
3. **Submit code** — Fork, create a branch, and open a Pull Request
4. **Improve docs** — Fix typos, add examples, translate content

## Privacy Policy

JieBang processes everything in your browser. We do not:
- Upload your files to any server
- Store your data after you close the tab
- Track you with cookies or analytics identifiers
- Share any information with third parties

The only server interaction is serving static files and (optionally) API requests.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## Links

- 🌐 Website: [www.jiebang.site](https://www.jiebang.site)
- 📖 API Docs: [www.jiebang.site/api-docs](https://www.jiebang.site/api-docs)
- 🤖 MCP Server: [www.jiebang.site/mcp](https://www.jiebang.site/mcp)
- 💬 Feedback: [GitHub Issues](https://github.com/jiebang-tools/tools/issues)

---

<div align="center">

**Built with ❤️ by [JieBang](https://www.jiebang.site)**

If you find this useful, consider giving us a ⭐ star!

</div>
