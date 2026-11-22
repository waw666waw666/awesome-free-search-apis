<h1 align="center">Awesome Free Search APIs</h1>

<p align="center">
  <b>Free search / fetch / embedding API credits — curated, claimed, and verified by hand.</b><br>
  <i>Every entry was actually registered by us and the credit was seen in the console before listing.</i>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-Apache%202.0-22272e.svg?style=flat-square" alt="License"></a>
  <img src="https://img.shields.io/badge/Verified-2026--11--22-brightgreen.svg?style=flat-square" alt="Verified">
  <img src="https://img.shields.io/badge/Providers-6-blue.svg?style=flat-square" alt="Providers">
  <img src="https://img.shields.io/badge/Credit%20Card-Not%20Required-success.svg?style=flat-square" alt="No credit card">
</p>

<p align="center">
  <a href="./README.md">简体中文</a> | <a href="./README_EN.md">English</a>
</p>

---

## What this is

**Search keys for AIs that can't search.**

Most AI models and agents can't browse the web: ask one about today's news, the latest docs, or a fresh fix for an error and it has no way to look it up. This list collects the APIs that give them that ability — web search, page fetching, embeddings and reranking — with the free credits, claim steps and traps for each, every entry personally registered and verified in the provider's console before listing. Dead offers are marked dead, not deleted, so the next person doesn't waste an evening on them.

**What you can do with it**

- Wire a search endpoint into your agent, bot or AI app so it can look things up and read pages itself.
- Build it into your own project: RAG knowledge bases, research assistants, data scraping, competitor monitoring.
- Run on the free credits first to prove the integration works — the table converts every haul into approximate call counts — and only pay when you outgrow them.

**Inclusion rules:** free, no credit card, personally claimed and verified. No rumors, no scraped lists.

---

## Contents

- [The haul at a glance](#the-haul-at-a-glance)
- [Which one should I pick?](#which-one-should-i-pick)
- [Keenable](#keenable) · [Exa](#exa) · [Tavily](#tavily) · [Tabstack](#tabstack) · [Voyage AI](#voyage-ai) · [Mixedbread](#mixedbread)
- [Add-on zone: embeddings and reranking (not web search)](#add-on-zone-embeddings-and-reranking-not-web-search)
- [Rules of this list](#rules-of-this-list)
- [Contributing](#contributing)

---

## The haul at a glance

| Provider | What | Free | Card? | Renews |
|---|---|---|---|---|
| [Keenable](#keenable) | Search + page fetch API | **100,000 requests/mo** | No | Monthly (resets on the 21st) |
| [Exa](#exa) | Search API for AI agents | **$10 signup + $10/mo ≈ ~1,400 searches/month (onboarding $10 tested: not paid)** | No | $10 monthly |
| [Tavily](#tavily) | Search API for AI agents | **1,000 credits/mo ≈ ~1,000 basic searches** | No | Monthly |
| [Tabstack](#tabstack) | Web access API (extract / research) | **10,000 credits ≈ ~1,000 page extracts** | No | One-time trial |

---

## Which one should I pick?

- **Search the web, maximum volume:** Keenable — 100k requests/mo.
- **Search the web, best quality for AI:** Exa or Tavily — results come with relevance scores.
- **Fetch one page's content:** Tabstack Extract.
- **Let it research a topic across the web and summarize:** Tabstack Research.
- **Embeddings / reranking:** see the [add-on zone](#add-on-zone-embeddings-and-reranking-not-web-search) below — Voyage (200M tokens per model, the biggest haul) or Mixedbread.

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
- **Free:** $10 for signing up (expires 2026-12-01), then $10 free every month. At the standard $7 per 1k searches, $10 buys ≈1,400 searches. The $10 onboarding bonus shown on the home page does not pay out — see Traps. When we claimed (2026-11), the codes `EXA20FREEBUFF` and `EXA20FIRESHIP` added $20 each — codes like these die without notice, test at claim time, don't trust old posts.
- **Card:** Not required. Email code login, no password.
- **How to claim:**
  1. Sign up at [https://exa.ai](https://exa.ai).
  2. You can walk through onboarding, but don't count on its $10 bonus (see Traps).
  3. Create a key in the console and check each credit tranche's expiry date there.
- **Traps (tested 2026-11-19):** Credit tranches expire separately — one of our $10 tranches expired on 2026-12-01 while the rest stayed. Spend the expiring tranche first. Also note: this platform bans accounts — one of our accounts holding the full $60 was disabled on 2026-11-22 with its balance stranded. Spend credits promptly; don't hoard them. The $10 onboarding bonus is decorative — don't spend time on it: on 2026-11-22 we did every step there is — created a key, searched once ourselves, sent a team invite, had the invitee accept and join, and had the invitee run a search as a member — and checked billing three times; the balance only ever held the $10 signup credit. The bonus never arrived.

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

---

## Add-on zone: embeddings and reranking (not web search)

The two below **do not search the web**. They live in their own zone, separate from the search list above. They are parts inside a search engine: turning text into vectors (embeddings) and reordering results (reranking). You need them for RAG and for building your own site search — and the credits are real — so they are listed here, clearly labelled as not search engines.

| Provider | What | Free | Card? | Renews |
|---|---|---|---|---|
| [Voyage AI](#voyage-ai) | Embedding + rerank API | **200M tokens per model ≈ ~1M short-text embeddings** | No | One-time per account |
| [Mixedbread](#mixedbread) | Embedding + rerank + search over your own data | **$5 Starter credit ≈ ~1,250 semantic searches** | No | One-time |

### Voyage AI

- **What:** Embedding and reranking models (MongoDB's Voyage), the retrieval layer for search and RAG.
- **Free:** A one-time allowance **per model, per account**: 200M tokens on each current model (voyage-4, voyage-4-large, voyage-4-lite, voyage-context-4, voyage-code-4, rerank-3, …), 50M on the domain models (voyage-finance-2, voyage-law-2, voyage-code-2), plus 200M text tokens and 150B pixels on the multimodal models. At ~200 tokens per passage, 200M tokens ≈ 1M short-text embeddings.
- **Card:** Not required.
- **How to claim:**
  1. Create an account at [https://dash.voyageai.com](https://dash.voyageai.com).
  2. In the API keys section, create a secret key — the free tokens are spent before any paid usage automatically.
- **Traps (tested 2026-11-21):** Free tokens do **not** apply to Batch API usage. The free tier's rate limits are low (we measured tier 0 at 3 RPM / 10k TPM) — fine for testing, not for bulk jobs. Free-tier content may be used for training unless you opt out.

### Mixedbread

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
