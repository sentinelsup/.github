# Security Policy

## Reporting a vulnerability

Email **support@maskbreak.com** with `SECURITY` in the subject. Please include
enough detail to reproduce: affected endpoint or package, the request you sent,
what you got back, and what you expected.

Do not open a public issue for a security report.

We aim to acknowledge every report within three business days. There is no paid
bug bounty at this time.

## Scope

In scope:

- The API at `maskbreak.com` — `/v1/evaluate`, `/v1/lookup`, and the account
  and dashboard endpoints
- The official SDKs: `@sentinelsup/sdk`, `sentinelsup` (PyPI),
  `sentinelsup/sdk` (Packagist), `@sentinelsup/mcp`
- `maskbreak.com` itself, including the console and authentication flows

Out of scope:

- Reports from automated scanners with no demonstrated impact
- Missing hardening headers with no exploitable consequence
- Denial of service, volumetric or otherwise — please do not test this
- Social engineering of our staff or customers
- Detection evasion. Finding a way to make traffic look clean to our engine is
  a product limitation, not a vulnerability. We are still interested, and
  `support@maskbreak.com` is the right address, but it is not a security report.

## Disclosure

Please give us 90 days before publishing. We will credit you when the fix
ships, unless you would rather stay anonymous.

## Supported versions

The API is versioned and additive — see the stability policy at
[maskbreak.com/api](https://maskbreak.com/api). For the SDKs, only the latest
release of each receives fixes.
