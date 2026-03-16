# Genealogy-MCP

> Genealogy-MCP is a community-driven open source project building the connective
> tissue between AI and family history for everyone. We welcome every contributor,
> prioritize free and open platforms, and believe no one should need a subscription
> to explore their own past.

---

## What We Build

We develop [Model Context Protocol](https://modelcontextprotocol.io/) (MCP) servers
that connect AI assistants to genealogy platforms. Each server exposes a set of tools
that let any MCP-compatible client search records, browse family trees, and work with
historical data -- no custom integration required.

| Repo | Platform | Tier | Tools | Status |
|---|---|---|---|---|
| [gramps-mcp](https://github.com/Genealogy-MCP/gramps-mcp) | Gramps Web (self-hosted) | Platinum | 19 | v1.1.0 |
| [wikitree-mcp](https://github.com/Genealogy-MCP/wikitree-mcp) | WikiTree | Gold | 10 | v0.1.0 |
| [gedcom-mcp](https://github.com/Genealogy-MCP/gedcom-mcp) | Local GEDCOM files | Bronze | 7 | v0.1.0 |

**36 tools** across three platforms, with more on the way.

---

## Our Values

1. **Open by default.** Code, protocols, and governance are public. AGPL-3.0, no exceptions.
2. **Your data stays yours.** We never aggregate, store, or broker genealogy data. Privacy is architecture, not policy.
3. **Community over heroics.** The project succeeds when no single person is essential. We build for contributors, not just users.
4. **Free platforms first.** We integrate with everything, but steer people toward tools that are free, open source, or publicly accessible.
5. **Quality earns trust.** Every tool ships with tests, documentation, and clear error messages. Reliability is how open source proves itself.

## What We Are NOT

- **Not a SaaS.** No hosting, no subscriptions, no premium tier.
- **Not a data aggregator.** We connect to platforms; we never copy or store your family data.
- **Not vendor-locked.** Any MCP-compatible AI client works equally.
- **Not a walled garden.** Scope is defined by the community, not controlled by one person.

---

## Get Involved

Whether you are a developer, a genealogist, or both -- there is room for you here.

- **Use the servers.** Pick a repo, follow the setup instructions, and connect it to your favourite AI assistant.
- **Report issues.** Found a bug or have a feature idea? Open an issue on the relevant repo.
- **Contribute code.** Every repo has a `CONTRIBUTING.md` and a `Makefile` with standard targets (`make install`, `make test`, `make lint`). PRs are welcome.
- **Suggest a platform.** Know a genealogy service that should have an MCP server? Start a discussion.

We are building the kind of project where any contributor can understand the full stack, ship a feature end-to-end, and see it used by real people researching their families.

---

## Shared Stack

All servers share: Python 3.10+ | FastMCP | Pydantic | pytest (>= 80% branch coverage) | ruff | pyright

Licensed under [AGPL-3.0-only](https://www.gnu.org/licenses/agpl-3.0.html).
