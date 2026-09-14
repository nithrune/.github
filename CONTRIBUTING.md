# Contributing

Thanks for looking. This is spare-time work, so the bar is *make it easy
to say yes* — small, verified, self-contained changes.

## Before you write code

**Open an issue first** for anything beyond a typo. A content change
often touches several files at once — definitions, drop logic, recipes
and documentation — so agreeing the shape first saves you rewriting it.

## Licensing — read this before your first pull request

Terms differ by repository, so each carries its own LICENSE. GitHub cannot
inherit one in any case: a licence file has to travel with the clone, which is
why it is the one community-health file that is never a default.

| Repository | Licence | Why |
|---|---|---|
| packs that ship Minecraft's own artwork | CC BY-NC-SA 4.0 | a grant here can only cover Nithrune's contribution, since the underlying pixels are Mojang's. Their guidelines forbid selling work built from those assets, which makes NonCommercial an obligation rather than a preference |
| everything else except `.github` | All rights reserved | entirely Nithrune's work. Forking, modifying or redistributing needs permission asked for first |
| `.github` | CC0 1.0 | boilerplate that exists to be copied, and nobody should have to attribute it |

**All rights reserved means what it says.** Downloading a release and running
it on your server is what these repositories are for. Copying the source, a
pack, a texture or a page of documentation into your own project, forking a
repository, or redistributing any of it is not permitted without explicit
written permission.

Ask by opening an issue in this repository. Permission is often given; it is
just not assumed.

**The first row follows content, never prefix.** A pack that ships Minecraft
artwork cannot be all rights reserved, because those pixels are not Nithrune's
to reserve. A pack generated from scratch can be. Each repository's own NOTICE
records which it is, and its licence follows from that.

**Contributions.** By opening a pull request you grant Nithrune a perpetual,
worldwide, irrevocable, royalty-free licence to use, modify, publish and
relicense your contribution as part of the project. You keep your own copyright
and may use your contribution elsewhere. This grant is needed because most of
these repositories reserve all rights: a licence that grants nothing cannot
carry a contribution back to the project. There is no separate CLA to sign.

`web-*` repositories take no contributions at all. Report a documentation
error as an issue on the repository the documentation is about.

The Nithrune name and marks are reserved separately from all of this and are
never licensed. Do not present your work as Nithrune's.

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
