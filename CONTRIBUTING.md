# Contributing

Thanks for looking. This is spare-time work, so the bar is *make it easy
to say yes* — small, verified, self-contained changes.

## Before you write code

**Open an issue first** for anything beyond a typo. A content change
often touches several files at once — definitions, drop logic, recipes
and documentation — so agreeing the shape first saves you rewriting it.

## Licensing — read this before your first pull request

There is no organisation-wide licence. GitHub cannot inherit licence
files, and code and artwork want different terms:

| Repository | Licence | Why |
|---|---|---|
| `tool-*`, `mod-*` | MIT | standalone; maximum reuse |
| `plugin-*` | GPL-3.0 | the server API these are compiled against is GPL-3.0, so a plugin is arguably a derivative work; matching it removes the question |
| `mobpack-*`, `rp-*` | CC BY-NC-SA 4.0 | creative content, not software: credit required, share-alike, no commercial reuse |
| `.github` | CC0 1.0 | boilerplate nobody should have to attribute |

**By opening a pull request you agree your contribution is licensed under
that repository's licence.** Inbound equals outbound; there is no separate
CLA to sign.

The Nithrune name and marks are excluded from every licence above. Fork
the code freely; do not ship it as Nithrune.

**Never contribute anything you do not hold the rights to.** Assets taken
from another creator's pack, from a paid resource, or extracted from
commercial software will be rejected. So will Minecraft's own assets.

## Conventions

**Language.** Write to us in **English**: issues, pull requests, commit
messages, documentation and code comments. It is the only language every
contributor here shares.

This says nothing about the content a repository ships. Which language its
user-facing text speaks is decided in that repository and stated in its
README — do not change it to match this rule.

**Naming.** Identifiers carry their repository's prefix and follow
whatever style that repository already uses. Do not introduce a second
convention alongside an existing one.

**Textures are generated from code**, not drawn by hand and not produced
by an image model. A pull request adding a `.png` without the source that
draws it will be asked for the source. This is what keeps a set of forty
items looking like one set.

**Commits** describe the change, not the session: *Fix ability firing on
client-side hits*, not *updates*. One logical change per commit.

## Verifying a change

A green parse proves nothing. Configuration that parses perfectly can
still fail to load, silently skip a step, or throw on first use.

Before you open a pull request:

1. Load the change on a real server or client of the version the
   repository targets.
2. Reload or restart, and read the **whole** log — not just the part you
   expected to change. Any new warning, error or exception means it is
   not ready.
3. Actually trigger the thing you changed, **in survival mode**. Creative
   mode makes item consumption a no-op, so anything that costs the player
   an item will look broken, or look fine for the wrong reason.
4. Say in the pull request what you ran and what the log showed.

"It should work" is not a verification step.

## Pull requests

- Branch off `main`, one topic per branch.
- Keep the diff to the topic. Unrelated reformatting hides the change.
- Fill in the template — especially the verification section.
- Draft pull requests are welcome for early feedback; mark them ready
  once tested.

## Reporting instead of fixing

That is fine, and often more useful. See [SUPPORT.md](SUPPORT.md) for
where things go, and [SECURITY.md](SECURITY.md) for anything that should
not be public.
