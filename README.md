# Firecrawl for Cursor

Turn any website into clean, LLM-ready markdown or structured data — directly in Cursor.

This plugin gives Cursor's agent full web access through the [Firecrawl CLI](https://github.com/firecrawl/cli): search, scrape, crawl, map, interact, monitor, and AI-powered extraction. Every operation includes JavaScript rendering, anti-bot handling, and proxy rotation.

## Install

### 1. Add the plugin

In Cursor (2.5+), run **`/add-plugin`** and choose **firecrawl**, or browse the [Cursor Marketplace](https://cursor.com/marketplace).

### 2. Install the Firecrawl CLI

The plugin's skills call the Firecrawl CLI, so install it globally:

```bash
npm install -g firecrawl-cli
```

### 3. Sign in

```bash
firecrawl login --browser
```

Prefer not to use the browser? Authenticate with a key instead:

```bash
firecrawl login --api-key "fc-YOUR-API-KEY"
# or persist it as an environment variable
export FIRECRAWL_API_KEY=fc-YOUR-API-KEY
```

Get a free API key at [firecrawl.dev/app/api-keys](https://firecrawl.dev/app/api-keys). Verify everything's ready with `firecrawl --status`.

## Capabilities

Once installed, Cursor uses Firecrawl automatically for web tasks:

- **Search** — web, news, and image search, with optional full-page scraping
- **Scrape** — clean markdown (or structured JSON) from any page, with JS rendering
- **Map** — discover every URL on a site
- **Crawl** — bulk-extract whole site sections
- **Interact** — click, fill forms, paginate, and log in on live pages
- **Agent** — AI-powered autonomous research and structured extraction
- **Monitor** — watch pages for meaningful changes, with webhook/email alerts
- **Parse** — convert local files (PDF, DOCX, XLSX, …) to markdown
- **Download** — save an entire site to local files

## Usage

Just ask Cursor naturally:

```
Search for "best practices for React testing" and summarize the key recommendations
Scrape https://docs.firecrawl.dev/introduction and pull out the main concepts
Map all the URLs under https://firecrawl.dev/blog
Monitor https://news.ycombinator.com and alert me when an AI story hits the top 10
```

## What's included

- **`skills/`** — 10 agent skills covering search, scrape, map, crawl, interact, agent, monitor, parse, download, plus a CLI workflow guide
- **`rules/install.mdc`** — sets up the Firecrawl CLI and handles authentication automatically

## Command reference

The skills cover the full command set. For every command and flag, see the [Firecrawl CLI docs](https://docs.firecrawl.dev/cli).

## Configuration

| Variable | Description |
|---|---|
| `FIRECRAWL_API_KEY` | Your API key (alternative to `firecrawl login`) |
| `FIRECRAWL_API_URL` | Custom endpoint for self-hosted instances |
| `FIRECRAWL_NO_TELEMETRY` | Set to `1` to disable anonymous CLI telemetry |

**Self-hosted:** point the CLI at your instance with `export FIRECRAWL_API_URL=https://your-instance.com` (custom URLs skip API-key auth).

## Resources

- [Firecrawl CLI docs](https://docs.firecrawl.dev/cli)
- [Firecrawl CLI repository](https://github.com/firecrawl/cli)
- [API reference](https://docs.firecrawl.dev/api-reference)
- [Get an API key](https://firecrawl.dev/app/api-keys)

## License

MIT

## Support

- [Firecrawl Discord](https://discord.gg/gSmWdAkdwd)
- [GitHub Issues](https://github.com/firecrawl/firecrawl-cursor-plugin/issues)
- hello@firecrawl.dev
