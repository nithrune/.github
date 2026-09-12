<h1 align="center">Nithrune</h1>

<p align="center"><em>Minecraft content — plugins, mods, mobpacks, resource packs.</em></p>

---

Old Norse **_niðr_** means *downward*. It shares a root with English
*nether*. A **rune** is a mark cut into a surface to make it mean something.

Nithrune cuts the marks that live below.

## What this is

Everything here is for **Minecraft** — server-side and client-side, code
and content. Nothing else lives in this organisation.

## Language

Everything written to communicate here is **English** — issues, pull
requests, commit messages, documentation and code comments.

What language a repository's own content speaks is that repository's
business, not the organisation's. Its README says so.

## Repository structure

Every repository is named after what it holds:

| Prefix | Contents |
|---|---|
| `mobpack-*` | Content packs — mobs, bosses, items, progression |
| `plugin-*` | Server plugins |
| `mod-*` | Client and server mods |
| `rp-*` | Resource and texture packs |
| `tool-*` | Build, generation and test tooling |
| `web-*` | The website and the project wikis it publishes |

Each repository documents itself: what it targets, what it needs to run,
and how to install it live in its own `README.md` and `INSTALL.md`.

Longer documentation lives on the web instead: each project gets its own
subdomain, and everything about that project is a page under it.

## Licensing

There is no org-wide licence: GitHub cannot inherit one, and code and
artwork want different terms. Each repository carries its own, and the
split is explained in
[CONTRIBUTING.md](https://github.com/nithrune/.github/blob/main/CONTRIBUTING.md).

The Nithrune name and marks are excluded from all of them.

`web-*` is the one exception. Those repositories carry an all-rights-reserved
licence: reading the website and the wikis is permitted, copying, modifying or
republishing any part of them is not. Ask by opening an issue.

## Reporting something

Security issues go through **private vulnerability reporting** on the
affected repository's Security tab — never a public issue. Everything
else: open an issue on the repository it concerns.
