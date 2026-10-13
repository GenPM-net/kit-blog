# @core/kit-blog

[![genpm](https://api.genpm.net/v1/badge/@core/kit-blog.svg)](https://genpm.net/p/@core/kit-blog) ![license](https://img.shields.io/badge/license-MIT-blue)

> Blog kit for Next.js: posts with authors, categories, tags, series, feeds, moderated comments and newsletter

A [GenPM](https://genpm.net) module: **source code + AI rules + MCP config**, injected into your project instead of hidden in `node_modules`. The code lands in `src/app/(blog)`, pinned to a verified commit, and you own it.

## Install

```bash
genpm add @core/kit-blog
```

No genpm yet? `curl -fsSL https://genpm.net/install.sh | sh` (macOS/Linux), `irm https://genpm.net/install.ps1 | iex` (Windows), or one-off with `npx @genpm-net/cli add @core/kit-blog`.

Or let your AI agent do it: run `genpm mcp setup` once, then ask *"add @core/kit-blog with genpm"* in Claude Code, Cursor, VS Code, Windsurf, Codex or Gemini CLI. It shows you a dry-run plan before writing anything.

## What it does

A complete blog on top of @core/kit-cms, edited in the same `/admin`: posts with rich text and cover images, author
profiles, categories, tags and series, scheduling, RSS/Atom/JSON feeds, site search, moderated comments, newsletter
with double opt-in and one-click unsubscribe, share links without third-party scripts and full SEO (BlogPosting
JSON-LD, sitemap, Open Graph). Glue and templates only: logic lives in @core/blog, comments and newsletter.

## At a glance

- **GenPM dependencies** (installed with it): [@core/kit-cms](https://genpm.net/p/@core/kit-cms), [@core/blog](https://genpm.net/p/@core/blog), [@core/comments](https://genpm.net/p/@core/comments), [@core/newsletter](https://genpm.net/p/@core/newsletter)
- **npm dependencies** (proposed, never installed without asking): `next`, `react`, `zod`
- **Environment variables** (added to `.env.example`): `NEWSLETTER_FROM`, `NEWSLETTER_POSTAL_ADDRESS`, `NEWSLETTER_SECRET`
- **AI rules**: [`AGENTS.md`](AGENTS.md), loaded by your agent only when it works in `src/app/(blog)`

## Security

GenPM installs a 40-character commit SHA (never a branch), verifies an Ed25519-signed manifest, never runs install scripts and scans AI rules for prompt injection. Details: [genpm.net/docs/security](https://genpm.net/docs/security).

## License

MIT — see [LICENSE](LICENSE). Browse the full catalog at [genpm.net](https://genpm.net).
