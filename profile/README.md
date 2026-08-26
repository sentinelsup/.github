<p align="center">
  <a href="https://maskbreak.com">
    <img src="https://maskbreak.com/favicon.svg" width="72" height="72" alt="Maskbreak">
  </a>
</p>

<h1 align="center">Maskbreak</h1>

<p align="center">
  <strong>Real-time fraud detection that stops VPNs, residential proxies, antidetect browsers, and AI bots — in under 40 ms.</strong>
</p>

<p align="center">
  <a href="https://maskbreak.com">Website</a>
  ·
  <a href="https://maskbreak.com/api">API Docs</a>
  ·
  <a href="https://maskbreak.com/blog">Blog</a>
  ·
  <a href="https://maskbreak.com/signup">Free API Key</a>
</p>

---

## What is Maskbreak?

Maskbreak is a fraud detection API built for teams who've outgrown IP blocklists.

Modern attackers don't use datacenter VPNs anymore — they rent residential proxies, spoof browser fingerprints with Kameleo/GoLogin, and run automation at scale. Tools built around IP reputation (IPQS, SEON, Sift) miss most of that traffic.

Maskbreak combines network analysis with device fingerprinting to catch what they can't:

- 🏠 **Residential proxy detection** — BrightData, Smartproxy, IPRoyal, ShadowNode
- 🎭 **Antidetect browser tampering** — Kameleo, GoLogin, AdsPower, Multilogin
- 🤖 **Bot & automation detection** — Puppeteer, Playwright, Selenium, agentic AI
- 🆔 **Persistent visitor ID** — survives incognito, VPN switching, cookie clears
- 🌍 **<40 ms p95 globally** — runs in your critical path without slowing it down

## Free tier

1,000 requests per hour, every detection signal, no credit card.

→ [Get a key in 2 minutes](https://maskbreak.com/signup)

## Official SDKs

| Language | Repository | Package |
|----------|-----------|---------|
| Node.js | [`maskbreak-node`](https://github.com/sentinelsup/maskbreak-node) | [![npm](https://img.shields.io/npm/v/@sentinelsup/sdk.svg?label=%40sentinelsup%2Fsdk)](https://www.npmjs.com/package/@sentinelsup/sdk) |
| Python | [`maskbreak-python`](https://github.com/sentinelsup/maskbreak-python) | [![PyPI](https://img.shields.io/pypi/v/sentinelsup.svg?label=sentinelsup)](https://pypi.org/project/sentinelsup/) |
| PHP | [`maskbreak-php`](https://github.com/sentinelsup/maskbreak-php) | [![Packagist](https://img.shields.io/packagist/v/sentinelsup/sdk.svg?label=sentinelsup%2Fsdk)](https://packagist.org/packages/sentinelsup/sdk) |

All three are zero-dependency and MIT licensed. Package names keep the
`sentinelsup` prefix from before the rename — renaming a published package
breaks every existing install.

## Quick start

**Node.js**

```bash
npm install @sentinelsup/sdk
```

```js
const Sentinel = require('@sentinelsup/sdk');
const sentinel = new Sentinel({ apiKey: process.env.SENTINEL_KEY });

const result = await sentinel.evaluate({ token: req.body.sentinelToken });
if (result.decision === 'block') return res.status(403).end();
```

**Python**

```bash
pip install sentinelsup
```

```python
from sentinel import Sentinel

sentinel = Sentinel()  # reads SENTINEL_KEY
result = sentinel.evaluate(token=request.json["sentinelToken"])
if result.decision == "block":
    abort(403)
```

**PHP**

```bash
composer require sentinelsup/sdk
```

```php
$sentinel = new \Sentinel\Client();   // reads SENTINEL_KEY
$result = $sentinel->evaluate(['token' => $_POST['sentinelToken']]);
if ($result->isBlocked()) {
    http_response_code(403);
    exit;
}
```

**Any other stack** — point your AI coding assistant at
[`maskbreak.com/integrate.md`](https://maskbreak.com/integrate.md) and it wires the
integration for you, or call `POST /v1/evaluate` directly ([API docs](https://maskbreak.com/api)).

## Where Maskbreak fits

| Use case | What it stops |
|----------|---------------|
| [Stripe checkout](https://maskbreak.com/blog/card-testing-attacks) | Card testing, chargeback-prone sessions |
| [Shopify drops](https://maskbreak.com/blog/shopify-bot-detection) | Sneaker bots, scalpers, scrapers |
| [SaaS signup](https://maskbreak.com/blog/oauth-signup-fraud) | Multi-accounting, bonus abuse, fake Google sign-ins |
| [Fintech KYC](https://maskbreak.com/case-studies/fintech-fake-accounts) | Synthetic identities, proxy-masked applications |

## Comparisons

[vs IPQS](https://maskbreak.com/vs/ipqs) ·
[vs SEON](https://maskbreak.com/vs/seon) ·
[vs Sift](https://maskbreak.com/vs/sift) ·
[vs Kount](https://maskbreak.com/vs/kount) ·
[vs minFraud](https://maskbreak.com/vs/minfraud)

## Contact

- 🐦 [@MaskbreakSup on X](https://x.com/MaskbreakSup)
- 📬 [support@maskbreak.com](mailto:support@maskbreak.com)
- 📊 [Status page](https://maskbreak.com/status)

---

<sub>© Sentinel Edge Networks LTD · Registered in England &amp; Wales 17150600 · London, UK</sub>
