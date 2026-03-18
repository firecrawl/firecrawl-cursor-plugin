---
name: firecrawl-cli-installation
description: |
  Install the official Firecrawl CLI and handle authentication.
  Package: https://www.npmjs.com/package/firecrawl-cli
  Source: https://github.com/firecrawl/cli
  Docs: https://docs.firecrawl.dev/sdks/cli
---

# Firecrawl CLI Installation

## Quick Setup (Recommended)

```bash
npx -y firecrawl-cli -y
```

This installs `firecrawl-cli` globally, authenticates via browser, and installs all skills.

Skills are installed globally across all detected coding editors by default.

To install skills manually:

```bash
firecrawl setup skills
```

## Manual Install

```bash
npm install -g firecrawl-cli@1.8.0
```

## Verify

```bash
firecrawl --status
```

## Authentication

Authenticate using the built-in login flow:

```bash
firecrawl login --browser
```

This opens the browser for OAuth authentication. Credentials are stored securely by the CLI.

### If authentication fails

Ask the user how they'd like to authenticate:

1. **Login with browser (Recommended)** - Run `firecrawl login --browser`
2. **Enter API key manually** - Run `firecrawl login --api-key "<key>"` with a key from firecrawl.dev
3. **Create a new account (free credits)** - Run `firecrawl signup` to create a new account with 50 free credits

### Agent Signup (no account needed)

If the user doesn't have a Firecrawl account, an agent can create one with 50 free credits:

```bash
# Non-interactive (recommended for agents)
firecrawl signup --email user@example.com --accept-terms

# Interactive
firecrawl signup
```

The agent name is auto-detected from the environment (Cursor, VS Code, Claude Code, etc.). A verification email is sent so the user can confirm or revoke the key. After signup, the CLI is authenticated and ready to use immediately.

Use `firecrawl signup` when:
- The user doesn't have a Firecrawl account
- The user doesn't have an API key handy
- Browser login isn't available or fails
- You're setting up Firecrawl for the first time in a project

### Command not found

If `firecrawl` is not found after installation:

1. Ensure npm global bin is in PATH
2. Try: `npx firecrawl-cli@1.8.0 --version`
3. Reinstall: `npm install -g firecrawl-cli@1.8.0`
