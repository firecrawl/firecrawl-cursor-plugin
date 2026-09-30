# Firecrawl Cursor Plugin

Cursor plugin that gives AI agents full web access through the [Firecrawl CLI](https://github.com/firecrawl/cli): search, scrape, map, crawl, browser interaction, AI-powered extraction, and Alexandria data providers for structured records.

## What's included

- **`skills/`** - 13 skills, synced automatically from [firecrawl/cli](https://github.com/firecrawl/cli): `firecrawl`, `firecrawl-agent`, `firecrawl-alexandria`, `firecrawl-crawl`, `firecrawl-developer-index`, `firecrawl-download`, `firecrawl-interact`, `firecrawl-map`, `firecrawl-monitor`, `firecrawl-parse`, `firecrawl-research-index`, `firecrawl-scrape`, `firecrawl-search`
- **`rules/install.mdc`** - Installation and authentication handling

## Setup

```bash
npm install -g firecrawl-cli
firecrawl login --browser
```

## Capabilities

- **Search** - Web, image, and news search with optional full-page scraping of results, plus matching Alexandria tools
- **Alexandria** - Discover catalogued data providers (official APIs, licensed publishers, Firecrawl indexes), read their contracts, and execute them for structured records instead of scraping pages
- **Scrape** - Single page content extraction to clean markdown, with JS rendering support
- **Map** - Discover all URLs on a site, with search filtering
- **Crawl** - Bulk content extraction from entire site sections
- **Interact** - Remote browser sessions for interactive pages (pagination, forms, logins)
- **Agent** - AI-powered autonomous web research and structured data extraction
- **Developer and research indexes** - Issues, merged pull requests, READMEs, docs, and published papers
- **Monitor, download, parse** - Watch pages for changes, save a site locally, parse local files
