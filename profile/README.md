<p align="center">
  <a href="https://maskbreak.com"><img src="https://maskbreak.com/favicon.svg" width="56" height="56" alt="Maskbreak"></a>
</p>

<h1 align="center">See the visit. Understand the risk.</h1>

<p align="center">
  <strong>Network intelligence and browser signals for signup, login, and checkout.</strong>
</p>

<p align="center">
  <a href="https://maskbreak.com">Website</a> ·
  <a href="https://maskbreak.com/api">API reference</a> ·
  <a href="https://maskbreak.com/signup">Get a free API key</a> ·
  <a href="https://maskbreak.com/blog">Guides</a>
</p>

---

## One visit. Signals you can act on.

**Maskbreak** helps developers assess suspicious visits before a sensitive action.
Send a browser SDK token to your backend, evaluate it server-side, and use the
returned `allow`, `review`, or `block` decision in your own policy.

- **Network context:** VPNs, proxies, Tor, and cloud-server signals. Service names are returned **when known**.
- **Browser context:** device fingerprints, signs of browser tampering, and automation signals.
- **A reason behind the decision:** inspect the score and signals, not just a yes/no answer.

A VPN alone calls for **review**, not a block. Signals are not proof of fraud.
Bare-IP lookups cover Tor and cloud-server ranges; VPN/proxy attribution and
device checks require an SDK-backed live visit.

**Free tier:** 1,000 visitor checks per hour, no credit card.
[See the current limits](https://maskbreak.com/pricing).

## Build with your stack

| Tool | Repository | Package |
| :--- | :--- | :--- |
| **Node.js SDK** | [maskbreak-node](https://github.com/sentinelsup/maskbreak-node) | [`@sentinelsup/sdk`](https://www.npmjs.com/package/@sentinelsup/sdk) |
| **Python SDK** | [maskbreak-python](https://github.com/sentinelsup/maskbreak-python) | [`sentinelsup`](https://pypi.org/project/sentinelsup/) |
| **PHP SDK** | [maskbreak-php](https://github.com/sentinelsup/maskbreak-php) | [`sentinelsup/sdk`](https://packagist.org/packages/sentinelsup/sdk) |
| **MCP server** | [maskbreak-mcp](https://github.com/sentinelsup/maskbreak-mcp) | [`@sentinelsup/mcp`](https://www.npmjs.com/package/@sentinelsup/mcp) |

The three server SDKs have no third-party runtime dependencies. All four
projects are MIT licensed. Existing `sentinelsup` package names are preserved
so integrations keep working.

## Start with a live-visit check

1. [Create an API key](https://maskbreak.com/signup).
2. Add the browser SDK to collect a visitor token.
3. Send the token to your backend and evaluate it there—keep the API key off the client.
4. Apply your own allow, review, or block policy before the protected action.

**[Follow the integration guide →](https://maskbreak.com/api)**
Node.js, Python, and PHP examples live in their repositories.
For an AI-assisted setup, use the [integration reference](https://maskbreak.com/integrate.md).

## Put it to work

[Account takeover protection](https://maskbreak.com/blog/account-takeover-endpoints) ·
[Signup abuse](https://maskbreak.com/blog/oauth-signup-fraud) ·
[Public-interest program](https://maskbreak.com/public-interest)

## Support & security

[Contact support](https://maskbreak.com/contact) ·
[Service status](https://maskbreak.com/status) ·
[Report a vulnerability privately](https://maskbreak.com/responsible-disclosure)

<sub>Built by <a href="https://github.com/kaspartomson20-alt">Kaspar Tomson</a> · Sentinel Edge Networks LTD · England &amp; Wales 17150600</sub>
