<!-- Paste this into a new repo called `.github` in your GitHub organization,
     at the path  profile/README.md  — GitHub auto-renders it on your org page.
     If you don't have an org, create one: https://github.com/account/organizations/new -->

<p align="center">
  <a href="https://sntlhq.com">
    <img src="https://sntlhq.com/favicon.svg" width="72" height="72" alt="Sentinel">
  </a>
</p>

<h1 align="center">Sentinel</h1>

<p align="center">
  <strong>Real-time fraud detection that stops VPNs, residential proxies, antidetect browsers, and AI bots — in under 40 ms.</strong>
</p>

<p align="center">
  <a href="https://sntlhq.com">Website</a>
  ·
  <a href="https://sntlhq.com/api">API Docs</a>
  ·
  <a href="https://sntlhq.com/blog">Blog</a>
  ·
  <a href="https://sntlhq.com/signup">Free API Key</a>
</p>

---

## What is Sentinel?

Sentinel is a fraud detection API built for teams who've outgrown IP blocklists.

Modern attackers don't use datacenter VPNs anymore — they rent residential proxies, spoof browser fingerprints with Kameleo/GoLogin, and run automation at scale. Tools built around IP reputation (IPQS, SEON, Sift) miss ~70% of that traffic.

Sentinel combines network analysis with device fingerprinting to catch what they can't:

- 🏠 **Residential proxy detection** — BrightData, Smartproxy, IPRoyal, ShadowNode
- 🎭 **Antidetect browser tampering** — Kameleo, GoLogin, AdsPower, Multilogin
- 🤖 **Bot & automation detection** — Puppeteer, Playwright, Selenium, agentic AI
- 🆔 **Persistent visitor ID** — survives incognito, VPN switching, cookie clears
- 🌍 **<40 ms p95 globally** — runs in your critical path without slowing it down

## Free forever

- 1,000 API requests per hour
- No credit card required
- Full feature access (not a gimped free tier)

→ [Get a key in 2 minutes](https://sntlhq.com/signup)

## Quick start

```bash
npm install @sentinel/sdk
```

```js
const Sentinel = require('@sentinel/sdk');
const sentinel = new Sentinel({ apiKey: process.env.SENTINEL_KEY });

const result = await sentinel.evaluate({ token: req.body.sentinelToken });
if (result.isSuspicious) return res.status(403).end();
```

## Where Sentinel fits

| Use case | What it stops |
|----------|---------------|
| [Stripe checkout](https://sntlhq.com/blog/stripe-fraud-detection-api) | Card testing, chargeback-prone sessions |
| [Shopify drops](https://sntlhq.com/blog/shopify-bot-detection) | Sneaker bots, scalpers, scrapers |
| [SaaS signup](https://sntlhq.com/blog/oauth-signup-fraud) | Multi-accounting, bonus abuse, fake Google sign-ins |
| [Fintech KYC](https://sntlhq.com/blog/fintech-fake-account-fraud) | Synthetic identities, proxy-masked applications |

## Comparisons

- [vs IPQS](https://sntlhq.com/vs/ipqs)
- [vs SEON](https://sntlhq.com/vs/seon)
- [vs Sift](https://sntlhq.com/vs/sift)
- [vs Kount](https://sntlhq.com/vs/kount)
- [vs minFraud](https://sntlhq.com/vs/minfraud)

## Stay in the loop

- 🐦 [@SentinelSup on X](https://x.com/SentinelSup)
- 💼 [Founder on LinkedIn](https://www.linkedin.com/in/raigo-mets-9b6268402/)
- 📬 [support@sntlhq.com](mailto:support@sntlhq.com)

---

<sub>© Sentinel Edge Networks LTD — London, UK</sub>
