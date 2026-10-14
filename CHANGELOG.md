# Changelog

## 0.4.0

This release moves the plugin from the Firecrawl CLI to the hosted Firecrawl MCP server.

- **Hosted MCP with browser sign-in.** The plugin connects to `https://mcp.firecrawl.dev/v2/mcp-oauth`. The first Firecrawl call asks you to sign in once in your browser. There is no API key to paste and nothing to install locally.
- **New skills.** `firecrawl` routes each request to the right tool, and `firecrawl-deep-research` runs cited, multi-source investigations. They replace the CLI skills and the CLI install rule.
- **CLI skills moved.** If you use the Firecrawl CLI, install its skills separately with `npx skills add firecrawl/cli`. The CLI itself keeps working.
- **Downloading a whole site** to local files has no direct replacement. Use map and crawl to collect a site's pages.
- **Local files** such as PDFs and documents are parsed through a hosted upload.
