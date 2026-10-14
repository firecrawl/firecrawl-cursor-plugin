# Firecrawl Cursor Plugin

> Generated from Firecrawl's plugin source. Do not edit this repository by hand; changes made here are overwritten by the next sync.

Firecrawl is the context API for AI agents. This plugin connects your agent to the hosted [Firecrawl MCP server](https://docs.firecrawl.dev/mcp-server/oauth) to search the web, read pages, collect structured data, interact with live pages, and track changes.

## What's included

- **`mcp.json`**: the hosted Firecrawl MCP server at `https://mcp.firecrawl.dev/v2/mcp-oauth`
- **`skills/firecrawl`**: routes each request to the right Firecrawl tool (search, scrape, Alexandria data providers, agent, map and crawl, interact, parse, monitors, developer, paper and US government search), with a reference per operation
- **`skills/firecrawl-deep-research`**: cited, multi-source investigations, comparisons, prospect discovery and enrichment

## Setup

Install the plugin, then sign in to Firecrawl when Cursor asks (or open **Customize**, find the `firecrawl` MCP server and choose **Authenticate**). There is no API key to paste and nothing to install locally.

## Capabilities

- **Search**: web, news and image search with query-relevant excerpts, plus matching Alexandria data providers
- **Scrape**: any URL to clean Markdown, JSON with a schema, a grounded answer or verbatim highlights
- **Alexandria**: discover catalogued data providers and execute them for structured records
- **Agent**: autonomous multi-source collection into structured data
- **Map and crawl**: list a site's URLs or collect a bounded section
- **Interact**: clicks, forms and navigation in a live browser session
- **Parse**: PDFs and documents, including local files through a hosted upload
- **Monitor**: recurring checks for page changes
- **Developer, paper and US government search**: issues, merged pull requests, READMEs and docs; published papers; statutes, regulations and court opinions
