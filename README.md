# org-repo

Organisation-wide defaults for **Nithrune**.

GitHub reads this repository to supply files that individual Nithrune
repositories do not define themselves. Nothing here is a library, a
plugin, or a mobpack — it is paperwork.

> GitHub requires this repository to carry the literal name `.github`,
> which describes nothing. Everywhere else it is called the **org-repo**.

## What is in here

| Path | Applies to |
|---|---|
| `profile/README.md` | the landing page at `github.com/nithrune` |
| `CODE_OF_CONDUCT.md` | every repository without its own |
| `CONTRIBUTING.md` | every repository without its own |
| `SECURITY.md` | every repository without its own |
| `SUPPORT.md` | every repository without its own |
| `.github/ISSUE_TEMPLATE/` | issue forms offered across the org |
| `.github/PULL_REQUEST_TEMPLATE.md` | default pull request body |

The nested folder is not a mistake. GitHub looks for issue and pull
request templates one level down, inside a repository, and this
repository's own name collides with that path.

## What is NOT in here

**Licences.** GitHub does not support a default licence file — one has to
travel with each clone, so every repository ships its own. See
[CONTRIBUTING.md](CONTRIBUTING.md) for which licence goes where.

**Brand assets.** The Nithrune name and marks are not covered by this
repository's CC0 dedication. See [NOTICE](NOTICE).

## Licence

[CC0 1.0 Universal](LICENSE), with the carve-out in [NOTICE](NOTICE).
Take the templates, they are yours.
