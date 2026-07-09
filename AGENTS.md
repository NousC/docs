# Documentation project instructions

> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

## About this project

- This is the public documentation for **Nous**, published at [docs.opennous.cloud](https://docs.opennous.cloud).
- **Nous is the context graph for GTM agents.** It resolves every person, conversation, and touchpoint across the GTM tool stack (Apollo, HubSpot, Smartlead, Gmail, LinkedIn) into one account record, returned to an agent in a single MCP call.
- Built on [Mintlify](https://mintlify.com). Pages are MDX with YAML frontmatter; configuration lives in `docs.json`.
- Run `mint dev` to preview locally; `mint broken-links` to check links.

## Positioning, use this language

Locked positioning (updated June 18 2026). Match it in any new or edited page.

- **What Nous is.** "the context graph for agentic GTM." The headline noun is "context graph." The one-liner is "a unified GTM API that replaces the scattered data across your GTM tools with a single context graph for AI agents." Never "customer graph," "GTM data infrastructure," "context layer," "platform," or "CRM."
- **The triplet.** Whenever copy lists what's inside the graph, use the exact triplet "person, conversation, and touchpoint." It is concrete and scannable.
- **The verb.** Nous makes your GTM stack **visible** to agents. Lean on "visible," "in one place," "act on." Avoid abstract verbs like "unify" in headline copy.
- **What it ships.** The **account record**, one identity-resolved record of an account, every tool unified, returned in a single MCP call. "Account record" is the product noun underneath the context graph.
- **Audience.** GTM agents and the people who build them, GTM engineers, outbound agencies. Agent-agnostic. Nous is reached over MCP and REST by *any* agent. Do not narrow to "Claude agents."
- **Scope.** GTM only. Nous resolves and serves GTM account data. It does not scrape, acquire leads, write copy, or send. Don't document it as if it does.
- **Open by default.** AGPL v3, self-host free forever; a hosted tier (Nous Cloud) for those who skip setup.

## Do not say

- ❌ "GTM data infrastructure for agents," retired positioning.
- ❌ "Customer graph for GTM agents," retired headline noun (replaced by "context graph" June 18 2026).
- ❌ "The context layer GTM agents run on," retired positioning (replaced May 28 2026).
- ❌ "Drop-in context infrastructure," retired marketing-site sub-line.
- ❌ "The Mind," "evidence substrate," "observation spine," "claim derivation." The internal mechanism is never named as a marketed capability. You **may** state the concrete outcome the manifesto markets. The graph self-heals as new signals arrive, and the ICP model sharpens from your own won and lost deals. Do not dress that up as a vague "self-learning loop" or "it gets smarter."
- ❌ "one record per human / per person" as the headline unit. The headline noun is the **context graph**; the product noun is the **account record**. Person-level identity resolution is the *mechanism*, and may be described as such on technical (architecture / API / MCP) pages.
- ❌ "Personalization touchpoint" as marketing copy. Use "touchpoint" alone.
- ❌ Narrowing to a single agent vendor ("built for Claude").

## Terminology

- **context graph** — the headline noun for the product
- **account record** — the unit Nous returns; the product noun underneath the context graph
- **identity resolution** — the mechanism that merges a person's data across tools
- **contact** — an individual person record (accurate usage on API / MCP / architecture pages)
- **account** / **company** — the company-level rollup (`get_company`)
- **MCP call** — the primary interface; **REST API** — the alternative
- Use "workspace" not "project"; "provider" or "integration"; and "MCP connector" only for the MCP server

## Style preferences

- Active voice and second person ("you")
- One idea per sentence; keep sentences concise
- Sentence case for headings
- Bold for UI elements. Click **Settings**
- Code formatting for file names, commands, paths, and code references
- **No em-dashes.** Use periods or restructure.
- **No colons** in customer-facing prose. Use periods or restructure.
- **No "X not Y" framing.** State what Nous is, never what it isn't.

## Content boundaries

- Document what is built and shipping. If a capability is roadmap, do not document it as present.
- Document scoring as a concrete surface. An ICP fit score and intent an endpoint returns, a model trained on your own won and lost deals. Do not narrate the internal learning mechanism or imply autonomous intelligence.
- Do not document lead scraping, copywriting, or sending. Out of scope by design.
