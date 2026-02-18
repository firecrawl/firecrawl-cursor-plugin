# Firecrawl Cursor Plugin

Cursor plugin that gives AI agents full web access through the [Firecrawl CLI](https://github.com/mendableai/firecrawl-cli): search, scrape, map, crawl, browser automation, and AI-powered extraction.

## What's included

- **`skills/firecrawl/SKILL.md`** - Complete CLI reference covering search, scrape, map, crawl, browser, and agent commands with workflow patterns and examples
- **`rules/install.mdc`** - Installation and authentication handling

## Setup

```bash
npm install -g firecrawl-cli
firecrawl login --browser
```

## Capabilities

- **Search** - Web, image, and news search with optional full-page scraping of results
- **Scrape** - Single page content extraction to clean markdown, with JS rendering support
- **Map** - Discover all URLs on a site, with search filtering
- **Crawl** - Bulk content extraction from entire site sections
- **Browser** - Remote Chromium sessions for interactive pages (pagination, forms, modals)
- **Agent** - AI-powered autonomous web research and structured data extraction
