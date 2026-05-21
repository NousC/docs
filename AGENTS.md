# Documentation project instructions

> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

## About this project

- This is the public documentation for **Nous**, published at [docs.opennous.cloud](https://docs.opennous.cloud).
- **Nous is the context layer GTM agents run on.** It unifies a GTM stack — Apollo, Salesforce, Smartlead, Gmail, LinkedIn — into one identity-resolved account record, returned to an agent in a single MCP call.
- Built on [Mintlify](https://mintlify.com). Pages are MDX with YAML frontmatter; configuration lives in `docs.json`.
- Run `mint dev` to preview locally; `mint broken-links` to check links.

## Positioning — use this language

Locked positioning (Nous Founding Charter, May 21 2026). Match it in any new or edited page.

- **What Nous is:** "the context layer GTM agents run on." Never "GTM data infrastructure," "a platform," or "a CRM."
- **What it ships:** the **account record** — one identity-resolved record of an account, every tool unified, returned in a single MCP call. "Account record" is the product noun.
- **Audience:** GTM agents and the people who build them — GTM engineers, outbound agencies. Agent-agnostic: Nous is reached over MCP and REST by *any* agent. Do not narrow to "Claude agents."
- **Scope:** GTM only. Nous unifies, resolves, and serves GTM account data. It does not scrape, acquire leads, write copy, or send. Don't document it as if it does.
- **Open by default:** AGPL v3, self-host free forever; a hosted tier (Nous Cloud) for those who skip setup.

## Do not say

- ❌ "GTM data infrastructure for agents" — retired positioning.
- ❌ "The Mind," "a self-learning loop," "it gets smarter" — the learning loop is not a marketed capability. Document what the product does today: unify, resolve, sync, serve.
- ❌ "one record per human / per person" as the headline unit — the headline unit is the **account record**. Person-level identity resolution is the *mechanism*, and may be described as such on technical (architecture / API / MCP) pages.
- ❌ Narrowing to a single agent vendor ("built for Claude").

## Terminology

- **account record** — the product; the unit Nous returns
- **identity resolution** — the mechanism that merges a person's data across tools
- **contact** — an individual person record (accurate usage on API / MCP / architecture pages)
- **account** / **company** — the company-level rollup (`get_company`)
- **MCP call** — the primary interface; **REST API** — the alternative
- Use "workspace" not "project"; "provider" or "integration", and "MCP connector" only for the MCP server

## Style preferences

- Active voice and second person ("you")
- One idea per sentence; keep sentences concise
- Sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document what is built and shipping. If a capability is roadmap, do not document it as present.
- Do not document the internal scoring / learning loop as a user-facing feature.
- Do not document lead scraping, copywriting, or sending — out of scope by design.
