<div align="center">

# 🔧 JieBang Tools

**Free online tools that respect your privacy.**

148+ utilities for developers, designers, and everyday users.<br>
Everything runs in your browser — your data never leaves your device.

[![Website](https://img.shields.io/badge/Website-www.jiebang.site-blue?style=flat-square)](https://www.jiebang.site)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![Tools](https://img.shields.io/badge/Tools-148+-orange?style=flat-square)](https://www.jiebang.site)

[🌐 Website](https://www.jiebang.site) · [🤖 MCP Server](https://www.jiebang.site/mcp) · [📖 API Docs](#api-endpoints)

</div>

---

## ✨ Why JieBang?

- 🆓 **100% Free** — No signup, no credit card, no hidden paywalls
- 🔒 **Privacy First** — All processing happens in your browser. Zero data uploads
- 🌙 **Dark Mode** — Built-in dark mode that follows your system preference
- ⚡ **Instant** — No installation, no loading screens. Open and use
- 📱 **Mobile Friendly** — Works great on phones and tablets
- 🌍 **Bilingual** — Full Chinese & English support

## 🛠️ Featured Tools

### Image & File
| Tool | Description |
|------|-------------|
| 🖼️ [Image Converter](https://www.jiebang.site/en/tools/image-convert.html) | Convert between PNG, JPG, WebP, BMP, GIF, HEIC |
| 📦 [Image Compressor](https://www.jiebang.site/en/tools/image-compress.html) | Batch compress images with quality control |
| 📄 [PDF Toolkit](https://www.jiebang.site/en/tools/pdf-toolkit.html) | Merge, split, compress, and convert PDFs |
| 📱 [QR Code Generator](https://www.jiebang.site/en/tools/qrcode-generator.html) | QR codes with logo, WiFi, vCard, SVG support |
| 🎨 [Color Picker](https://www.jiebang.site/en/tools/color-picker.html) | WCAG contrast checker, palette generator, eye dropper |

### Developer Tools
| Tool | Description |
|------|-------------|
| 📝 JSON/YAML Converter | Convert between JSON and YAML |
| 🗄️ SQL Formatter | Beautify and format SQL queries |
| 🔢 Base Converter | Binary, octal, decimal, hex conversions |
| 🌐 HTML Entity Encoder | Encode/decode HTML entities |
| ⏰ Cron Parser | Parse and explain cron expressions |
| 🔍 SEO Checker | Analyze webpage SEO health and meta tags |
| 📋 Meta Extractor | Extract metadata from any URL |

### Utilities
| Tool | Description |
|------|-------------|
| ⏱️ Timezone Converter | Convert time between world timezones |
| 🔐 Hash Calculator | MD5, SHA1, SHA256 hashes |
| 📊 Base64 Encoder | Encode/decode Base64 and files |
| 📅 Cron Task Manager | Create and manage scheduled tasks |

...and [130+ more tools](https://www.jiebang.site)!

## 🤖 MCP Server

JieBang also provides an [MCP (Model Context Protocol)](https://modelcontextprotocol.io/) server, allowing AI assistants like Claude, Cursor, and Windsurf to directly use these tools.

### Quick Setup

1. **Get an API key:**
   ```bash
   curl -X POST https://www.jiebang.site/api/auth/register \
     -H "Content-Type: application/json" \
     -d '{"email": "your@email.com", "password": "your-password"}'
   ```

2. **Add to your MCP client config:**
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

3. **Use it:** Ask your AI assistant to use any JieBang tool!

## 🔌 API Endpoints

All tools are available as REST APIs:

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

**Free tier:** 100 API calls/day — no credit card required.

## 🏗️ Tech Stack

- **Frontend:** Pure JavaScript, zero dependencies
- **Hosting:** Cloudflare Pages (edge computing)
- **Storage:** Cloudflare KV for API keys
- **MCP:** Streamable HTTP transport

## 🤝 Contributing

Found a bug? Have a tool idea? Contributions welcome!

1. Fork this repo
2. Create your feature branch (`git checkout -b feature/amazing-tool`)
3. Commit your changes (`git commit -m 'Add amazing tool'`)
4. Push to the branch (`git push origin feature/amazing-tool`)
5. Open a Pull Request

## 📄 License

[MIT](LICENSE) — Free to use, modify, and distribute.

---

<div align="center">

**[⭐ Star this repo](https://github.com/jiebang-tools/tools) if you find it useful!**

Made with ❤️ by [JieBang](https://www.jiebang.site)

</div>
