# Security Policy

## Reporting a vulnerability

**Do not open a public issue for a security problem.**

Use GitHub's private vulnerability reporting instead:

1. Go to the affected repository.
2. Open the **Security** tab.
3. Click **Report a vulnerability**.

That opens a private advisory visible only to you and the maintainer. No
email address is involved, and nothing is disclosed until a fix exists.

If the repository has that tab disabled, open a normal issue saying only
*"security report, please enable private reporting"* — no details — and
it will be turned on.

## What to include

- Which repository, and which version or commit.
- What an attacker can actually do with it.
- Reproduction steps, a config snippet, or a minimal test case.
- The software versions involved, if it is a runtime issue.

## What counts

These repositories hold server-side and client-side Minecraft content.
Worth reporting:

- Privilege escalation or arbitrary command execution.
- Behaviour that bypasses land protection, permissions or economy limits
  in a way that is clearly unintended.
- Credentials, tokens or private hostnames committed to a repository.
- Denial of service reachable by an unprivileged player.

Not vulnerabilities:

- Balance complaints. Something being too strong is a design issue — open
  a normal issue instead.
- Flaws in third-party software, or in Minecraft itself. Report those to
  whoever maintains them. Tell us as well if something here makes one
  materially worse.
- Anything that requires operator or console access to trigger.

## Response

Reports are read as time allows — this is unpaid, spare-time work, so no
response time is promised. Published advisories credit the reporter
unless anonymity is requested.
