# Security Policy

**The full policy lives at
[maskbreak.com/responsible-disclosure](https://maskbreak.com/responsible-disclosure).**
That page is authoritative — scope, response targets, safe harbour and
coordinated-disclosure terms are all defined there. This file exists so GitHub
has something to point at; it deliberately does not restate the policy, because
two copies drift.

## Reporting

Email **support@maskbreak.com** with the subject `[SECURITY] <short title>`.

Do not include live credentials, personal data, or an unredacted exploit in the
first email — ask for an encrypted channel and one will be arranged after
acknowledgement. Do not open a public issue, here or anywhere else, before a
coordinated disclosure date is agreed.

Acknowledgement target is **2 business days**, triage within 5. There is no
paid bug-bounty programme; public credit and swag are offered instead.

## What this org covers

The published packages — `@sentinelsup/sdk`, `sentinelsup` (PyPI),
`sentinelsup/sdk` (Packagist) and `@sentinelsup/mcp` — are in scope, as is the
API they call. Only the latest release of each SDK receives fixes.

One thing worth stating before it arrives as a report: **detection evasion is
not a vulnerability.** Finding a way to make traffic look clean to the engine
is a product limitation. It is still worth telling us about, at the same
address, but it is not a security issue and is not covered by safe harbour.
