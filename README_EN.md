<h1 align="center">Awesome Free Search APIs</h1>

<p align="center">
  <b>Free search / fetch / embedding API credits — curated, claimed, and verified by hand.</b><br>
  <i>Every entry was actually registered by us and the credit was seen in the console before listing.</i>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-22272e.svg?style=flat-square" alt="License"></a>
  <img src="https://img.shields.io/badge/Verified-2026--11--22-brightgreen.svg?style=flat-square" alt="Verified">
  <img src="https://img.shields.io/badge/Providers-7-blue.svg?style=flat-square" alt="Providers">
  <img src="https://img.shields.io/badge/Credit%20Card-Not%20Required-success.svg?style=flat-square" alt="No credit card">
</p>

<p align="center">
  <a href="./README.md">简体中文</a> | <a href="./README_EN.md">English</a>
</p>

---

## What this is

A list dedicated to **free credits for search-class APIs only**: web search, page fetching, embeddings and reranking. Every entry was registered by hand, the credit was verified in the provider's console, and the claim steps and traps are written down. Dead offers are marked dead, not deleted — so the next person doesn't waste an evening on them.

**Inclusion rules:** free, no credit card, personally claimed and verified. No rumors, no scraped lists.

---

## Contents

- [The haul at a glance](#the-haul-at-a-glance)
- [Which one should I pick?](#which-one-should-i-pick)
- [Keenable](#keenable) · [Exa](#exa) · [Tavily](#tavily) · [Tabstack](#tabstack) · [QuanticData](#quanticdata) · [Voyage AI](#voyage-ai) · [Mixedbread](#mixedbread)
- [Rules of this list](#rules-of-this-list)
- [Contributing](#contributing)

---

## The haul at a glance

| Provider | What | Free | Card? | Renews |
|---|---|---|---|---|
| [Keenable](#keenable) | Search + page fetch API | **100,000 requests/mo** | No | Monthly (resets on the 21st) |
| [Exa](#exa) | Search API for AI agents | **$10 signup + $10 onboarding + $10/mo ≈ ~4,300 searches in month one** | No | $10 monthly |
| [Tavily](#tavily) | Search API for AI agents | **1,000 credits/mo ≈ ~1,000 basic searches** | No | Monthly |
| [Tabstack](#tabstack) | Web access API (extract / research) | **10,000 credits ≈ ~1,000 page extracts** | No | One-time trial |
| [QuanticData](#quanticdata) | SERP + scraping APIs | **$2 credit/mo** | No | Monthly |
| [Voyage AI](#voyage-ai) | Embedding + rerank API | **200M tokens per model ≈ ~1M short-text embeddings** | No | One-time per account |
| [Mixedbread](#mixedbread) | Embedding + rerank + search API | **$5 Starter credit ≈ ~1,250 semantic searches** | No | One-time |

---

## Which one should I pick?

- **Search the web, maximum volume:** Keenable — 100k requests/mo.
- **Search the web, best quality for AI:** Exa or Tavily — results come with relevance scores.
- **Fetch one page's content:** Tabstack Extract, or QuanticData's scraping endpoints.
- **Let it research a topic across the web and summarize:** Tabstack Research.
- **Raw Google results (SERP):** QuanticData.
- **Embeddings / reranking (search-stack parts, they don't search the web themselves):** Voyage (200M tokens per model, the biggest haul) or Mixedbread.

---

## Keenable

- **What:** Web search and page-fetch API built for AI agents. One key covers search and fetch.
- **Free:** 100,000 search/fetch requests per month (≈100,000 calls), resetting on the 21st — about $400/mo at the $4-per-1k overage price.
- **Card:** Not required.
- **How to claim:**
  1. Sign up at [https://keenable.ai](https://keenable.ai) with an email address and verify it.
  2. Open the console at [https://app.keenable.ai](https://app.keenable.ai) and create an API key.
  3. Call `POST https://api.keenable.ai/v1/search` with header `X-API-Key: <key>`.
- **Traps (tested 2026-11-21):** Disposable / privacy email domains get only **1,000 requests/mo** instead of 100,000 — use a normal mailbox. A new key's full value is shown **once**, and only via the copy button — save it immediately. Rate limit 10 requests/second.

## Exa

- **What:** Search API designed for AI agents and RAG pipelines.
- **Free:** $10 for signing up + $10 for finishing onboarding, then $10 free every month. At the standard $7 per 1k searches, the first month's $30 buys ≈4,300 searches, then ≈1,400/month. When we claimed (2026-11), the codes `EXA20FREEBUFF` and `EXA20FIRESHIP` added $20 each — codes like these die without notice, test at claim time, don't trust old posts.
- **Card:** Not required. Email code login, no password.
- **How to claim:**
  1. Sign up at [https://exa.ai](https://exa.ai).
  2. Finish the onboarding flow to release the second $10.
  3. Create a key in the console and check each credit tranche's expiry date there.
- **Traps (tested 2026-11-19):** Credit tranches expire separately — one of our $10 tranches expired on 2026-12-01 while the rest stayed. Spend the expiring tranche first.

## Tavily

- **What:** Search / extract / crawl API for AI agents.
- **Free:** The Researcher plan is free forever: 1,000 credits per month, resetting monthly — ≈1,000 basic searches (1 credit each) or ≈500 advanced searches (2 credits each).
- **Card:** Not required.
- **How to claim:**
  1. Sign up at [https://app.tavily.com](https://app.tavily.com) with email + password and verify the email.
  2. The free plan is active immediately; create a key on the home page.
  3. Call `POST https://api.tavily.com/search` with header `Authorization: Bearer <key>`.
- **Traps (tested 2026-11-21):** The widely shared codes `GEEKROOM` (expired) and `GEEKROOM2` (fully redeemed) are **dead** — the "8,000 free credits" posts are stale. We verified both in the console; don't waste time on them.

## Tabstack

- **What:** Mozilla's web-access API for agents — Research / Extract / Generate / Automate. The free credits cover roughly 1,000 Markdown extracts or 40 fast research runs.
- **Free:** 10,000 credits on signup, shown in the console as "10,000 credits remaining" — ≈1,000 page extracts or ≈40 fast research runs.
- **Card:** Not required.
- **How to claim:**
  1. Sign up at [https://tabstack.ai](https://tabstack.ai) with an email address.
  2. Click the verification link in the email, then set an organization name and a password.
  3. The console at [https://console.tabstack.ai/dashboard](https://console.tabstack.ai/dashboard) shows the balance; create an API key there when you need one.
- **Traps (tested 2026-11-22):** The console calls it a "free trial" and does **not** print an expiry date for the credits — don't hoard them forever.

## QuanticData

- **What:** SERP, scraping, crawl and data APIs behind one key, billed per successful result only.
- **Free:** $2 of credit every month, no card — about 2,222 plain SERP searches or ~1,300 scraped pages at list price. Failed or blocked calls are never billed.
- **Card:** Not required.
- **How to claim:**
  1. Register at [https://app.quanticdata.io/register](https://app.quanticdata.io/register).
  2. Create a key at [https://app.quanticdata.io/api-keys](https://app.quanticdata.io/api-keys).
  3. Call `https://api.quanticdata.io/v1` with `Authorization: Bearer <key>`.
- **Traps:** The $2 covers the **Data APIs** only. Residential proxies are a separate product — the separate 100 MB proxy trial asks for SMS verification.

## Voyage AI

- **What:** Embedding and reranking models (MongoDB's Voyage), the retrieval layer for search and RAG.
- **Free:** A one-time allowance **per model, per account**: 200M tokens on each current model (voyage-4, voyage-4-large, voyage-4-lite, voyage-context-4, voyage-code-4, rerank-3, …), 50M on the domain models (voyage-finance-2, voyage-law-2, voyage-code-2), plus 200M text tokens and 150B pixels on the multimodal models. At ~200 tokens per passage, 200M tokens ≈ 1M short-text embeddings.
- **Card:** Not required.
- **How to claim:**
  1. Create an account at [https://dash.voyageai.com](https://dash.voyageai.com).
  2. In the API keys section, create a secret key — the free tokens are spent before any paid usage automatically.
- **Traps (tested 2026-11-21):** Free tokens do **not** apply to Batch API usage. The free tier's rate limits are low (we measured tier 0 at 3 RPM / 10k TPM) — fine for testing, not for bulk jobs. Free-tier content may be used for training unless you opt out.

## Mixedbread

- **What:** Embeddings, reranking and search APIs (mxbai models, Toast 1).
- **Free:** $5 one-time Starter credit, no card required. It does not renew and its expiry is not published. At $4 per 1k semantic searches that's ≈1,250 searches, or ≈20M content tokens indexed at the Fast rate of $0.25 per 1M tokens.
- **Card:** Not required.
- **How to claim:**
  1. Sign up at [https://www.mixedbread.com](https://www.mixedbread.com) (we used GitHub login).
  2. Create an API key in the platform console.
  3. Call `https://api.mixedbread.com/v1` with `Authorization: Bearer <key>`.
- **Traps (tested 2026-11-22):** One-time $5 only — our balance showed $4.98 after the first test calls. In the vendor's own words, data collected under the free tier is retained indefinitely.

---

## Rules of this list

- **Sources and steps only.** No accounts, no keys, no referral tricks.
- **Tested, not copied.** Every entry carries its verification date; the console is the source of truth.
- **Dead deals get marked, not deleted.**

## Contributing

PRs adding new search-class freebies or correcting dead offers are welcome. One inclusion rule: **personally registered and verified in the console**. Use the fixed format: what it is / how much (with approx. call counts) / card required? / claim steps / traps / verification date. No rumors, no copied lists.

Last verified: 2026-11-22.
